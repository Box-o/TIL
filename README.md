# TIL

**<11월 20일 월요일>**

**타임차트**
부트캠프 초대방 합류 2:41 출석 3시 쯤
서약서 서명, 훈련생 정보 제출, 등록 문제로 임시 출석 시스템 사용

OT zoom 못들어서 docs 노션을 읽어봄
안드로이드 학습자료 Gitbook에서 안드로이드 스튜디오 설치까지 진행 후 강의 진행

1. 안드로이드 스튜디오 설치 후 기본 기능 사용 (시물레이션, SDK설치)
2. BMI 계산기 따라하기 (Main view에서 컴포넌트 배치하고 align 해보기, 시물레이션으로 실제 모습 확인)
3. BMI 계산기 따라하기 (Main view에 이어 Result view를 만들어 id 할당하기, **컴파일 문제 해결못함**)



**오늘 코딩하며 배운 것 / 1주차 BMI계산기**

**activity.kt**
activity창의 메인 코드를 작성하는 공간

**activity.xml**
activity창의 레이아웃을 배치하거나 코드 작성하는 공간
preview기능이 있어 블럭 배치 후 코드를 다듬을 수 있다
각 블럭의 점을 사용하여 코드를 작성하지 않아도 정렬할 수 있다



***문제점**
Hardcoded string shude use @string resource
똑같이 따라한 것 같은데 뭔가 문제가 있는 듯
오타가 있거나..

Proxy setting
ㄴ 핫스팟 사용해서 그런건지?



**요약**
Android 개발 종합반 1주차의 문제를 찾다가 끝남, 해결못함
내일 다시 처음부터 시도해 봐야겠다




**<11월 21일 화요일>**

***이전 문제해결**
어제의 문제는 ImageView id를 변경하다 요소의 끝을 누락함 ex: ~@+id/tv_resText" **/>**
하나의 오류로 여러 장소에 에러가 발생해 어제는 찾지 못했으나 오늘 해결함



**타임차트**
부트캠프 출석 8:50 등록 문제로 임시 출석 시스템 사용
11시 장세진 튜터의 '개발자의 마음가짐' 세션 참가
ㄴ개발자가 왜 되고싶은지, 개발자가 되어 해보고 싶은 것, 개발자가 가지면 좋은 마음가짐, 1기 수강생들의 결과물 Preview
12:30 2주차 로또번호 생성기 강의 시작



**오늘 코딩하며 배운 것 / 1주차 BMI계산기**

**변수 Var Val**
Var = 가변(mutable) 변수
ㄴ지정된 값을 계속 변경할 수 있음

Val = 불변(immutable) 변수
ㄴ변수가 상수로 취급되어 한번 지정한 값은 변하지 않음

컴파일 에러, 변수에 대한 이해가 부족해 오탈자 찾는데 많은 시간 소요

**선언한 id 호출**
R.id.[id명]

**drawable폴더의 이미지 호출**
R.drawable.[이미지 이름]

