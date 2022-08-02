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
