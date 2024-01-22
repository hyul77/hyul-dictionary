# 1. Singly Linked List

Fig. 1 Singly Linked List 예시
 

Singly Linked List 인 경우 Data와 주소값을 가지는 Node들이 연결된 것을 뜻한다.

head라는 노드에서부터 시작해 data1 노드 -> data2 노드 -> data3 노드 -> .... -> tail 로 이동하는 것을 뜻한다.

 

탐색, 삽입, 삭제를 생각하자면

탐색인 경우 Data3의 값을 찾기 위해선 head -> Data1 -> Data2 -> Data3 이렇게 순서대로 찾아야한다.

즉, 최악의 경우 n개의 data가 있으면 O(n)의 탐색 시간이 걸린다.

 

탐색에서 그렇다면 중간에 삽입하는 거 또한 O(n), 찾아서 삭제하는 거 또한 O(n)이 된다.

물론 head 또는 tail 부분에 추가하는 것은 O(1) time 이므로 vector 처럼 앞에 추가하는 것 부분에서 활용도가 좋다.

 

# 2. Doubly Linked List


Fig. 2 Doubly Linked List

미리 그림을 설명하자면 화살표 가 겉이 아닌 양 사이드의 사각형 중앙에 존재 해야 옳은 그림이다.

 

해당 Doubly Linked List 경우 노드 가운데에 data를 저장하고 left, right와 같이 좌우 노드들의 주소 값을 저장한다.

Singly LInked List는 오른쪽의 값들만 탐색할 수 있는 거와 달리 Doubly Linked List는 좌우 이동이 편하다.

이러한 이점을 제외 한다면, 탐색, 삽입, 삭제의 경우 Singly Linked List와 동일한 시간이 걸린다.