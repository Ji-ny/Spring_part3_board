# Spring_part3_board
## [board]


### [api규격서]

| 방식 | 호출 대상 | 파라미터 | 작업 | 반환되는 데이터 |
| --- | --- | --- | --- | --- |
| GET | /replies/board/{bno} (게시물 번호) | 게시물 번호 | 해당 게시물의 댓글들 조회 | JSON 배열 |
| POST | /replies/ | JSON으로 구성된 댓글 데이터 | 댓글 추가 | 추가된 댓글의 번호 |
| DELETE | /replies/{rno} | 댓글 번호 | 댓글 삭제 | 삭제 결과 문자열 |
| PUT | /replies/{rno} | 댓글번호 + 수정할내용 | 댓글 수정 | 수정 결과 문자열 |






### [엔티티관계도]

![image](https://user-images.githubusercontent.com/96537605/182355268-dd634309-de74-46b7-9c1e-f49f32fecf55.png)



---
## [설명]

### 6.3.1 댓글 조회 기능의 분리

- 댓글이 추가되거나 삭제되면 화면의 갱신이 필요하다.
- 별도의 함수로 제작해서, 사용하도록 분리한다.
    

![image](https://user-images.githubusercontent.com/96537605/182356386-8467cb65-431d-41e6-8825-2b398b5d71d6.png)

- Reply Count를 클릭하면, 댓글이 출력되는 것을 알 수 있다.

### 6.3.2 댓글 추가와 모달창

1. add Reply 버튼을 누른다.
![image](https://user-images.githubusercontent.com/96537605/182356416-6c33f5b8-5bc8-4386-843f-6c49a7272bc8.png)

2. 댓글의 내용과, 댓글 다는 사람의 이름을 적고 save한다.

![image](https://user-images.githubusercontent.com/96537605/182356461-739e8552-9f92-4c45-b0a9-272d9a1a3547.png)

3. 결과 확인 - 댓글이 추가됐다.

![image](https://user-images.githubusercontent.com/96537605/182356552-6f9dace5-a9ae-4677-887f-61ebf38571ca.png)

### 6.3.3 댓글 삭제 처리

1. 댓글 클릭

![image](https://user-images.githubusercontent.com/96537605/182356631-b3b69140-8989-4c70-8476-397ab2f9f765.png)

2. remove 버튼을 누르면, 댓글이 삭제된다.

![image](https://user-images.githubusercontent.com/96537605/182356714-adc94a3d-a40d-40f8-b27f-534541eaf2ea.png)


### 6.3.4 댓글수정 처리

1. 댓글 클릭

![image](https://user-images.githubusercontent.com/96537605/182356756-887fe2a1-a3ba-49a8-bf07-a1e9955f7905.png)


2. 수정할 것을 입력하고 Modify 버튼을 누르면, 댓글이 수정된다.
![image](https://user-images.githubusercontent.com/96537605/182356819-0a5a8cc6-6e60-45bf-a90d-889a4e92c892.png)
![image](https://user-images.githubusercontent.com/96537605/182356835-6e877146-4e3c-4a66-950f-b9236fb1fa94.png)

3. 결과 확인
![image](https://user-images.githubusercontent.com/96537605/182356876-d02ed9ae-a410-46c1-b86c-cd9dcce1cacb.png)
