# PlayPick
It's for PlayPick

---
## 👤 팀원 구성

<table class="tg"><thead>
  <tr>
    <th class="tg-9353"><span style="font-weight:bold">최현수</span></th>
    <th class="tg-9353"><span style="font-weight:bold">김정민</span></th>
    <th class="tg-9353"><span style="font-weight:bold">이신원</span></th>
    <th class="tg-9353"><span style="font-weight:bold">전지연</span></th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-9353"><img src="https://cdn.discordapp.com/attachments/1383999022238273586/1384715997809741945/image.png?ex=685370c4&is=68521f44&hm=a179a00ce94ed8a5958c96b23ad7bffe5b7f4daddb69ae2b87bd6bc187ef71f8&" alt="Image" width="109" height="100"></td>
   <td class="tg-9353"><img src="https://avatars.githubusercontent.com/u/6846349?s=80&v=4" alt="Image" width="109" height="109"></td>
    <td class="tg-9353"><img src="https://mblogthumb-phinf.pstatic.net/MjAxNzExMTNfOTkg/MDAxNTEwNTE5MDU1OTAx.CgrsefuknGH3WyTiveT8LsFGXw288baNiov22l9sCywg.x3YtB2I7VXitiMcvgOkRkiH5umtLrNWj7IothphFwF0g.PNG.211grims/136.png?type=w800" alt="Image" width="109" height="100"></td>
    <td class="tg-9353"><img src="https://cdn.discordapp.com/attachments/1383999022238273586/1384715530136715366/1750066148038.jpg?ex=68537055&is=68521ed5&hm=74fb22315aca7246b65fbf04678837fb854606ec610d37f84029ecbba24a583b&" alt="Image" width="109" height="100"></td>
  </tr>
  <tr>
<td class="tg-7btt" style="text-align: center;">
  <a href="https://github.com/IMCODER0000" target="_blank" rel="noopener noreferrer" >GitHub</a>
</td>
<td class="tg-7btt" style="text-align: center;">
  <a href="https://github.com/Mur-pixel" target="_blank" rel="noopener noreferrer">GitHub</a>
</td>
<td class="tg-9353" style="text-align: center;">
  <a href="https://github.com/redEevee" target="_blank" rel="noopener noreferrer">GitHub</a>
</td>
<td class="tg-7btt" style="text-align: center;">
  <a href="https://github.com/dia0723" target="_blank" rel="noopener noreferrer">GitHub</a>
</td>

  </tr>
</tbody></table>
  
  
</div>

---

## 🧩 구조 설명

- **모노레포 기반 구조**로 구성되어 있으며, `Lerna`를 통해 각 앱을 효율적으로 관리합니다.
- `main-container`는 전체 앱의 진입점 역할을 하며, Micro Frontend 방식으로 각 앱(`Landing-Page`, `choices-of-a-spring-day`, `navigation-bar-app`,`person-quiz-game`,`spot-the-difference`,`versus-game`,`navigation-bar-app`)을 로드합니다.
- 각 앱은 **독립적으로 개발 및 배포 가능**하도록 설계되어 있습니다.
  
---
기술스택
---
시작페이지 
---

---

<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
 PlayPick 프로젝트 구조
 
</head>
<body>
  <div>
    <p><span class="folder">📁 PlayPick</span></p>
    <p>├── <span class="folder">📁 choices-of-a-spring-day/</span> # 게임 페이지</p>
    <p>│   ├── <span class="folder">📁 public/</span> # 이미지 리소스</p>
    <p>│   └── <span class="folder">📁 src/</span> # React 기반 게임 로직</p>
    <p>├── <span class="folder">📁 Landing-Page/</span> # 랜딩 페이지 프론트엔드</p>
    <p>│   ├── <span class="folder">📁 public/</span> # 이미지 및 LandingImage 하위 폴더</p>
    <p>│   └── <span class="folder">📁 src/</span> # React 기반 UI 구성</p>
    <p>├── <span class="folder">📁 main-container/</span> # 메인 컨테이너 (모듈 연동 및 통합 관리)</p>
    <p>│   ├── <span class="folder">📁 @mf-types/</span> # 모듈 간 타입 정의</p>
    <p>│   └── <span class="folder">📁 src/</span> # 메인 앱 진입점</p>
    <p>├── <span class="folder">📁 person-quiz-game/</span> # 게임 페이지</p>
    <p>│   └── <span class="folder">📁 src/</span> # 메인 앱 진입점</p>
    <p>├── <span class="folder">📁 spot-the-difference/</span> # 게임 페이지</p>
    <p>│   └── <span class="folder">📁 src/</span> # 메인 앱 진입점</p>
    <p>├── <span class="folder">📁 versus-game/</span> # 게임 페이지</p>
    <p>│   └── <span class="folder">📁 src/</span> # 메인 앱 진입점</p>
    <p>├── <span class="folder">📁 navigation-bar-app/</span> # 네비게이션 바 모듈 앱</p>
    <p>│   └── <span class="folder">📁 src/</span> # 컴포넌트 및 스타일</p>
    <p>├── <span class="folder">📁 node_modules/</span> # 의존성 모듈 (자동 생성)</p>
    <p>├── <span class="folder">📁 .idea/</span> # JetBrains IDE 설정</p>
    <p>├── <span class="file">package.json</span> # 루트 패키지 의존성</p>
    <p>├── <span class="file">lerna.json</span> # Lerna 설정 (모노레포 관리)</p>
    <p>└── <span class="file">README.md</span> # 프로젝트 소개 파일</p>
  </div>
