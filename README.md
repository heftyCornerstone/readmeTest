# 살까말까

# 요구사항
## 필수기능

**데이터베이스**
- [x] Supabase를 활용한 CRUD
- [x] Supabase를 활용한 로그인, 회원 가입
**유저 로그인 정보 관리**
- [ ] onAuthStateChanged를 적극 활용하여 인증된 유저의 상태 변경 추적
- [x]  Context API를 활용한(혹은 다른 전역상태 툴을 이용한) 전역상태 관리
**라우팅**
- [x]  RRD(React Router DOM)
 **마이 페이지에서...**
- [x] 내 게시물 보기
- [x] 프로필 수정 기능
**배포**
- [x] 호스팅플랫폼 Vercel 이용, 배포에 적용될 브랜치는 main 브랜치로

## 도전기능
- [ ] 로그인, 회원가입 예외 처리
- [ ] 소셜 로그인 (구글, 깃헙)
- [ ] 비밀번호 찾기 기능
- [ ] 팔로우, 팔로워 기능
- [ ] 팔로우한 상대 게시물 확인 기능
- [x] 댓글 기능
- [x] 좋아요, 북마크 기능
- [x] 반응형 웹 구현
- [ ] 무한스크롤 기능
- [ ] 더보기 기능
- [ ] memo, useMemo, useCallback을 이용한 렌더링 최적화 적용
- [ ] Vercel 에 배포한 뒤 커스텀 도메인 적용 (500원 정도하는 저렴한 도메인 권장)

## 기능 구현

#### 필수 요구사항 구현에 관한 특이사항
* 내 게시물 보기 기능은 마이페이지가 아닌 `내 포스트` 페이지로 구현
* 전역상태관리를 위해 RTK를 사용

#### 로그인 정보 유지
* 새로고침하거나 브라우저를 닫아도 로그인 정보를 유지하기 위해 redux-persist 사용
#### alret 처리 ([**React-Toastify**](https://fkhadra.github.io/react-toastify/introduction/))
- React-Toastify로 사용자 친화적인 성공 또는 에러 메세지를 보여줌
#### react-hook-form
- react-hook-form을 사용하여, 폼 상태를 효율적으로 관리하고, 유효성 검사(validation)를 진행

# 프로젝트 개요


# 프로젝트명 : 살까말까

웹사이트 살까말까 소개...

# 페이지 구성


<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/a0d06574-99a8-401e-8a52-327f05ccfd46/image.png' width='50%'></p>

# 페이지별 레이아웃과 기능

## 비로그인

### 레이아웃
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/562dcae1-e5c3-46b6-a5c0-b66450b5509e/image.png' width='60%'></p>

### 로그인 / 회원 가입
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/9c5a699d-c8bc-41ff-9a17-76a477f933db/image.png' width='40%'></p>
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/91089aec-2c64-4f9f-ba17-7a2b27e5987a/image.png' width='50%'></p>


## 로그인 성공
### 레이아웃
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/2c668f06-8779-4f1f-b8a6-c37c0ffc827c/image.png' width='60%'></p>

### 홈
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/63de1518-39b3-464b-8c31-afd481192e94/image.png' width='60%'></p>

- 게시글 접근 가능
- 내비게이션 바를 이용해 다른 페이지로 접근 가능

### 게시글 상세
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/4cf3aad1-39e7-4172-9556-cc63607420f8/image.gif' width='60%'></p>

#### 게시글 수정
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/db63c66c-ede2-4d89-9897-83c840625f3c/image.gif' width='60%'></p>


### 검색
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/e204937d-fd3a-4a49-bf99-399e54c17269/image.gif' width='60%'></p>


### 내 글
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/b56a5d1a-5c19-4310-8ac0-8059a1edd787/image.gif' width='60%'></p>


### 좋아요를 누른 포스트
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/66082a60-45ec-486b-b4b8-c33f6c590cc4/image.gif' width='60%'></p>

### 글 작성
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/8c964b80-1db1-4584-aea6-9b2ebd87e308/image.gif' width='60%'></p>

### 마이페이지
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/9eb244d8-673e-4ea9-9ce6-b1237f5d377c/image.png' width='60%'></p>

#### 비밀번호 변경
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/08fda750-eb18-4935-9261-65a7ca1483f4/image.png' width='50%'></p>

#### 회원 탈퇴
<p align='center'><img src='https://velog.velcdn.com/images/heftycornerstone/post/6f3d4009-0a4c-4f02-ad3c-b780f78ae413/image.png' width='50%'></p>


# 기술 스택

React
전역상태관리 : RTK, redux-persist
DB : Supabase
라우팅 : React-Router-Dom
스타일링 : Styled-Components

그 외 라이브러리
Toastify
React-Hook-Form
Slick-Carousel

# 팀원
