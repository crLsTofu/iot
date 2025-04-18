# 싸이월드 미니홈피 (Cyworld Mini Homepage)

추억의 싸이월드 미니홈피를 재현한 레트로 웹사이트 프로젝트입니다.

## 프로젝트 소개

이 프로젝트는 2000년대 초중반 한국에서 큰 인기를 끌었던 싸이월드 미니홈피의 UI/UX를 재현하였습니다. 
HTML, CSS, JavaScript를 사용하여 만들어졌으며, 실제 싸이월드의 디자인 요소와 기능을 최대한 유사하게 구현하였습니다.

## 주요 기능

- 체크무늬 배경과 하늘색 테두리의 미니홈피 프레임
- Today/Total 방문자 카운터
- 프로필 섹션 (프로필 이미지, 상태 메시지)
- 음악 플레이어 (HTML5 Audio 태그 활용)
- 방명록 기능 (등록 및 삭제)
- 미니룸 섹션
- 다이어리 탭
- 모바일 반응형 디자인

## 기술 스택

- HTML5
- CSS3
- JavaScript (ES6+)
- Bootstrap 5 (일부 유틸리티 클래스만 활용)

## 데이터 구조

미니홈피 데이터는 모듈화되어 관리됩니다:

```js
const personalData = {
    // 프로필 정보
    profile: {
        homepageTitle: "...",
        todayFeeling: "...",
        statusMessage: "...",
        profileInfo: {
            name: "...",
            birthday: "...",
            email: "..."
        }
    },
    
    // 음악 정보
    songs: [
        {id: '...', title: '...', src: '...'},
        // 음악 목록
    ]
};
```

## 프로젝트 구조

```
/
├── index.html           # 메인 HTML 파일
├── css/
│   └── style.css        # 스타일시트
├── js/
│   ├── script.js        # 자바스크립트 로직
│   └── personal-data.js # 프로필 및 음악 데이터 (통합된 데이터 파일)
├── audio/               # 음악 파일 디렉토리
│   └── *.mp3            # 음악 파일들 (별도 추가 필요)
└── images/
    └── characters/      # 방명록 캐릭터 이미지 등
```

## 사용 방법

1. 이 저장소를 클론합니다:
   ```
   git clone [repository URL]
   ```
2. audio 디렉토리에 음악 파일을 추가합니다 (아래 "음악 플레이어 세팅" 섹션 참조).
3. 웹 브라우저에서 `index.html` 파일을 엽니다.
4. 미니홈피를 즐기세요!

## 구현된 기능

- 방문자 수 카운터 (localStorage 활용)
- HTML5 Audio를 활용한 음악 플레이어
- 음악 선택, 재생/일시정지, 이전/다음 트랙 기능
- 재생 진행 바 및 시간 표시 기능
- 방명록 작성 및 삭제
- 미니룸 댓글 등록
- 탭 메뉴 전환 기능
- 다이어리 작성 기능
- 모듈화된 데이터 구조로 유지보수성 향상

## 음악 플레이어 세팅

프로젝트를 실행하기 위해서는 다음 음악 파일을 별도로 준비하여 `audio/` 디렉토리에 추가해야 합니다:
1. `DAUL, Noair, plan8, CHANNEL 201 - SIMPLE (Feat. JUNNY, 창모 (CHANGMO)).mp3`
2. `Turtles(거북이) - Airplane(비행기).mp3`
3. `Blue spring (작전명 청-춘!)_잔나비.mp3`

*참고: 음악 파일은 저작권 문제로 Git 저장소에 포함되어 있지 않습니다.*

## 최근 업데이트

- 하드코딩된 데이터를 분리하여 모듈화
- 프로필 데이터(profile-data.js)와 음악 데이터(music-data.js)를 personal-data.js로 통합
- 모든 미니홈피(leejaewon, leejaeseong, kimsiyeon, hwangyooseok)에 변경사항 적용
- 데이터 구조 개선으로 유지보수성 향상

## 향후 개선 사항

- 일촌 관리 기능 추가
- 미니미 설정 기능
- 사진첩 기능
- 방명록 작성 폼 구현
- 플레이리스트 저장 기능

## 라이센스

???
