## 브랜치: 새 브랜치 만들기

<img width="473" height="314" alt="스크린샷 2026-03-30 오전 11 45 06" src="https://github.com/user-attachments/assets/629b8102-0e72-46d3-bc67-da5637ec7757" />

상단 브랜치 버튼 클릭 -> 다음과 같이 적기

```
feature/detail-page
```
새 브랜치 체크아웃 체크 -> 브랜치 생성

<img width="1162" height="657" alt="스크린샷 2026-03-30 오전 11 46 35" src="https://github.com/user-attachments/assets/b7677d2a-9f18-43fe-bd9b-2a4d45213581" />

하면 이렇게 나옴.

<img width="620" height="147" alt="스크린샷 2026-03-30 오전 11 51 54" src="https://github.com/user-attachments/assets/9b26af7e-4c1d-48aa-be0a-db851af16ebd" />

detail-page.md 파일 만들고

<img width="1162" height="657" alt="스크린샷 2026-03-30 오전 11 50 27" src="https://github.com/user-attachments/assets/1a55b693-071a-4400-9ddf-29f074c465c8" />

커밋하셈.

<img width="668" height="234" alt="스크린샷 2026-03-30 오전 11 53 02" src="https://github.com/user-attachments/assets/7c1924eb-59d3-4b65-9035-2a3a2d3b3d41" />

그리고 feature-list.md 도 수정하고

<img width="814" height="491" alt="스크린샷 2026-03-30 오전 11 53 54" src="https://github.com/user-attachments/assets/f8427806-d38b-49a8-b9a8-95358a712aab" />

-에 바뀐 내용 즉시 푸시 체크 -> 커밋

<img width="949" height="455" alt="스크린샷 2026-03-30 오전 11 55 42" src="https://github.com/user-attachments/assets/7cfb7343-e92e-4456-9e99-53be06372c6c" />

깃허브에서도 브랜치 바꾸면 볼 수 있음.

---

## 체크아웃

1. 사이드바 브랜치에서 원하는 브랜치를 우클릭 후 체크아웃을 하거나 더블클릭
2. 새 브랜치 생성.. 이름은 feature/cart

<img width="614" height="228" alt="스크린샷 2026-03-31 오후 6 52 44" src="https://github.com/user-attachments/assets/3f4a2bf6-db01-46b5-954e-00207869d191" />

feature-list.md 파일을 위 처럼 수정

<img width="739" height="167" alt="스크린샷 2026-03-31 오후 6 54 19" src="https://github.com/user-attachments/assets/e0bda2fc-273d-4218-9a20-ab2530d31804" />

cart.md를 만들어서, 위 처럼 작성.

<img width="1440" height="821" alt="스크린샷 2026-03-31 오후 6 55 32" src="https://github.com/user-attachments/assets/e4addddb-3bb3-4098-aed2-23883cc81b50" />

그리고 커밋.

<img width="1199" height="188" alt="스크린샷 2026-03-31 오후 6 56 43" src="https://github.com/user-attachments/assets/9b50a235-8765-4ce9-b04c-57eccd79ff26" />

그럼 이렇게 됨.

---

## 병합: 브랜치와 브랜치 합치기

1. main으로 체크아웃.
2. 병합하려는 커밋에서 마우스 오르녹 클릭 후 병합 선택

<img width="636" height="189" alt="스크린샷 2026-03-31 오후 7 05 57" src="https://github.com/user-attachments/assets/50ae1b5a-928e-4a08-8eb1-9d0a8f5ce9fb" />

하지만 origin/main은 그대로.
상단 push 누르고, main 체크한 다음에 확인 누르면 다음처럼 됨.

<img width="989" height="208" alt="스크린샷 2026-03-31 오후 7 07 31" src="https://github.com/user-attachments/assets/b8b7d877-0de9-47c5-9f58-2d577e01083e" />

---

## 충돌
main 체크아웃 하고, feature/cart을 병합 하면 충돌메시지 뜸.

<img width="511" height="379" alt="스크린샷 2026-03-31 오후 7 30 08" src="https://github.com/user-attachments/assets/01122a57-9ea3-4c1e-863d-ea0c2fb3d867" />

히스토리 창에서 어떤게 충돌인지 확인 가능.
vsc에서 충돌이 난 파일을 수정하고 커밋.

<img width="591" height="196" alt="스크린샷 2026-03-31 오후 7 31 47" src="https://github.com/user-attachments/assets/c5d1a3cb-7a1c-424d-8830-18ce0656cf9b" />

그럼 이렇게 됨.

---

## 풀 리퀘스트

### 브랜치 생성
1. feature/comment 브랜치 생성
2. comment.md 파일 생성후 "댓글 기능" 작성.
3. 커밋

<img width="564" height="214" alt="스크린샷 2026-03-31 오후 7 38 35" src="https://github.com/user-attachments/assets/620e8da6-a520-41e7-8744-61307fd14679" />

### 풀 리퀘스트 보내기

<img width="919" height="390" alt="스크린샷 2026-03-31 오후 7 39 12" src="https://github.com/user-attachments/assets/f268c312-242b-4a33-a3b4-dc65d4b1b97f" />

깃허브에 가면 저런 메시지가 뜸.
초록색 버튼 클릭.

<img width="917" height="493" alt="스크린샷 2026-03-31 오후 7 39 49" src="https://github.com/user-attachments/assets/bc895924-2b91-4f23-b367-09df3d54a7aa" />
<img width="910" height="296" alt="스크린샷 2026-03-31 오후 7 40 22" src="https://github.com/user-attachments/assets/f037bc85-733a-40b9-96b7-5a1661ddde8f" />

이렇게 됨.

<img width="888" height="199" alt="스크린샷 2026-03-31 오후 7 41 22" src="https://github.com/user-attachments/assets/a0f09b28-823c-4b54-a16e-b39c38ee7111" />

수락하려면 저거 누르면 됨.

<img width="618" height="228" alt="스크린샷 2026-03-31 오후 7 42 15" src="https://github.com/user-attachments/assets/b3ea763f-38e2-45f3-b668-098afb44985b" />

소스트리에서는 패치버튼을 누르고, main을 체크아웃 하고 pull 하면 됨.

---

## 릴리즈
원하는 브랜치 우클릭 -> 태그 -> 태그 이름(v1.0.0) 작성 

그리고 푸시 -> 모든 태크 푸시를 하면 깃허브에 태그가 보임.
태그도 푸시해줘야함.
