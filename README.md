# [🦁&nbsp;멋쟁이 사자처럼 FE 6기 Javascript 프로젝트] Enter EUID

<img width="320" alt="스크린샷 2023-08-02 12 57 21" src="https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/140426866/cc17ecd6-577b-4d8a-a25f-7348e1cb29dd">

<br />

## 🌈&nbsp;<span style="color: red">멋</span><span style="color: orange">쟁</span><span style="color: gold">이</span><span style="color: green">사</span><span style="color: blue">자</span><span style="color: navy">처</span><span style="color: purple">럼</span> JavaScript 프로젝트 16조&nbsp;⛅️

> 프로젝트 기간 : 2023년 7월 28일 ~ 2023년 8월 2일 <br />

> 발표 자료: https://docs.google.com/presentation/d/1dQDNeH2JcraF7RMDGaqDud1QcAXQLUoRCKW1fAQ2DO8/edit?usp=sharing

<br />

### 👫 TEAM 소개

|                                                             [김규민](https://github.com/Engsheet)                                                             |                                                            [김민성](https://github.com/Imeanstar)                                                             |                                                           [방서빈](https://github.com/seobinbang7)                                                            |                                                            [이은빈](https://github.com/ingbinsee)                                                             |
| :-----------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------: |
| <img width="200" height="200" src="https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/140426866/4440b538-2642-4ae2-8cfb-5eab72930884" /> | <img width="200" height="200" src="https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/140426866/d3802bfd-2a4d-4e5c-82aa-20e3eb2d51ab" /> | <img width="200" height="200" src="https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/140426866/0f8c39fd-b050-4c7d-9a3e-6f2d0bdcb19b" /> | <img width="200" height="200" src="https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/140426866/94906d38-ae44-4f77-acbb-0c9e96b92f8a" /> |

<br />

### 💻 담당 기능

| 이름   | 담당 기능                                                                                         |
| ------ | ------------------------------------------------------------------------------------------------- |
| 김규민 | 프로젝트 setting, 로고 페이지, 카테고리 페이지, 채팅 페이지, 전체 UI 및 스크립트 동작 점검 (QA)   |
| 김민성 | 스크럼 마스터, 로그인/회원가입 페이지, 회원가입/로그인 인증 페이지, 프로필 페이지, 웹 접근성 점검 |
| 방서빈 | 선배님 스토리 페이지, 스와이프 구현, 검색 페이지                                                  |
| 이은빈 | 기기 거래 페이지, 기기 거래 상세 페이지, 채팅 페이지 스크립트 기능 구현                           |

<br />

### ⚒️ Skills

<p herf="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=html,tailwind,js,git,github,figma"/>
</p>

<br />

### ⭐️ 가이드라인 준수 사항

#### 1. localStorage를 사용하여 "관심분야 선택 항목"을 저장했습니다.

#### 2. 회원가입 기능을 구현했습니다. (휴대폰 번호, input, button 구성)

#### 3. 회원가입을 통해 사용자를 생성하고 관리했습니다.

- 휴대폰 번호 입력시 랜덤한 6자리 난수를 생성
- 해당 인증번호 입력시 Upique ID 숫자를 부여 후 localStorage에 저장
- 해당 유저의 Unique ID를 확인 후 로그인
- 응답받은 Unique ID는 localStorage에 저장
- 다음 번에 로그인 시 Unique ID가 존재한다면 루트 경로로 리디렉션
- 어떤 경우든 Unique ID가 유효하지 않다면 사용자에게 알리고 로그인 페이지로 리디렉션
- 로그아웃은 클라인트 단에서 localStorafe에 저장된 Unique ID를 삭제하는 방식으로 구현

#### 4. 인증번호 유효성 검사했습니다.

- 휴대폰 번호: localStorage에 저장된 key 값으로 사용
- 인증번호 : 입력받은 고유한 ID를 value 값으로 가짐
- 휴대폰 번호와 인증번호 모두 입력, 조건을 만족해야 제출 버튼이 활성화

#### 5. 기기 거래 화면 구성했습니다.

- 데이터 스키마를 통해 데이터 설계 후 기기 거래 화면에 해당 데이터들 불러와 노출
- 거래 항목 선택시 디테일 페이지로 들어가 이미지, 유저정보, 본문 등을 불러와 노출

#### 6. 검색창 기능 구현했습니다.

- 검색 기능을 구현해 거래 항목의 text와 일치하는 항목들을 리랜더링

<br />

### ⚠️ 이슈

#### 1. stash사용 중 파일 삭제

> 문제상황

- 커밋할 내용을 Stash에 저장해 두었으나, 실수로 파일을 날리고, 마지막 commit은 하루전 내용이었던 상황. Stash에 두 가지 옵션이 있는데 꺼내면서 삭제하는 pop 옵션으로 진행하여 Stash에도 없고, reload를 해서 "ctrl + z"도 시행되지 않는 상황 발생.

> 해결방안

- https://www.baeldung.com/git-recover-dropped-stash
  해당 사이트 내용 참고하여 복구 완료

#### 2. 엔터 입력시 원하지 않는 곳을 선택

> 문제상황

- 회원가입,로그인 인증페이지에서 인증문자 입력 후 엔터를 입력했을 때, 동의하고 시작하기 가 눌러지는것이 바람직하나 인증문자 다시 받기가 눌러지는 이슈 발생

> 해결방안

- alert창으로 안내해주고 focus를 동의하고 시작하기 로 이동시키는 방식으로 해결

#### 3. 렌더링 시 data가 undefined로 처리되는 이슈

> 문제상황

- 페이지 로드 시 data.json에 저장된 정보를 화면에 렌더링해야 하나 데이터를 가져오지 못하는 이슈 발생

> 해결방안

- 구조 분해 할당으로 요소를 한 번 더 분해 후 적용하는 방식으로 해결

#### 4. 카테고리 검색 시 한글로 검색되지 않는 이슈

> 문제상황

- 한글 입력과 영어 입력의 매커니즘 차이에서 오는 문제
- APPLE은 A->AP->APP->APPL->APPLE의 방식으로 입력되지만 프론 은 ㅍ->프->플->프로->프론의 방식으로 입력되어 중간에 원치않는 값도 인식될 수 있음

> 해결방안

- 추가로 해당 완성값이 include true일 경우 hidden속성을 제거해주는 방식을 채택하여 이슈 해결

#### 5. 좋아요 버튼 클릭 시 동작하지 않는 이슈

> 문제상황

- 좋아요 버튼 클릭 시 html 파일에 마크업된 내용은 클릭 이벤트가 정상 작동하나, 동적 렌더링이 된 내용은 클릭 이벤트가 적용되지 않는 이슈 발생

> 해결방안

- 이벤트 위임을 활용하여 상위 요소에 클릭 이벤트를 주는 방법을 활용하여 해결

<br />

### 📷 페이지별 안내

#### 1. 회원가입 및 카테고리

![bandicam 2023-08-02 09-34-31-764](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/2140ca9f-9e87-433b-aa22-5403126fba29)

#### 2. 프로필 및 로그아웃

![bandicam 2023-08-02 09-51-13-939](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/64c02169-f453-416c-9554-3a5b7cfd92ce)

#### 3. 기기 거래

![bandicam 2023-08-02 12-17-03-625](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/b61e8dcd-1116-4840-8e2e-67a30ba3e016)

<br />

### 🏅 기능별 안내

#### 1. 모든 페이지의 상단 바

- 현재 시간 노출

#### 2. 선배님 스토리, 거래 기기, 마이 이듬 페이지의 하단 바

- 메뉴를 클릭하면 해당하는 메뉴의 아이콘만 색상 변경

#### 3. 시작 페이지

- Unique ID 없이 시작하기 누르면 유효하지 않음을 알리는 창이 뜨고 로그인 페이지로 리디렉션

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/bbea6c8d-b46b-427e-b110-7d524f7edb5d)

