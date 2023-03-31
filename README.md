

문서정보 : 2023.03.29. 작성, 작성자 [@SAgiKPJH](https://github.com/SAgiKPJH)

<br>

# FASTAPI_Python_C#
Fast API in Python And C#

### 목표
* [ ] FastAPI
  * [x] FastAPI에 대해서 조사합니다.
  * [ ] FastAPI를 이용하여 간단한 RESTful API를 구현합니다.
  * [ ] 서비스로 등록하여 실행합니다.
    * [ ] Window C#
    * [ ] Linux Python
* [ ] RabbitMQ
  * [ ] RabbitMQ에 대해서 조사합니다.
  * [ ] RabbitMQ를 이용하여 간단하게 실행합니다.
  * [ ] RabbitMQ를 이용하여 메세지를 전송합니다.
  * [ ] FastAPI를 통해 메시지 큐를 구성합니다.
  * [ ] FastAPI를 통해 메시지를 받아 처리하는 기능을 추가합니다.
* [ ] Keras/TensorFlow
  * [ ] Keras/TensorFlow에 대해서 조사합니다.
  * [ ] Keras/TensorFlow 예제를 작성합니다.
  * [ ] FastAPI 앱에서 로드하고 사용하는 기능을 구현합니다.
  * [ ] 메모리 확인합니다.
* [ ] 핵심 목표
  * [ ] Python 실행 중 모델 내리고 올릴려봅니다.
  * [ ] 메모리 상태를 확인합니다.
* [ ] ...

### 제작자
[@SAgiKPJH](https://github.com/SAgiKPJH)

---

# FastAPI에 대해서 조사합니다.

### FastAPI란?
- [-웹 프레임워크-]
- [-Python 3.7 이상-] 버전에서 [-작동-]하는 웹 프레임워크 
- 비동기식(Asynchronous) 코드를 지원
- 빠른 속도와 적은 양의 코드로 RESTful API를 구현

### RESTful이란?

- Representational State Transfer
- 웹의 장점을 최대한 활용할 수 있는 아키텍처
- RESTful API는 REST 아키텍처 스타일의 제약 조건을 준수하고 RESTful 웹 서비스와 상호 작용할 수 있도록 하는 애플리케이션 프로그래밍 인터페이스(API)

### 참고 사이트
- [FastAIP Tutorial](https://fastapi.tiangolo.com/ko/tutorial/)
- [FastAPI First Steps](https://fastapi.tiangolo.com/ko/tutorial/first-steps/)
- [네트워크 REST API란? REST RESTful이란?](https://khj93.tistory.com/entry/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-REST-API%EB%9E%80-REST-RESTful%EC%9D%B4%EB%9E%80)

<br><br><br>

# FastAPI를 이용하여 간단한 RESTful API를 구현합니다.

### python

1. FastAPI 설치 및 간단 구성
   ```bash
   pip install fastapi

   # FastAPI 실시간 미리보기 라이브러리
   pip install "uvicorn[standard]"
   ```
   - FastAPI 인스턴스를 생성하고 "/" 경로로 들어오는 GET 요청에 대해 "Hello World" 메시지를 반환
   ```py
   from fastapi import FastAPI

   app = FastAPI()

   @app.get("/")
   def read_root():
       return {"Hello": "World"}
   ```
   ![image](https://user-images.githubusercontent.com/66783849/228773734-2a67ee25-9fb0-472e-b62a-283d128e2b49.png)  
2. FastAPI 서버 실행 및 접속
   ```bash
   # main.py 파일에서 app 객체를 가져와서 Uvicorn 서버를 시작
   #  "--reload" 플래그를 사용하면 코드가 변경될 때마다 자동으로 서버가 재시작
   uvicorn main:app --reload

   # Directory 안에 존재할 경우, "/"가 아닌 "."으로 구분합니다.
   uvicorn python.fastapi:app --reload # python/fastaip.py인 경우
   ```
   - `http://localhost:8000`로 접속
   - 또는 CLI `curl http://localhost:8000`를 통하여 GET 요청  
   ![image](https://user-images.githubusercontent.com/66783849/228773807-999313f3-d2c8-4682-a2c8-28eb4e6cbc90.png)

<br><br><br>

#

<br><br><br>

#

<br><br><br>

#

<br><br><br>

#

<br><br><br>

#
