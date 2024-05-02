# Django_study

## 1번째 강의


### pwd
#### 현재 위치 확인



### 서버 실행시키는 방법
#### python manage.py runserver



### 프로젝트 생성
#### django-admin startproject "프로젝트 이름"



### 새로운 앱 생성
#### django-admin startapp "앱 이름"



### 데이터베이스 생성 및 초기화
#### python manage.py makemigration
#### python manage.py migrate



### 관리자 계정 생성
#### python manage.py createsuperuser

## 2번째 강의

### url과 url이어주기
#### url과 url을 이어주기 위해서 우선 아무것도 없는 상태인 ' '를 새로운 html과 연결해주기 위해 inflearn_lecture app의 url과 연결시켜준뒤 html과 연결시켜주려고 한다.
#### path(' ', include('inflearn_lecture.urls'))
#### urls에서 바로 html과 연결하는 것은 불가능하기 때문에 views를 통해서 html과 연결시켜준다.
#### views.py
##### def home_list(request) :
#####       return render(request, 'inflearn_lecture/home_list.html')
#### urls.py
##### urlpatterns = [
#####       path(' ', views.home_list, name = 'home_list') ]

### html 폴더
#### html 파일을 저장하는 폴더는 templates라는 폴더를 따로 만들어서 저장해준다.