**if, else if, else**
if([조건문]){
  resultText = "정답입니다"
  //_조건문이 참일 경우 위 명령을 가변변수에 적용한다_
} else if([조건문]){
  resultText = "틀렸습니다"
  //_if조건문이 참이 아닐 경우 위 명령을 가변변수에 적용한다_
} else {
  resultText = "숫자를 입력해 주세요"
  //_모든 조건문이 참이 아닐 경우 위 명령을 가변변수에 적용한다_

1주차 숙제 배운점 정리
BMI 계산기를 만들어 보는 수업이였습니다

무작정 따라해 보고 레이아웃에 컴포넌트 배치와 정렬을 해 보았습니다
가변과 불변의 변수개념을 몰라 코드에 오류가 많아 일부 지우고 다시 따라하다 문제를 찾았습니다

각 버튼과 이미지에 id를 할당하고 가변 변수에 if조건에 따른 여러 값을 지정한 후 텍스트와 이미지를 출력해 보았습니다
math의 pow 기능으로 반올림을 구현해 보았습니다



**오늘 코딩하며 배운 것 / 2주차 로또번호 생성기**
무지성 따라하긴 했고 문제없이 끝냈는데 뭔소린지 모르겠다
한 40% 이해한듯 gitbook Chapter3를 공부해 보고 2주차 복습을 다시해 볼 예정
gitbook이 끝나면 내가 따라 작성한 코드에서 다르게 바꿔보며 확인해 봐야겠다



**오늘 코딩하며 배운 것 / gitbook Chapter3**

<작성코드> Log 사용 시 자동으로 'android.util.Log'가 import됨
Log.v("BasicSyntax", "로그를 출력합니다. method = Log.v")
Log.d("BasicSyntax", "로그를 출력합니다. method = Log.d")
Log.i("BasicSyntax", "로그를 출력합니다. method = Log.i")
Log.w("BasicSyntax", "로그를 출력합니다. method = Log.w")
Log.e("BasicSyntax", "로그를 출력합니다. method = Log.e")

<실제 출력 로그>
 D  로그를 출력합니다. method = Log.d   //cyen      개발자용 로그
 I  로그를 출력합니다. method = Log.i   //green     인포 로그
 W  로그를 출력합니다. method = Log.w   //yellow    경고 로그
 E  로그를 출력합니다. method = Log.e   //red       에러 매시지 출력

무슨 차이로 구분하는지 아직은 잘 모르겠다
Log.v는 logcat에 나타나지도 않음

내 경험상 error와 warning은 한 카테고리로 묶어 'Error code'로 확인하고
info는 현재 진행 상황을 알리는데 사용할 수 있을 것 같고, 각 로그 상세보기 시 나타내는 것이 verbose로 추청된다
rollout 전 popup display를 만들어 테스트가 가능할 것도 같다?
ㄴ자세한 질문은 gitbook을 모두 끝낸 후 한번에 물어볼 예정

변수 Var
변경 가능한 값을 저장할 수 있는 공간
값을 사용하거나 변경하고 싶을 때 Var로 지정한 공간을 호출해서 사용 가능하다
예시1) Var 변수명 = "박상우"
ㄴ이 경우 String으로 선언됨
예시2) Var 변수명 : String
      변수명 = 123
ㄴ이 경우 String으로 선언되었기 때문에 정수는 사용할 수 없음

데이터 타입
Boolean = true/false
String = 문자열
Char = 문자 1개
Byte = 8비트 정수
Short = 16비트 정수
Int = 32비트 정수
ㄴ아래 3개 중 32비트 정수값이 표현 범위가 제일 넓다
  Int외 정수들은 안써봐서 언제 쓰는지는 잘 모르겠다
ㄴChar도 마찬가지 String에서 한글자만 써지는데?
  구글검색 결과 특정 API에서 Char을 반환하거나 입력할 때 사용한다고 한다
  일반적인 경우에는 잘 사용하지 않는다고 한다
 
<미니 퀴즈>
실제 에러를 출력하기 위한 로그함수의 이름은 무엇일까요?
Error / Log.e
개발자들이 보기 위한 목적으로 사용되는 로그함수의 이름은 무엇일까요?
Debug / Log.d
특정 로그를 필터링하기 위해 사용되는 로그함수의 첫 번째 파라미터는 무엇일까요?
level:debug

 

**이것저것 눌러보다 배운 것**

Command + Shift + Arror = 코드 한줄 움직이기



2주차 숙제 배운점 정리
로또 생성기를 만들어 보는 수업이였습니다

이번에는 따라하는데 특별한 문제 없었고 강의를 마쳤습니다
하지만 각 항목의 기능에 대한 이해가 잘 안되어서 3주차 수업을 시작하기 전,
gitbook의 기본 문법을 공부하고 2주차 복습 후 다음 주차로 넘어갈 예정입니다

로또번호 생성을 위한 numPicker의 상/하한을 지정하고 랜덤 리스트를 생성하고,
선택한 번호 외 랜덤한 숫자를 오름차순으로 정렬해 보았습니다
각 번호의 숫자범위 별 색상을 지정하고 범위에 일치하면 순서와 무관하게 색상을 적용했습니다







