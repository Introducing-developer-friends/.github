#  SNS

## 🎯기획 의도
명함을 주고받은 이후에 비즈니스 목적이 없으면 연락을 하지 않게 됩니다.
비즈니스 외에도 연결고리를 만들 수 있다면 비즈니스 목적 없는 좋은 만남을 만들어나갈 수 있다고 생각하여
본 서비스를 기획하였습니다.

## 🔑주요 기능

1. **회원가입 및 비즈니스 정보 수집**  
   - 회원가입 시 회사명, 직책, 연락처 등의 비즈니스 정보를 입력하여 개인 명함을 생성합니다.

2. **인맥 관리**  
   - 아이디를 통해 인맥을 추가하고, 추가된 인맥의 비즈니스 정보를 확인할 수 있습니다.
   - 인맥 리스트에서 특정 유저를 클릭하면 해당 유저의 명함 정보와 피드를 함께 볼 수 있습니다.

3. **게시물 피드**  
   - 메인 피드 페이지에서는 본인의 게시물뿐만 아니라 나와 인맥들이 작성한 모든 게시물이 표시됩니다.
   - 게시물에 좋아요를 누르거나 댓글을 작성할 수 있습니다.

4. **알림 기능**  
   - 30초마다 새로운 알림을 조회하여 게시물에 대한 좋아요, 댓글, 친구 요청 등을 확인할 수 있습니다.

5. **유저 정보 수정**  
   - 유저는 자신의 비즈니스 프로필 및 계정 정보를 수정할 수 있으며, 비밀번호 변경 기능을 제공합니다.
