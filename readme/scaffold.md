---
description: 여유될 때 소분류 정리하기
---

# Scaffold 및 기타 레이아웃 정리

### **Scaffold()를 이용한 화면 인터페이스 제작**

| **appBar**                       | 화면 상단에  탭 바를 만들어줌              |
| -------------------------------- | ------------------------------ |
| **body**                         | 상단 바와 하단 바 사이에 메인 내용이 들어가는 영역  |
| **bottomNavigationBar**          | 화면 하단에 탭 바를 만들어줌               |
| **floatingActionButton**         | 화면 공중에 위치하는 버튼을 만들어줌           |
| **floatingActionButtonLocation** | 'FloatingActionButton'의 위치를 조정 |
| **toolbarHeight**                | 'appBar'의 높이를 지정해줌             |

### **Scaffold()의 drawer 기능**

| **drawer**                      | 앱바의 좌측에 자동으로 메뉴 위젯을 추가하고, 클릭 또는 화면을 드래그하여 메뉴를 꺼낼 수 있음 |
| ------------------------------- | ----------------------------------------------------- |
| **endDrawer**                   | 'drawer'와 기능은 동일하나, 위젯을 앱바의 우측에 추가함                   |
| **drawerEdgeDragWidth**         | 드래그로 메뉴를 꺼낼 때, 터치를 인식하는 너비를 지정해줌                      |
| **drawerEnableOpenDragGesture** | 드래그로 메뉴를 꺼내는 기능을 켜고 끌 수 있음                            |
| **drawerScrimColor**            | 메뉴가 나와있을 때 여백 공간의 색상을 지정                              |

※ drawer 관련 위젯은 AppBar()의 괄호가 아닌, Scaffold()의 괄호에 입력해야 함

### **AbbBar()의 기능**

| **title**           | 앱바의 중간에 들어갈 요소를 입력할 수 있음 |
| ------------------- | ------------------------ |
| **centertitle**     | 'title'속성을 가운데 정렬시킬 수 있음 |
| **leading**         | 앱바의 좌측에 위젯을 추가시킬 수 있음    |
| **actions**         | 앱바의 우측에 위젯을 추가시킬 수 있음    |
| **backgroundColor** | 앱바의 배경색을 변경할 수 있음        |
| **elevation**       | 앱바의 그림자 정도를 지정할 수 있음     |

### **bottomNavigationBar의 하위 위젯들**

| **Tabbar()**              | <p>tabs[]의 배열 안에 tab()위젯을 이용하여 각각의 탭을 생성해줌.<br>탭 화면의 내용은 Body 안에 TabBarView()의 children[] 배열안에 담아줘야 함.</p>                                                  |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **BottomNavigationBar()** | <p>각각의 탭에 currentIndex라는 속성으로 인덱스가 부여됨.<br>하지만, 값만 부여되고 클릭 시에 인덱스의 변경은 onTap을 이용하여 직접 구현해줘야 함<br>그 후, 화면을 담은 리스트에 배열의 인덱스 값으로 currentIndex 값을 넘겨 화면을 전환</p> |

### **레이아웃 위젯 ( 하나의 자식 요소만 가능 )**

| **Container()** | 크기의 기본 값을 최대 크기(부모 요소의 크기)로 가지는 레이아웃 위젯             |
| --------------- | --------------------------------------------------- |
| **SizedBox()**  | 크기의 기본 값을 자식 요소의 크기로 가지는 레이아웃 위젯, Container()보다 가벼움 |

### **레이아웃 위젯 ( 다수의 자식 요소 가능 )**

| **Row()**    | Children 속성의 배열 속 요소들을 가로로 정렬시켜 보여줌 |
| ------------ | ----------------------------------- |
| **Column()** | Children 속성의 배열 속 요소들을 세로로 정렬시켜 보여줌 |
