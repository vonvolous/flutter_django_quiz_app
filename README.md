# flutter_django_quiz_app

## Useful URL

A few resources for Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)
- [online documentation](https://docs.flutter.dev/)
- [Dark SDK downgrade for flutter swiper](https://polarcompass.tistory.com/227)
- [null-safety issue](https://postforty.tistory.com/79)
  * In VS Code: Manage->Setting->Flutter Run Additional Args->Add Item
  ```shell
  --no-sound-null-safety
  ```

### 1. 플러터 프론트엔드 반응형 앱 만들기
  * 프로젝트 구조 설정 및 홈 화면 만들기 ✅
  * 퀴즈 모델 및 풀기 화면 만들기 ✅
  * 퀴즈 결과 화면 만들기 ✅

### 2. 장고 백엔드 API 서버 만들기
  * Django Rest Framework 개발 및 API 만들기 ✅
    - 가상 환경: 
    ```python
      $ sudo apt install virtualenv
      $ virtualenv {env name} //가상 환경 생성
      $ source quiz/bin/activate // 가상 환경 활성화
    ```
    <br />
    - django 설치:
    1. pip install django djangorestFramework
    2. django-admin startproject {myapi} . //프로젝트 생성
    3. python manage.py startapp {app name} // 앱 폴더 생성
    <br />
    - django app 실행:
    1. python manage.py makemigrations
    2. python manage.py migrate
    3. python manage.py runserver
    <br />
    - 관리자 설정:
    1. python manage.py createsuperuser
    2. 서버 실행후 /admin으로 이동해 로그인
    3. quiz app에 quiz 추가 가능해짐
  * Django project를 heroku에 deploy하기

### 3. 플러터와 API 연동하기