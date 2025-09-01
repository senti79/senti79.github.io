# BOMS 메시지 저장소

이 저장소는 BOMS 앱의 전광판 메시지와 관련 콘텐츠를 관리합니다.

## 📋 포함 내용

- **messages.json**: 전광판 메시지 데이터
- **features/**: 기능 소개 페이지들
- **challenges/**: 도전과제 상세 페이지들
- **dev-behind/**: 개발비하인드 스토리들
- **fun-facts/**: 재미있는 사실들
- **promotions/**: 프로모션 및 이벤트 안내

## 🚀 사용법

### 1. 메시지 추가/수정
`messages.json` 파일을 편집하여 새로운 메시지를 추가하거나 기존 메시지를 수정할 수 있습니다.

### 2. 상세 페이지 생성
각 메시지의 `link` 필드에 해당하는 HTML 페이지를 생성하여 자세한 내용을 제공할 수 있습니다.

### 3. 실시간 업데이트
GitHub에 푸시하면 자동으로 GitHub Pages에 반영되어 사용자들에게 실시간으로 전달됩니다.

## 📁 파일 구조

```
├── messages.json                    # 메시지 데이터
├── features/                        # 기능 소개
│   ├── keyboard-shortcuts.html
│   └── new-features.html
├── challenges/                      # 도전과제
│   ├── 7-day-streak.html
│   └── monthly-challenge.html
├── dev-behind/                      # 개발비하인드
│   ├── ticker-system.html
│   └── architecture.html
├── fun-facts/                       # 재미있는 사실
│   ├── tiptap-editor.html
│   └── history.html
└── promotions/                      # 프로모션
    ├── monthly-challenge.html
    └── special-events.html
```

## 🔧 메시지 타입

- **user-tip**: 사용자 팁 및 가이드
- **dev-behind**: 개발 과정 및 기술적 내용
- **challenge**: 도전과제 및 목표
- **fun-fact**: 재미있는 사실 및 정보
- **promotion**: 프로모션 및 이벤트

## 📝 메시지 형식

```json
{
  "id": "고유ID",
  "type": "메시지타입",
  "text": "전광판에 표시될 텍스트",
  "priority": 우선순위숫자,
  "link": "상세페이지URL",
  "createdAt": "생성일시"
}
```

## 🎯 우선순위

- **1**: 가장 높은 우선순위 (사용자 팁)
- **2**: 높은 우선순위 (개발비하인드, 재미있는 사실)
- **3**: 중간 우선순위 (도전과제)
- **4**: 낮은 우선순위 (프로모션)

## 🔄 업데이트 방법

1. `messages.json` 파일 편집
2. 필요시 상세 페이지 HTML 파일 생성/수정
3. GitHub에 커밋 및 푸시
4. 자동으로 GitHub Pages에 반영

## 📞 지원

문제가 있거나 새로운 기능을 요청하려면 이슈를 생성해주세요.

## 라이센스

MIT License - 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.