#### 4. 회원가입 및 로그인 페이지

- input에 휴대폰 번호 입력
- 정규 표현식으로 입력한 휴대폰 번호가 11자리 숫자인지 확인
- 입력받은 값과 정규표현식 매치되는지 확인
- 숫자 11자리 입력되면 인증번호 문자받기 버튼 활성화
- 활성화된 인증번호 문자받기 버튼 클릭하면 랜덤 숫자 alert 창으로 알림
- 인증문자 다시 받기 클릭 시 새로운 숫자 노출
- 노출된 숫자 그대로 입력을 해야 동의하고 시작하기 버튼 클릭이 됨
- 동의하고 시작하기 버튼을 클릭 시 선배님 스토리 페이지로 리디렉션
- 검색창에 관심분야 입력시 해당되는 관심분야만 노출
- "+" 버튼을 클릭 시 해당 관심분야의 데이터 값이 localStorage에 저장됨
- 체크된 버튼을 클릭 시 해당 관심분야의 데이터 값이 localStorage에서 삭제됨
- 이대로 저장할래요 버튼을 클릭 시 선배님 스토리 페이지로 리디렉션

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/518bb726-16a5-4caa-a28a-af322baf158a)

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/5be94cde-d1f4-44b2-8f53-488a7eed2cf4)

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/4a07ccab-2f30-48ad-af41-7a7d5fceb94b)

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/3989b913-fd8e-43d2-82a1-000746b45f70)

