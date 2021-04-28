![Write_Call](https://user-images.githubusercontent.com/59414764/114134492-ce1f9680-9942-11eb-99e0-bb6a51a8bd0b.gif)

# Write-Call
"CNN을 어떻게 실생활에 적용시켜볼 수 있을까?"
<b>손글씨로 거는 전화</b>

## 구현환경
- Tensorflow(Keras), Tensorflow-Lite, Python
- Android Studio, Kotlin

## Dev Note
<details>
  <summary><b> ~ 2020년 4월 9일</b></summary>
  
  1. MNIST 숫자 데이터를 이용하여 CNN 모델 만들기
  2. mnist.tflite(Tensorflow Lite) 모델 파일 변형하기
  3. 안드로이드의 그림판 패키지를 이용하여 분류할 input data 생성
  4. mnist.tflite이 적용된 tensorflow-lite 패키지를 이용하여 input data 숫자 인식하기
  5. 얻어낸 숫자들과 intent를 이용하여 전화로 연결 📞
  
</details>
<details>
  <summary><b> ~ 2020년 4월 23일</b></summary>
  
  Feedback
  1. 단순 Toy Project로 끝내지 말자 ⭐
  2. 배운 것을 현 프로젝트에 어떻게 적용시켜볼 수 있을까 그때 그때 고민해보자 
  3. 한 글자씩 입력해야하는 단점이 있다. 한꺼번에 쓰고 text를 detection을 통해 한 글자씩 찾고 Recognition. 글자들의 위치 정보를 이용하여 문자를 순서대로 배열하면 되지 않을까?
  4. 모델의 tflite 파일(모델 정보 및 가중치)을 갱신해야할 때도 있다. 서버를 이용해 갱신할 수 있도록 만들자.
  5. 모델 성능 개선을 위해 사용시 즉각 데이터를 수집하는 것도 필요해보인다. differential privacy 정책에 의하면 온전한 데이터를 서버에 보내는 것이 아닌, 일부 학습된(사람이 해석할 수 없는) 가중치만을 서버에 보낼 필요가 있어보인다. 모바일 환경에서 NDK라는 것을 사용하면 되지 않을까? Classifier만 학습하도록 하면 되지 않을까?
  6. 나중에 숫자 뿐만 아니라 글씨도 알아볼 수 있도록 하면 좋을 것 같다. ~~텍스트 분석도 해야하려나~~
  7. Random Ferns, Bayesian 이론을 여기에 적용할 수도 있을까?

  공부해야할 것들 - 다 할 필요는 없다 천천히 하나씩 꼼꼼하게
  1. Text Detection, Recognition OCR 논문 리뷰 - (볼 것은 많다...이활석님 Github https://github.com/hwalsuklee/awesome-deep-text-detection-recognition)
  2. Kotiln 공부
  3. C++ 복습 (교재: 전문가를 위한 C++)
  4. ML, DL 공부 - (https://github.com/xcellentbird/Deep_Learning)
  5. Android(Linux, NDK), API(Firebase, OpenCV, Tensorflow-Lite) - (https://github.com/xcellentbird/Study-Android)
  6. Django, Naver Cloud, Networks - Backends
  7. 기술 철학
  
  Community를 활용하자.
  - 현 DL 논문 리뷰 스터디를 통해 OCR 논문을 리뷰하고, 다른 의견을 들어보자. 영어 논문을 읽는 것에 익숙해지자. ~~영어 공부도 좀~~
  - KDT 데브 코스를 통해, 중급 이상의 ML지식, Sparks, Django 공부하자.
  - Android 스터디를 통해 UI, OS 등을 공부하고 실제 Android App을 만들어보자. 사용자 경험을 분석하고, AI 윤리 규칙을 고려하여 개발해보자.
  - 모르는 것은 Kaggle Korea, Keras Korea, Vision-AI 오픈 카톡방을 이용해 물어보자! ~~열심히 하는 모습이 눈에 띄면 더 좋잖아?~~
  
  TMI
  - 색채 심리학과 Vision Machine의 결합은 어떤 UX로 이어지며 어떻게 디자인 할 수 있을까? ~~Clova Rush에 참여할 수 있으면 좋으련만 ㅠ~~
  - 조만간 Github Study Repo 통합이 필요해보인다.
  - 개발자에게 필요한 역량? 집요함과 약간의 유연성, 문제해결능력, 언어 및 프레임워크에 대한 깊은 지식, CS 지식(알고리즘, 운영체제, 컴퓨터구조, 자료구조, 네트워크, DB)
  - 좋아하는 공부를 하는 것도 좋지만, 사회의 Needs를 분석하고, 그에 맞는 기술을 공부하는 것 또한 중요하다. - AI Engineer + ML Ops + Android (+ iOS)
  - 내가 높은 연봉을 바라는 것은, 순수하게 돈을 위해서가 아닌, 프로젝트에서 꼭 필요한 사람이라고 느낄 수 있는 대우를 바라고, 아쉽지만 그에 대한 지표가 연봉이기 때문이다.

</details>
