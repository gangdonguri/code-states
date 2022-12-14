## 메소드

### 조회 (GET)
- 블로그 글 목록 조회 GET http://localhost:1337/api/posts
- 특정 블로그 글 조회 GET http://localhost:1337/api/posts/1
- 모든 댓글 조회 GET http://localhost:1337/api/comments
- 특정 댓글 조회 GET http://localhost:1337/api/comments/1
- 특정 블로그 글에 달린 댓글 조회 GET 

### 생성 (POST)
- 새 블로그 글 생성 POST http://localhost:1337/api/posts
{
  "data": {
    "title": "HTTP 기초",
    "description": "HTTP 기초에 대해 알아보자.",
    "categorie": "HTTP",
    "like": 0
    "user": [
      {
        "id": 1
      }
    ]
  } 
}
- 새 댓글 생성
- 블로그 글 좋아요
- 다른 글쓴이 팔로우

### 삭제 (DELETE)
- 특정 블로그 글 삭제 DELETE http://localhost:1337/api/posts/1
- 특정 댓글 삭제 DELETE http://localhost:1337/api/comments/1
- 블로그 글 좋아요 취소

### 수정 (PUT)
- 특정 블로그 글 수정 
- 특정 댓글 수정

## 리소스

### post
- title
- description
- categorie
- createdAt
- updatedAt
- like
- user
- comments

### user
- username
- email
- provider
- password
- resetPasswordToken
- confirmationToken
- confirmed
- blocked
- role
- follwer
- following
- comments
- posts

### comment
- user
- post
- comment