#### 5. 선배님 스토리 페이지

- swiper를 사용해서 data 값들을 슬라이드
- 다음으로 이동하는 화살표, 이전으로 이동하는 화살표 클릭 시 동작
- 중앙 밑에 위치한 버튼 클릭 시 슬라이드 정지 그리고 다시 클릭하면 버튼이 바뀌고 슬라이드 동작
- data.json의 데이터들을 fetch를 사용하여 불러와서 화면에 노출함
- 선배님 스토리, 기기거래, 질의응답, 같이해요 메뉴 클릭 시 text 색상이 바뀌고 border-bottom 생김

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/52963fc1-f4b9-4961-9dae-d7139763e04c)

#### 6. 검색 페이지

- input 창에 title 값 입력하고 enter 키 누르면 일치하는 값이 노출
- 노출된 리스트 클릭하면 상세페이지로 이동
- 친구들이 많이 찾고 있어요! 아래의 키워드 부분을 옆으로 밀면 슬라이드
- 키워드들을 선택하면 input 창에 입력됨
- 키워드 선택으로 input창에 입력된 상태에서 enter 키 누르면 일치하는 값이 노출
- 일치하는 값이 없을 경우 "검색 결과가 없습니다." 문구 페이지에 노출

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/426f9d3b-4a88-4ce8-86ce-22fa147f9889)

#### 7. 기기거래 페이지

- data.json의 데이터들을 fetch를 사용해서 불러와서 화면에 노출
- 하트 아이콘 클릭 시 붉은 색으로 변경되는 동시에 숫자 값 증가
- 증가된 상태에서 한번 더 클릭하면 색상이 변경되는 동시에 숫자 값 감소
- 리스트 클릭 시 상세 페이지로 리디렉션

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/6b2d483e-f81e-4826-92f3-4315a893c899)

#### 8. 상세페이지

- data.json의 데이터들을 fetch를 사용해서 불러와서 화면에 노출
- 상단 오른쪽에 위치한 다운로드 아이콘을 클릭하면 해당 페이지의 화면 파일이 다운로드됨
- 점 3개로 이루어진 아이콘을 클릭하면 메뉴가 노출 됨
- 한번 더 점 3개로 이루어진 아이콘을 클릭하면 메뉴가 사라짐
- 하트 아이콘 클릭 시 아이콘 색상 변경
- 하단에 노출되는 리스트들 선택하면 해당하는 상세페이지로 리디렉션
- 채팅하기 버튼 클릭 시 채팅 페이지로 리디렉션

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/07c981d6-e942-4913-a2f8-dca5ec273920)

#### 9. 채팅 페이지

- 상단 우측에 위치한 전화기 아이콘 클릭 시 FaceTime으로 연결됨 (mac으로 확인 가능)
- 점 3개로 이루어진 아이콘을 클릭하면 메뉴가 노출 됨
- 한번 더 점 3개로 이루어진 아이콘을 클릭하면 메뉴가 사라짐
- 메시지 보내가 input 창에 text를 입력하고 enter 키 또는 화살표 아이콘 클릭하면 해당 text가 말풍선으로 노출
- 메세지를 보낸 시점에서 현재 날짜 출력
- 메세지를 보낸 시점에서 현재 시간 출력

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/e8606902-ca78-406b-bbb3-476d2e0a8cc7)

#### 10. 마이 페이지

- 나의 프로필을 클릭하면 프로필 수정 페이지로 이동
- 프로필 수정 페이지에서 상단 우측 "x" 아이콘 클릭하면 마이 페이지로 리디렉션
- 로그아웃 클릭 시 localStorage의 데이터인 Unique ID 값 삭제

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/cc2fce1c-2da0-44e3-b419-51937ea065e4)

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/92416215-7578-4eb3-a7a3-da311c7abd7e)