</body>
</html>

---

## 📷 결과 화면 예시
(아래 스크린샷은 실제 구현된 결과를 캡쳐하여 삽입)

### 랜딩 페이지

#### 게임 소개 섹션 
- 다양한 게임 콘텐츠(밸런스 게임, 틀린그림 찾기, 인물 맞추기, 시뮬레이션 게임 등)를 카드 형태로 배치하여 직관적인 탐색이 가능하도록 구성했습니다.
![image](https://github.com/user-attachments/assets/b4f25cd1-aa6e-4702-8656-fae8e452a00d)
![image](https://github.com/user-attachments/assets/674e837c-f585-46f6-a902-70306117dbb3)

#### 서비스 특징 강조
- "다양한 콘텐츠", "혼자 그리고 함께", "성취와 보상" 등 사용자가 느낄 수 있는 주요 혜택을 시각적으로 간결하게 표현했습니다.
![image](https://github.com/user-attachments/assets/5f24745d-b3a6-4460-bc8e-8d1c8ff67ce0)

#### 유저 후기 섹션
- 이용자들의 생생한 후기를 배치하여 신뢰성과 공감대를 높였습니다.
![image](https://github.com/user-attachments/assets/c460139a-2e50-4e84-99e9-c4be10a08f0c)

#### Call to Action
- "지금 바로 시작할 준비가 되셨나요?"라는 문구와 함께 무료 시작 버튼을 하단에 배치해 사용자의 행동을 유도합니다.
![image](https://github.com/user-attachments/assets/ff838878-8b3c-4257-b25c-96ef16c7df26)

---

### Versus Game 페이지
- 두 가지 극단적인 선택지 중 하나를 반드시 골라야 하는 심리게임입니다.
- 가벼운 질문부터 토론을 유발하는 질문까지 다양한 주제로 구성되어 있습니다.
![image](https://github.com/user-attachments/assets/3127a195-4bbb-4fef-b308-4b324b20f986)
![image](https://github.com/user-attachments/assets/d5eab00a-5471-4189-96be-c9e43bebca6c)
![image](https://github.com/user-attachments/assets/b41d4370-6e21-4d99-9fff-c075f22e6616)

---

### 틀린 그림 찾기 게임
- 두 장의 비슷한 그림을 제한 시간 내에 서로 다른 부분을 찾아내는 관찰력 게임입니다.
![image](https://github.com/user-attachments/assets/37ed29d5-4cb0-4aa8-9f88-d4f94c1c36fa)
![image](https://github.com/user-attachments/assets/e18ca7ab-bba9-4740-a7eb-a296eb8d1ee9)

---

### 인물 맞추기 게임
- 사진을 보고 정답을 추리하는 퀴즈로, 재미있게 관찰력과 추리력을 높일 수 있습니다.
![image](https://github.com/user-attachments/assets/d41a1665-f397-49b7-ad88-bc0a81f180da)
![image](https://github.com/user-attachments/assets/e6c2fcbd-1776-4beb-a087-1d0dbcc087a1)
![image](https://github.com/user-attachments/assets/7aa49c51-9ad6-4aaa-b7c6-6094abc7f37b)

---

### 시나리오 게임
- 사용자가 주어진 상황과 선택지에 따라 스토리를 진행하는 형식의 게임으로, 자신의 선택에 따라 다양한 전개를 즐길 수 있습니다.
![image](https://github.com/user-attachments/assets/2273c812-9cfb-4b22-a312-cfc1321366f6)
![image](https://github.com/user-attachments/assets/1d70f9d2-d0c5-4ef6-ba6c-2533aad66040)
![image](https://github.com/user-attachments/assets/d1646219-ffb8-4684-9f84-5b516afa3dae)

---

### 로그인 화면(소셜 로그인 혹은 게스트 로그인 선택)
- 사용자 편의성을 고려해 간결하고 직관적인 구조로 설계되었습니다.
- 상단에는 PlayPick 로고와 함께 환영 메시지를 배치하여 브랜드 아이덴티티와 서비스 목적을 전달합니다.
- 카카오 로그인을 통해 간편하게 시작할 수 있도록 구성하고, 별도의 회원가입 없이도 이용 가능한 게스트 모드를 제공해 진입 장벽을 낮췄습니다.
- 하단에는 이용약관 및 개인정보처리방침을 명시하여 서비스 이용에 대한 신뢰성을 높였습니다.
![image](https://github.com/user-attachments/assets/c816b533-14d2-4b0a-a912-e4bb6f8a32a2)




