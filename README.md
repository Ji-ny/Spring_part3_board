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
https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F8473e4df-c20e-44d0-8991-9fbfc5f8af44%2FUntitled.png?table=block&id=f80615d1-a100-45cf-9c34-6a0207bdd34b&spaceId=aafcde50-e80f-48fb-92b5-14300c82804d&width=1010&userId=a49e65f5-5a01-4be6-acfb-0a85124b39dc&cache=v2
