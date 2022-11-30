# 플러터 바로바로 메모용

1. 텍스트필드의 변화를 핸들링하려면 TextEditingController()객체를 생성해줘야 함\
   ([https://here4you.tistory.com/129)](https://here4you.tistory.com/129)
2. ReorderableListView로 순서 바꾸기가 가능한 LIst를 간편하게 만들 수 있음\
   \- onReorder로 순서 바꾸기 구현\
   \- children 하위에 배열.map(배열 각 요소에 붙여줄 명칭) => Listtile(key:key(map에붙여준명칭)).t  oList()로 구현