## 프로젝트 아키텍처
수정중!
## 💻기술 스택
- **프론트엔드**:  
  ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
  ![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
  ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
  ![Redux](https://img.shields.io/badge/Redux-764ABC?style=for-the-badge&logo=redux&logoColor=white)

- **백엔드**:  
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![TypeORM](https://img.shields.io/badge/TypeORM-FF5733?style=for-the-badge&logo=typeorm&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)
![EC2](https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=amazon-ec2&logoColor=white)
![S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)


## 🛠️개발 과정
<details>
<summary>클릭하여 작업 과정을 확인하세요</summary>
수정중!
</details>

## 역할 분담

### 강용제
- 프로젝트 기획 및 와이어프레임 설계
- 프론트엔드 개발 (React)

### 김도연
- 백엔드 개발 (NestJS, MySQL, TypeORM)
- 인프라(AWS, Docker, CloudFront, GitHub Actions)

## 📅개발 기간
- **2024년 9월 15일 ~ 11월 15일 (56일)**

## ℹ️ 사용 버전
- **React**: `v18.3.1`
- **React-Router-DOM**: `v6.26.2`
- **Redux Toolkit**: `v2.2.7`
- **TypeScript**: `v5.5.3`
- **Vite**: `v5.4.1`
- **Node.js**: `v20.15.0`
- **NestJS**: `v10.0.0`
- **MySQL**: `v8.0.39`
- **TypeORM**: `v0.3.20`

## 🗂️프로젝트 구조
<details>
<summary>프론트엔드</summary>
  
```bash
Devlntro_front/
│
│
├── src/
│   ├── api/
│   │   ├── axiosInstance.ts
│   │   └── useAuthRedirect.ts
│   │
│   ├── assets/
│   │   └── react.svg
│   │
│   ├── components/
│   │   ├── FeedDetail.tsx
│   │   ├── NavBar.tsx
│   │   ├── PasswordChange.tsx
│   │   └── ProtectedRoute.tsx
│   │
│   ├── contexts/
│   │   └── AuthContext.tsx
│   │
│   ├── pages/
│   │   ├── CreatePostPage.tsx
│   │   ├── FeedPage.tsx
│   │   ├── FriendsFeedPage.tsx
│   │   ├── FriendsPage.tsx
│   │   ├── LoginPage.tsx
│   │   ├── MyPage.tsx
│   │   └── SignUpPage.tsx
│   │
│   ├── redux/
│   │   ├── store.ts
│   │   ├── userSlice.ts
│   │   └── notificationSlice.ts
│   │
│   ├── App.css
│   ├── App.tsx
│   ├── index.css
│   └── main.tsx
│
├── .env.development
├── .env.production
├── .eslintrc.cjs
├── .gitignore
├── index.html
├── package-lock.json
├── package.json
├── README.md
├── tsconfig.json
├── tsconfig.node.json
└── vite.config.ts

```

- `src/`: 소스 코드를 포함하는 메인 디렉토리
  - `api/`: API 관련 설정 및 인스턴스
  - `assets/`: 이미지 등의 정적 자원
  - `components/`: 재사용 가능한 React 컴포넌트
  - `contexts/`: React Context API를 사용한 상태 관리
  - `pages/`: 각 페이지를 나타내는 컴포넌트
  - `redux/`: Redux 관련 파일 (스토어 설정, 슬라이스 등)
- `.env.development` 및 `.env.production`: 개발 및 프로덕션 환경 변수 설정
- `vite.config.ts`: Vite 설정 파일
- `package.json`: 프로젝트 의존성 및 스크립트 정의
</details>

<details>
<summary>백엔드</summary>


  
```bash
dev-intro_api/
│
├── .github/
├── coverage/
├── dist/
├── node_modules/
├── profile/
├── src/
│   ├── auth/
│   │   ├── dto/
│   │   │   ├── auth-login.dto.ts
│   │   │   ├── auth-register.dto.ts
│   │   │   ├── auth-refresh-token.dto.ts
│   │   ├── auth.controller.spec.ts
│   │   ├── auth.controller.ts
│   │   ├── auth.module.ts
│   │   ├── auth.service.spec.ts
│   │   ├── auth.service.ts
│   │   ├── jwt-auth.guard.spec.ts
│   │   ├── jwt-auth.guard.ts
│   │   ├── jwt.strategy.spec.ts
│   │   └── jwt.strategy.ts
│   │
│   ├── comment/
│   │   ├── dto/
│   │   │   ├── comment.dto.ts
│   │   ├── comment.controller.spec.ts
│   │   ├── comment.controller.ts
│   │   ├── comment.module.ts
│   │   ├── comment.service.spec.ts
│   │   └── comment.service.ts
│   │
│   ├── common/
│   │   ├── filters/
│   │   │   └── http-exception.filter.ts
│   │   ├── interceptors/
│   │   ├── utils/
│   │       ├── utils.helper.ts
│   │       └── validation.helper.ts
│   │
│   ├── contacts/
│   │   ├── dto/
│   │   │   ├── create-contact.dto.ts
│   │   ├── contacts.controller.spec.ts
│   │   ├── contacts.controller.ts
│   │   ├── contacts.module.ts
│   │   ├── contacts.service.spec.ts
│   │   └── contacts.service.ts
│   │
│   ├── controllers/
│   │   └── sample.controller.ts
│   ├── dto/
│   ├── entities/
│   │   ├── business-contact.entity.ts
│   │   ├── business-profile.entity.ts
│   │   ├── comment-like.entity.ts
│   │   ├── comment.entity.ts
│   │   ├── friend-request.entity.ts
│   │   ├── notification.entity.ts
│   │   ├── post-like.entity.ts
│   │   ├── post.entity.ts
│   │   ├── refresh-token.entity.ts
│   │   └── user-account.entity.ts
│   │
│   ├── feed/
│   │   ├── dto/
│   │   ├── feed.controller.spec.ts
│   │   ├── feed.controller.ts
│   │   ├── feed.module.ts
│   │   ├── feed.service.spec.ts
│   │   └── feed.service.ts
│   │
│   ├── migrations/
│   │   ├── 001-InitialMigration.ts
│   │   ├── 002-CreateFriendRequestTable.ts
│   │   ├── 003-CreateNotificationTable.ts
│   │   └── 004-CreateRefreshTokenTable.ts
│   │
│   ├── notification/
│   │   ├── dto/
│   │   ├── notifications.controller.spec.ts
│   │   ├── notifications.controller.ts
│   │   ├── notifications.module.ts
│   │   ├── notifications.service.spec.ts
│   │   └── notifications.service.ts
│   │
│   ├── post/
│   │   ├── dto/
│   │   │   ├── create-post.dto.ts
│   │   │   ├── update-post.dto.ts
│   │   │   └── like-post.dto.ts
│   │   ├── post.controller.spec.ts
│   │   ├── post.controller.ts
│   │   ├── post.module.ts
│   │   ├── post.service.spec.ts
│   │   └── post.service.ts
│   │
│   ├── s3/
│   │   ├── s3.module.ts
│   │   ├── s3.service.spec.ts
│   │   └── s3.service.ts
│   │
│   ├── seeds/
│   │   └── initial-data.seed.ts
│   │
│   ├── user/
│   │   ├── dto/
│   │   │   ├── create-user.dto.ts
│   │   ├── user.controller.spec.ts
│   │   ├── user.controller.ts
│   │   ├── user.module.ts
│   │   ├── user.service.spec.ts
│   │   └── user.service.ts
│   │
│   ├── app.controller.spec.ts
│   ├── app.controller.ts
│   ├── app.module.ts
│   ├── app.service.ts
│   ├── main.ts
│   └── ormconfig.ts
├── test/
├── .dockerignore
├── .env
├── .eslintrc.js
├── .gitignore
├── .prettierrc
├── Dockerfile
├── nest-cli.json
├── package-lock.json
├── package.json
└── README.md

```





</details>

## 📚Swagger UI
http://3.36.153.140:3000/api-docs

## 🗄️ERD 설계도
![ERD 설계도](./images/erd_diagram.png)

## 📋수동 API 명세서
<details>
<summary>API 명세서 펼치기/접기</summary>

## 1. 인증 및 사용자 관리
<details>
<summary>1.1 아이디 중복 검사</summary>

- **엔드포인트**: GET /auth/check-id/{login_id}
- **응답**:
    - 사용 **가능** (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "사용 가능한 아이디입니다."
        }
        ```
        
    - 사용 **불가** (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "이미 사용 중인 아이디입니다."
        }
        ```
</details>        

<details>
<summary>1.2 회원가입</summary>

- **엔드포인트**: POST /auth/register
- **요청 본문**:
    
    ```json
    {
      "login_id": "String",
      "password": "String",
      "confirmPassword": "String",
      "name": "String",
      "company": "String",
      "department": "String",
      "position": "String",
      "email": "String",
      "phone": "String"
    }
    ```
    
- **응답**:
    - **성공** (201 OK):
        
        ```json
        {
          "statusCode": 201,
          "message": "회원가입이 성공적으로 완료되었습니다.",
          "userId": "Number"
        }
        ```
        
    
    - **아이디 중복** (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "이미 존재하는 아이디입니다.",
          "error": "Bad Request"
        }
        ```
        
    - **비밀번호 불일치** (400 Bad Request)
    - **서버 내부 에러**
        
        ```json
        {
          "statusCode": 400,
          "message": "비밀번호와 확인 비밀번호가 일치하지 않습니다.",
          "error": "Bad Request"
        }
        ```
</details>        

<details>
<summary>1.3 로그인</summary>

- **엔드포인트**: POST /auth/login
- **요청 본문**:
    
    ```json
    {
      "login_id": "String",
      "password": "String"
    }
    
    ```
    
- **응답**:
    - 성공 (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "로그인 성공",
          "token": "JWT_TOKEN",
          "userId": "Number"
        }
        
        ```
        
    - 실패 (401 Unauthorized):
        
        ```json
        {
          "statusCode": 401,
          "message": "아이디 또는 비밀번호가 잘못되었습니다.",
          "error": "Unauthorized"
        }
        ```
</details>        

## 2. 게시물 조회 (통합 엔드포인트)

<details>
<summary>2.1 피드 조회 (메인 페이지, 내 게시물, 특정 유저 게시물 조회)</summary>

- **엔드포인트**: `GET /posts`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **쿼리 파라미터**:
    - `sort`: `"latest"`, `"likes"`, `"comments"` (정렬 기준 선택, 기본값은 `"latest"`)
    - `filter`: `"all"`, `"own"`, `"specific"` (게시물 필터링)
    - `specificUserId`: 특정 유저 게시물 조회 시 필요한 유저 ID

### **요청 예시**:

- **메인 페이지 (본인 + 인맥 게시물)**:
    
    ```sql
    GET /posts?filter=all&sort=latest
    ```
    
- **내 게시물 조회 (마이 게시물)**:
    
    ```bash
    GET /posts?filter=own&sort=latest
    ```
    
- **특정 유저 페이지 (특정 유저 게시물)**:
    
    ```sql
    GET /posts?filter=specific&specificUserId=123&sort=comments
    ```
    

### **응답 예시**:

### 성공 (200 OK):

```json
{
  "statusCode": 200,
  "message": "피드를 성공적으로 조회했습니다.",
  "posts": [
    {
      "postId": 123,
      "createrId": 456,
      "createrName": "홍길동",
      "createdAt": "2024-09-18T12:34:56.000Z",
      "imageUrl": "https://example.com/image.jpg",
      "isOwnPost": true},
    {
      "postId": 124,
      "createrId": 789,
      "createrName": "김철수",
      "createdAt": "2024-09-18T13:00:00.000Z",
      "imageUrl": "https://example.com/image2.jpg",
      "isOwnPost": false}
  ]
}
```

### 잘못된 파라미터 (400 Bad Request):

```json
{
  "statusCode": 400,
  "message": "잘못된 요청입니다. specificUserId가 필요합니다.",
  "error": "Bad Request"
}
```

### 게시물 없음 (404 Not Found):

```json
{
  "statusCode": 404,
  "message": "해당 게시물을 찾을 수 없습니다.",
  "error": "Not Found"
}
```

---
</details>

<details>
<summary>2.2 게시물 상세 조회</summary>

- **엔드포인트**: `GET /posts/{postId}`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`

### **응답 예시**:

### 성공 (200 OK):

```json
{
  "statusCode": 200,
  "message": "게시물을 성공적으로 조회했습니다.",
  "postId": 123,
  "createrId": 456,
  "createrName": "홍길동",
  "createdAt": "2024-09-18T12:34:56.000Z",
  "imageUrl": "https://example.com/image.jpg",
  "content": "이 게시물의 내용입니다.",
  "likesCount": 42,
  "commentsCount": 10,
  "isOwnPost": true,
  "comments": [
    {
      "commentId": 1,
      "authorName": "김철수",
      "content": "멋진 게시물이네요!",
      "createdAt": "2024-09-18T12:45:00.000Z"
    },
    {
      "commentId": 2,
      "authorName": "이영희",
      "content": "좋은 글 감사합니다.",
      "createdAt": "2024-09-18T13:00:00.000Z"
      "likeCount": "2"
    }
  ],
  "likes": [
    {
      "userId": 789,
      "userName": "김철수"
    },
    {
      "userId": 890,
      "userName": "이영희"
    }
  ]
}
```

### 유효하지 않은 게시물 ID (400 Bad Request):

```json
{
  "statusCode": 400,
  "message": "유효하지 않은 게시물 ID입니다.",
  "error": "Bad Request"
}
```

### 게시물 없음 (404 Not Found):

```json
{
  "statusCode": 404,
  "message": "해당 게시물을 찾을 수 없습니다.",
  "error": "Not Found"
}
```
</details>

## 3. 게시물 관리

<details>
<summary>3.1 게시물 작성</summary>

- **엔드포인트**: POST /posts
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **요청 본문**:
    - **Form Data**:
        - `content`: String (필수) - 게시물 내용
        - `image`: File (선택) - 업로드할 이미지 파일
- **응답**:
    - **성공** (201 Created):
        
        ```json
        {
          "statusCode": 201,
          "message": "게시물이 성공적으로 작성되었습니다.",
          "postId": "Number"
        }
        ```
        
    - **실패** (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "게시물 작성에 실패했습니다. 필수 필드를 확인해주세요.",
          "error": "Bad Request"
        }
        ```
</details>        

<details>
<summary>3.2 게시물 수정</summary>

- **엔드포인트**: PUT /posts/{postId}
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **요청 본문**:
    - **Form Data**:
        - `content`: String (선택) - 게시물 내용
        - `image`: File (선택) - 새로 업로드할 이미지 파일
- **응답**:
    - **성공** (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "게시물이 성공적으로 수정되었습니다."
        }
        ```
        
    - **실패** (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "게시물 수정에 실패했습니다. 유효한 데이터를 입력해주세요.",
          "error": "Bad Request"
        }
        ```
        
    - **실패** (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "게시물을 찾을 수 없습니다.",
          "error": "Not Found"
        }
        
        ```
</details>        

<details>
<summary>3.3 게시물 삭제</summary>

- **엔드포인트**: DELETE /posts/{postId}
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **응답**:
    - **성공** (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "게시물이 성공적으로 삭제되었습니다."
        }
        ```
        
    - **실패** (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "게시물을 찾을 수 없습니다.",
          "error": "Not Found"
        }
        ```
</details>        

<details>
<summary>3.4 게시물 좋아요</summary>

- **엔드포인트**: POST /posts/{postId}/like
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **응답**:
    - **성공** (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "게시물에 좋아요를 눌렀습니다.",
          "likeCount": "Number"
        }
        ```
        
    - **성공** (200 OK) - 좋아요 취소:
        
        ```json
        {
          "statusCode": 200,
          "message": "게시물 좋아요를 취소했습니다.",
          "likeCount": "Number"
        }
        ```
        
    - **실패** (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "게시물을 찾을 수 없습니다.",
          "error": "Not Found"
        }
        ```
 </details>       

## 4. 댓글관리

<details>
<summary>댓글 작성</summary>

- **엔드포인트**: POST /posts/{postId}/comments
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **요청 본문**:
    
    ```json
    {
      "content": "String"
    }
    ```
    
- **응답**:
    - **성공** (201 Created):
        
        ```json
        {
          "statusCode": 201,
          "message": "댓글이 성공적으로 작성되었습니다.",
          "commentId": "Number"
        }
        ```
        
    - **실패** (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "댓글 작성에 실패했습니다. 내용을 입력해주세요.",
          "error": "Bad Request"
        }
        ```
</details>        

<details>
<summary>댓글 수정</summary>

- **엔드포인트**: PUT /posts/{postId}/comments/{commentId}
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **요청 본문**:
    
    ```json
    {
      "content": "String"
    }
    ```
    

**응답**

- **성공** (200 OK):
    
    ```json
    {
      "statusCode": 200,
      "message": "댓글이 성공적으로 수정되었습니다."
    }
    ```
    
- **실패** (400 Bad Request):
    
    ```json
    {
      "statusCode": 400,
      "message": "댓글 수정에 실패했습니다. 유효한 내용을 입력해주세요.",
      "error": "Bad Request"
    }
    ```
    
- **실패** (404 Not Found):
    
    ```json
    {
      "statusCode": 404,
      "message": "댓글을 찾을 수 없습니다.",
      "error": "Not Found"
    }
    ```
</details>     

<details>
<summary>댓글 삭제</summary>

- **엔드포인트**: DELETE /posts/{postId}/comments/{commentId}
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **응답**:
    - **성공** (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "댓글이 성공적으로 삭제되었습니다."
        }
        ```
        
    - **실패** (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "댓글을 찾을 수 없습니다.",
          "error": "Not Found"
        }
        ```
</details>

<details>
<summary>댓글 좋아요</summary>

- **엔드포인트**: POST /posts/{postId}/comments/{commentId}/like
- **헤더**: Authorization: Bearer {JWT_TOKEN}
- **응답**:
    - **성공** (200 OK) - 좋아요 추가:
        
        ```json
        {
          "statusCode": 200,
          "message": "댓글에 좋아요를 눌렀습니다.",
          "likeCount": "Number"
        }
        ```
        
    - **성공** (200 OK) - 좋아요 취소:
        
        ```json
        {
          "statusCode": 200,
          "message": "댓글 좋아요를 취소했습니다.",
          "likeCount": "Number"
        }
        ```
        
    - **실패** (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "댓글을 찾을 수 없습니다.",
          "error": "Not Found"
        }

        ```
</details>        

## 5. 명함 관리

<details>
<summary>5.1 명함 리스트 조회</summary>

- **엔드포인트**: GET /contacts
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - 성공 (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "명함 리스트를 성공적으로 조회했습니다.",
          "contacts": [
            {
              "userId": "Number",
              "name": "String",
              "company": "String",
              "department": "String"
            }
          ]
        }
        ```
        
    - 실패 (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "잘못된 요청입니다.",
          "error": "Bad Request"
        }
        ```
        
    - 실패 (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "명함 리스트를 찾을 수 없습니다.",
          "error": "Not Found"
        }
        ```
</details>        

<details>
<summary>5.2 명함 상세 정보 조회</summary>

- **엔드포인트**: GET /contacts/{userId}
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - 성공 (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "명함 상세 정보를 성공적으로 조회했습니다.",
          "contact": {
            "userId": "Number",
            "name": "String",
            "company": "String",
            "department": "String",
            "position": "String",
            "email": "String",
            "phone": "String"
          }
        }
        ```
        
    - 실패 (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "유효하지 않은 사용자 ID입니다.",
          "error": "Bad Request"
        }
        ```
        
    - 실패 (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "해당 사용자의 명함을 찾을 수 없습니다.",
          "error": "Not Found"
        }
        ```
</details>        

<details>
<summary>5.3 인맥 추가 (명함 추가)</summary>

- **엔드포인트**: POST /contacts
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "loginId": "Number"
    }
    ```
    
- **응답**:
    - 성공 (201 Created):
        
        ```json
        {
          "statusCode": 201,
          "message": "인맥이 요청이 성공적으로 추가되었습니다.",
          "contactId": "Number"
        }
        ```
        
    - 실패 (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "대상 사용자를 찾을 수 없습니다.",
          "error": "Bad Request"
        }
        ```
        
    - 실패 (409 Conflict):
        
        ```json
        {
          "statusCode": 409,
          "message": "이미 인맥 요청을 보냈거나 인맥 관계가 존재합니다.",
          "error": "Conflict"
        }
        ```
 </details>        

<details>
<summary>5.4 인맥 요청 수락</summary>

- **엔드포인트**: POST /contacts/accept/{requestId}
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - 성공 (200 OK):

```json
{
  "statusCode": 200,
  "message": "인맥 요청이 수락되었습니다.",
  "contactId": "Number"// 새로 생성된 인맥 관계의 ID
}
```

- 실패 (400 Bad Request):

```json
{
  "statusCode": 400,
  "message": "유효하지 않은 요청입니다.",
  "error": "Bad Request"
}
```

- 실패 (404 Not Found):

```json
{
  "statusCode": 404,
  "message": "해당 인맥 요청을 찾을 수 없습니다.",
  "error": "Not Found"
}
```
</details>

<details>
<summary>5.5 인맥 요청 거절</summary>

- **엔드포인트**: POST /contacts/reject/{requestId}
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - 성공 (200 OK):

```json
{
  "statusCode": 200,
  "message": "인맥 요청이 거절되었습니다."
}
```

- 실패 (400 Bad Request):

```json
{
  "statusCode": 400,
  "message": "유효하지 않은 요청입니다.",
  "error": "Bad Request"
}
```

- 실패 (404 Not Found):

```json
{
  "statusCode": 404,
  "message": "해당 인맥 요청을 찾을 수 없습니다.",
  "error": "Not Found"
}
```
</details>

<details>
<summary>5.6 받은 인맥 요청 목록 조회</summary>

- **엔드포인트**: GET /contacts/requests/received
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - 성공 (200 OK):

```json
{
  "statusCode": 200,
  "message": "받은 인맥 요청 목록을 성공적으로 조회했습니다.",
  "requests": [
    {
      "requestId": "Number",
      "senderLoginId": "String",
      "senderName": "String",
      "requestedAt": "DateTime"
    }
  ]
}
```

- 실패 (400 Bad Request):

```json
{
  "statusCode": 400,
  "message": "요청 처리 중 오류가 발생했습니다.",
  "error": "Bad Request"
}
```
</details>

<details>
<summary>5.7 보낸 인맥 요청 목록 조회</summary>

- **엔드포인트**: GET /contacts/requests/sent
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - 성공 (200 OK):

```json
{
  "statusCode": 200,
  "message": "보낸 인맥 요청 목록을 성공적으로 조회했습니다.",
  "requests": [
    {
      "requestId": "Number",
      "senderLoginId": "String",
      "senderName": "String",
      "requestedAt": "DateTime"
    }
  ]
}
```

- 실패 (400 Bad Request):

```json
{
  "statusCode": 400,
  "message": "요청 처리 중 오류가 발생했습니다.",
  "error": "Bad Request"
}
```
</details>

<details>
<summary>5.8 인맥 삭제 (명함 삭제)</summary>

- **엔드포인트**: DELETE /contacts/{contactId}
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - 성공 (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "인맥이 성공적으로 삭제되었습니다."
        }
        ```
        
    - 실패 (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "유효하지 않은 인맥 ID입니다.",
          "error": "Bad Request"
        }
        ```
        
    - 실패 (404 Not Found):
        
        ```json
        {
          "statusCode": 404,
          "message": "해당 인맥을 찾을 수 없습니다.",
          "error": "Not Found"
        }
        ```
</details>        

## 6. 사용자 정보 관리

<details>
<summary>6.1 나의 명함 정보 수정</summary>
  
- **엔드포인트**: PUT /users/businessprofile
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "name": "String",
      "company": "String",
      "department": "String",
      "position": "String",
      "email": "String",
      "phone": "String"
    }
    ```
    
- **응답**:
    - 성공 (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "프로필 정보가 성공적으로 수정되었습니다."
        }
        ```
        
    - 실패 (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "잘못된 요청입니다. 유효한 정보를 입력해주세요.",
          "error": "Bad Request"
        }
        ```
</details>         

<details>
<summary>6.2 비밀번호 변경 </summary>

- **엔드포인트**: PUT /users/password
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "currentPassword": "String",
      "newPassword": "String",
      "confirmNewPassword": "String"
    }
    ```
    
- **응답**:
    - 성공 (200 OK):
        
        ```json
        {
          "statusCode": 200,
          "message": "비밀번호가 성공적으로 변경되었습니다."
        }
        ```
        
    - 실패 (400 Bad Request):
        
        ```json
        {
          "statusCode": 400,
          "message": "새 비밀번호와 확인 비밀번호가 일치하지 않습니다.",
          "error": "Bad Request"
        }
        ```
        
    - 실패 (401 Unauthorized):
        
        ```json
        {
          "statusCode": 401,
          "message": "현재 비밀번호가 올바르지 않습니다.",
          "error": "Unauthorized"
        }
        ```
</details>        

<details>
<summary>6.3 회원 탈퇴</summary>

- **엔드포인트**: DELETE /users
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:

```json
{
  "password": "String"
}
```

- **응답**:
    - 성공 (200 OK):

```json
{
  "statusCode": 200,
  "message": "회원 탈퇴가 성공적으로 처리되었습니다."
}
```

- 실패 (400 Bad Request):

```json
{
  "statusCode": 400,
  "message": "회원 탈퇴 처리 중 오류가 발생했습니다.",
  "error": "Bad Request"
}
```

- 실패 (401 Unauthorized):

```json
{
  "statusCode": 401,
  "message": "비밀번호가 올바르지 않습니다.",
  "error": "Unauthorized"
}
```
</details>

## 7. 알림 관리

<details>
<summary>7.1 알림 목록 조회</summary>

### 엔드포인트: `GET /notifications`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - **성공** (200 OK):
    
    ```json
    {
      "statusCode": 200,
      "message": "알림 목록을 성공적으로 조회했습니다.",
      "notifications": [
        {
          "notificationId": 1,
          "type": "friend_request",
          "message": "홍길동님이 친구 요청을 보냈습니다.",
          "postId": null,
          "commentId": null,
          "isRead": false,
          "createdAt": "2024-10-03T12:34:56Z",
          "senderId": 99
        }
      ]
    }
    ```
    
    - **실패** (400 Bad Request):
    
    ```json
    {
      "statusCode": 400,
      "message": "알림 조회 중 오류가 발생했습니다.",
      "error": "Bad Request"
    }
    ```

</details>

<details>
<summary>7.2 알림 읽음 처리</summary>

### 엔드포인트: `PATCH /notifications/{notificationId}/read`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **응답**:
    - **성공** (200 OK):
    
    ```json
    {
      "statusCode": 200,
      "message": "알림이 성공적으로 읽음 처리되었습니다."
    }
    ```
    
    - **실패** (404 Not Found):
    
    ```json
    {
      "statusCode": 404,
      "message": "해당 알림을 찾을 수 없습니다.",
      "error": "Not Found"
    }
    ```

</details>

<details>
<summary>7.3 친구 요청 알림 생성</summary>

### 엔드포인트: `POST /notifications/friend-request`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "receiverId": 99,
      "message": "홍길동님이 친구 요청을 보냈습니다."
    }
    ```
    
- **응답**:
    - **성공** (201 Created):
    
    ```json
    {
      "statusCode": 201,
      "message": "친구 요청 알림이 성공적으로 생성되었습니다.",
      "notificationId": 1
    }
    ```
    
    - **실패** (400 Bad Request):
    
    ```json
    {
      "statusCode": 400,
      "message": "친구 요청 알림 생성 중 오류가 발생했습니다.",
      "error": "Bad Request"
    }
    ```

</details>

<details>
<summary>7.4 게시물 좋아요 알림 생성</summary>

### 엔드포인트: `POST /notifications/like-post`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "postId": 123,
      "receiverId": 456,
      "message": "김철수님이 당신의 게시물에 좋아요를 눌렀습니다."
    }
    ```
    
- **응답**:
    - **성공** (201 Created):
    
    ```json
    {
      "statusCode": 201,
      "message": "게시물 좋아요 알림이 성공적으로 생성되었습니다.",
      "notificationId": 2
    }
    ```
    
    - **실패** (400 Bad Request):
    
    ```json
    {
      "statusCode": 400,
      "message": "게시물 좋아요 알림 생성 중 오류가 발생했습니다.",
      "error": "Bad Request"
    }
    ```

</details>

<details>
<summary>7.5 댓글 알림 생성</summary>

### 엔드포인트: `POST /notifications/comment`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "postId": 123,
      "receiverId": 456,
      "message": "이영희님이 당신의 게시물에 댓글을 남겼습니다."
    }
    ```
    
- **응답**:
    - **성공** (201 Created):
    
    ```json
    {
      "statusCode": 201,
      "message": "댓글 알림이 성공적으로 생성되었습니다.",
      "notificationId": 3
    }
    ```
    
    - **실패** (400 Bad Request):
    
    ```json
    {
      "statusCode": 400,
      "message": "댓글 알림 생성 중 오류가 발생했습니다.",
      "error": "Bad Request"
    }
    ```

</details>

<details>
<summary>7.6 댓글 좋아요 알림 생성</summary>

### 엔드포인트: `POST /notifications/like-comment`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "commentId": 789,
      "receiverId": 456,
      "message": "김철수님이 당신의 댓글에 좋아요를 눌렀습니다."
    }
    ```
    
- **응답**:
    - **성공** (201 Created):
    
    ```json
    {
      "statusCode": 201,
      "message": "댓글 좋아요 알림이 성공적으로 생성되었습니다.",
      "notificationId": 4
    }
    ```
    
    - **실패** (400 Bad Request):
    
    ```json
    {
      "statusCode": 400,
      "message": "댓글 좋아요 알림 생성 중 오류가 발생했습니다.",
      "error": "Bad Request"
    }
    ```

</details>

<details>
<summary>7.7 알림 삭제</summary>

### 엔드포인트: `DELETE /notifications/{notificationId}`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **설명**: 사용자가 특정 알림을 삭제합니다.
- **응답**:
    - **성공** (200 OK):
    
    ```json
    {
      "statusCode": 200,
      "message": "알림이 성공적으로 삭제되었습니다."
    }
    ```

    - **실패** (404 Not Found):
    
    ```json
    {
      "statusCode": 404,
      "message": "해당 알림을 찾을 수 없습니다.",
      "error": "Not Found"
    }
    ```
    - **실패** (400 Bad Request):

    ```json
    {
      "statusCode": 400,
      "message": "알림 삭제 중 오류가 발생했습니다.",
      "error": "Bad Request"
    }
    ```

</details>

<details>
<summary>7.8 알림 일괄 삭제</summary>

### 엔드포인트: `DELETE /notifications`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **설명**: 사용자가 다수의 알림을 한 번에 삭제합니다.
- **요청 본문**:
    
    ```json
    {
      "notificationIds": [1, 2, 3]
    }
    ```
    
- **응답**:
    - **성공** (200 OK):
    
    ```json
    {
      "statusCode": 200,
      "message": "선택한 알림들이 성공적으로 삭제되었습니다."
    }
    ```
    
    - **실패** (400 Bad Request):
    
    ```json
    {
      "statusCode": 400,
      "message": "알림 삭제 요청 중 오류가 발생했습니다.",
      "error": "Bad Request"
    }
    ```
    - **실패** (404 Not Found):

    ```json
    {
      "statusCode": 404,
      "message": "삭제할 알림을 찾을 수 없습니다.",
      "error": "Not Found"
    }
    ```

</details>

<details>
<summary>7.9 로그인 ID로 사용자 ID 조회</summary>

### 엔드포인트: `POST /notifications/find-user-id`
- **헤더**: `Authorization: Bearer {JWT_TOKEN}`
- **요청 본문**:
    
    ```json
    {
      "login_id": "test_login"
    }
    ```
    
- **응답**:
    - **성공** (200 OK):
    
    ```json
    {
      "statusCode": 200,
      "message": "사용자 ID를 성공적으로 조회했습니다.",
      "userId": 123
    }
    ```
    
    - **실패** (404 Not Found):
    
    ```json
    {
      "statusCode": 404,
      "message": "해당 로그인 ID에 해당하는 사용자를 찾을 수 없습니다.",
      "error": "Not Found"
    }
    ```

</details>





</details>