![image](https://github.com/lion-js-project16-euid/lion-js-project16-euid/assets/81348938/6da62c20-ca8f-4d99-9b86-4ffb670db9f0)

<br />

### 💊 성능 검사

#### 1. 시작 페이지 (index.html)

![시작 페이지](https://lh6.googleusercontent.com/FzQF1Qt3RdpfnAonjFB_I__Yf7DXT5CaEqV4GAZkMYexliLUUcMH4r7rDj9CO0glOroCEkFE2zKzxSMgVO1aHJPTYcVTwodpGWgfJ_--8GvVgx-3vdOARYOVJegCp534CbGU_YKQoQFIpbw7fsnj2mVE9g=s2048)

#### 2. 회원가입 & 로그인 (sign-up.html & login.html)

![회원가입 & 로그인](https://lh3.googleusercontent.com/zYToZMJiQAiIbHAEcRjglhwtSbM7MuJ710-dOVpbPZzVGCHyRBD7NkxdhIznpJgbBwzVpfOF0Pn-iJ07qUwOYl8PXaIRjiZbPbzsVbnH1jgzN0tQExzJyA-KtNoxRY-gZ2eIWE3N_3U3A1dSreB69RPO6A=s2048)

#### 3. 회원가입 & 로그인 인증 (sign-up-certification.html & login-certification.html)

![회원가입 & 로그인 인증](https://lh3.googleusercontent.com/u0Dm-stxnec4KbOahqo3SC07XXEI5xoSZXcrRvFamjWcIja1Rzkjwo4g1_wWUwwaX63Fvvv26cTyoNgXAslOHzDaexg4OWbjqmZviHND67wP8NXPgtV9XLTqjxwcWLmb70OhQLvT3m82uJiPR812KFhw-g=s2048)

#### 4. 카테고리 (category.html)

![카테고리](https://lh3.googleusercontent.com/vHz02nVpyfZNQ1-tFwnA-eDMUNoWZifbmzBMmA-pPFEA2uqphtRvtPgqnS5gEdZILeAsogAu_nL4fALsteTb89EFGaU3bvG0mNR_XK7QVmv4fN1u71wBZi6i2ZoX3k_DbnIhZzYRN6VOxj3EwfuJ9W7yoQ=s2048)

#### 5. 선배님 스토리 (story.html)

![선배님 스토리](https://lh3.googleusercontent.com/yW1Ydf9mJswyxWm8zV--mOKQnMUfVVrz0Tb9_Tp0andGlnHr2iteJorkuXqPdGUVw2CpnxoHLg1ADejyVvOP5ftzRGdUWzu0jE0RsFuN3u2KvzpjQY5NPPaGCjc7_t1lDuLwIqnV1Pt2UaGv09FJH8REgQ=s2048)

#### 6. 기기 거래 (device.html)

![기기 거래](https://lh5.googleusercontent.com/I2WWxFG8Et4gdePibRgnb-bhcx6DXyHxp_AnBb96yv1IPz9W88EEsN9d54FaO0MnF94hYOejxUOr0nPl9S4gGgx0fWtPBHNwF9H2DiVuDGckFko28c1KJ0T9w93Z2xJHvt7vRRKlgKJ894Wq16QfOcCjNw=s2048)

#### 7. 기기 상세

![기기 상세](https://lh4.googleusercontent.com/-1czJ3cZIXMz-wUiBo1vDgWimxucD-AGttkFQMt1KiAsPJdkMXmYaaubasvXdQXZyAP-HGxRTyUZpGahQYXIb3NBlySJRk64r2O2wrTCBYyll-RN-VG1099jmZdrWylJOTphPcjvPIURRl77uDjmfJz44A=s2048)

#### 8. 기기 거래 채팅 (chat.html)

![기기 거래 채팅](https://lh5.googleusercontent.com/Zl75ayf5bVGTnCnqpAcNSTbdPCdlIlloElf6z64fWjBFnJ7J9LXVahVDpYRGePBcOWJh437G80TukvPlewxVvUTT-Mlp_dRqjEKm_In5TVX_rMImWJzU8Fwly6Z7Kyvp0-DFmKmT38dqwUGd-kqGIS78wg=s2048)

#### 9. 프로필 (profile.html)

![프로필](https://lh5.googleusercontent.com/WIeI6uWe2RFq9LNzQ0bjsc3Tnpyy4wEKByvfoWK11G6N497a4wGDPAGOLSuYhQe6wnOUFHJTa_8aYRKMAfrpwP8eKf2J1ef1_U-Pw84RuX5D7VA93P6tP3hEqrW9RyUDojO6oyXcv-3DAPIYvglYSm-jJw=s2048)

#### 10. 프로필 수정 (profileCard.html)

![프로필 수정](https://lh6.googleusercontent.com/tQPTgYgz8KNWZyurtrOyGKPJ6w77eOqTKHce6ByaApfd9nzdqow8PQoACGwFJ2rmB8BdolQrElY5lsnk9JeSdTPTJUThZZnuKhWLqQ3hrFP2XSKqLXyq8KwpVRTbytT8k6siMlmnZ7eI7zYcMXJ4G4bPEg=s2048)

<br />

### ✏️ 프로젝트 소감

#### 🧑🏻‍💻 김규민

직접 스크립트를 조원 분들에 비해 많이 만들지는 않았지만, 다른 분들의 코드가 제대로 동작하는지 QA하고 리팩토링을 하는 기회를 가져서 좋았고,
기능 구현에서 여러 많은 문제가 있었는데 시간이 부족해 해결하지 못한 문제도 있지만, 발견했던 문제들 중에 대부분은 같이 해결할 수 있었어서 만족스러웠습니다.
ESlint / Prettier 와 코딩 컨벤션 등의 틀을 처음부터 작성해본 경험도 좋았습니다.
이것저것 바꿔달라고 요청드린 게 많았는데 다들 너무 고생하셨습니당 ㅠㅠ

#### 🧑🏻‍💻 김민성

단기간에 많은 작업을 하게 되어서 힘들었지만 좋은 경험이었습니다.
파일을 날려먹는 실수도 했지만, 도움을 받아 복구하였고 그것 또한 좋은 경험이라 생각합니다.
localStorage관련해서만 많이 다뤄보아서 다음에 기회가 된다면 json관련으로도 다뤄보고싶습니다.
제가 부족한 부분들 다른분들께서 너무 잘 채워주셔서, 바빴지만 그래도 싸우지 않고 수월하게 잘 끝났던 것 같아서 만족스럽습니다 :)

#### 👩🏻‍💻 방서빈

js 프로젝트를 진행하면서 fetch로 json 데이터를 불러오려는 과정에서 긴시간동안 부딪쳐 힘들었지만.. 또 그만큼 새로 알게된 지식들이 있어 해결하고 돌아보니 좀 뿌듯했습니다. 해결하고 나면 계속 이어지는 에러와 입력한 값과 다르게 적용되는 스타일의 공격에 몸에 힘이 빠져나가는 것처럼 지치기도 했지만 프로젝트 조원들의 응원과 회고조원들과의 대화에 힘을 짜낼 수 있었던 것같습니다. 과정은 진짜 많이 힘들었지만 뿌듯합니다.. 근데 뿌듯한만큼 실력 부족으로 구현하지 못한 기능들에대한 아쉬움이 남는 건 어쩔 수 없는 것같습니다. 자바스크립트의 동작 방식과 순서의 중요성을 이해할 수 있었던 좋은 경험이었습니다.

#### 👩🏻‍💻 이은빈

동적 렌더링을 진행하며 브라우저 렌더링의 순서 및 과정에 영향을 받아 페이지 틀이 무너지거나 동적인 기능이 구현하지 않는 등의 문제를 겪었습니다. 이를 통해 문제 상황을 해결하는 능력을 기를 수 있었으며, 동료들과 함께 고민하는 과정을 통해 협업에 대한 중요성을 다시 한 번 깨달을 수 있었습니다. 또한, 자바스크립트 기능 작동 원리에 대해 더욱 알 수 있는 시간이었습니다.
다양한 기능을 고민하고 구현하는 과정을 통해 자바스크립트에 대한 이해를 높일 수 있었으며 기능 구현에 대한 흥미를 한 층 더 높일 수 있는 계기가 되었습니다.

<br />

### 🦾 프로젝트 사용법

#### 백엔드 서버 실행

```bash
npm run serve:backend
```

#### 프론트 서버 실행

```bash
npm run serve:frontend
```

#### tailwind 실행

```bash
npm run tailwind
```

#### 동시 실행

```bash
npm start 또는 npm run start
```
