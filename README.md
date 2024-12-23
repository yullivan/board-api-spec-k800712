# 게시판 API

## 기능
- 게시글 작성,조회,수정,삭제
- 게시글 이미지, 파일 업로드
- 댓글 작성, 조회, 수정, 삭제
- 사용자 인증, 권한 관리

## 기술스택
- Node.js
- Express.js
- MongoDB
- JWT for authentication


## API 엔드포인트

### 게시글

- `GET /api/posts`: 모든 게시글 조회
- `GET /api/posts/:id`: 특정 게시글 조회
- `POST /api/posts`: 새 게시글 작성
- `PUT /api/posts/:id`: 게시글 수정
- `DELETE /api/posts/:id`: 게시글 삭제
- `POST /api/upload` : 이미지 등 파일 업로드
- `POST /api/posts/:id/report`: 게시글 신고

### 댓글

- `GET /api/posts/:postId/comments`: 특정 게시글의 모든 댓글 조회
- `POST /api/posts/:postId/comments`: 새 댓글 작성
- `PUT /api/comments/:id`: 댓글 수정
- `DELETE /api/comments/:id`: 댓글 삭제
- `POST /api/comments/:id/report`: 댓글 신고
### 인증

- `POST /api/auth/register`: 새 사용자 등록
- `POST /api/auth/login`: 로그인



