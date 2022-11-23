# Provider 정리하기

{% embed url="https://kimiszero.tistory.com/92" %}

(추후 가독성 좋게 다시 정리하기)

1. yaml에 provider 디펜던시 추가
2. main.dart의 머테리얼 앱의 home에 ChangeNotifierProvider 추가(뷰는 child에 새로 연결시켜주면 됨)
3. Provider 클래스 정의해줄 dart파일 새로 생성
4. 만든 dart파일의 class에 ChangeNotifier 상속
5. get 선언해서 다른 위젯에서 읽을 수 있게 해주기
6. main.dart의 ChangeNotifierProvider - create에 생성한 Provider 클래스를 리턴
7. main.dart 외의 파일에서 Provider 사용 시에는  state 상단에  \
   '`late [클래스명] [변수명]' 선언`
8. 오버라이드 된 빌드 대괄호 안에 아래와 같은 형식으로 사용\
   \_todosProvider = Provider.of(context);
9. 이제 선언된 변수로 해당 화면에서 마음대로 호출 가능



* ```
  late는 null이면 초기화 시점을 뒤로 미루는 변수
  ```
* ```
  notifyListeners() 사용하면 연관 위젯들 한 번에 리빌딩 해줌
  ```
