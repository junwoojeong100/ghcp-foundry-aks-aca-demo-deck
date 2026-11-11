# GitHub Copilot × Microsoft Foundry × ACA · AKS — 데모로 보는 AI 앱 개발·운영

데모 중심 소개 슬라이드(**21장**)입니다. 만들고(GitHub Copilot), 지능을 붙이고(Microsoft Foundry), 올려서 운영하는(Azure Container Apps · AKS) 전 과정을 슬라이드가 아니라 **실제 실행 화면과 검증 기록**으로 보여 줍니다. 슬라이드 안에 화면 녹화 영상 **7개**(합계 약 4분 40초)가 들어 있고, 한국어 발표 노트가 달려 있습니다.

**English edition:** 영문판 슬라이드(영문 발표 노트 포함)도 있습니다 — [README.en.md](README.en.md)

## 웹에서 바로 보기 — 다운로드 없이

| | |
| --- | --- |
| **슬라이드 — 한국어** (21장, 영상 7개 내장) | [📑 브라우저에서 열기](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fjunwoojeong100.github.io%2Fghcp-foundry-aks-aca-demo-deck%2FGitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_KO.pptx) |
| **PPTX — 한국어** | [⬇ GitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_KO.pptx](https://junwoojeong100.github.io/ghcp-foundry-aks-aca-demo-deck/GitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_KO.pptx) (약 32 MB) |
| **슬라이드 — English** (21장, 영상 7개 내장, 영문 발표 노트) | [📑 브라우저에서 열기](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fjunwoojeong100.github.io%2Fghcp-foundry-aks-aca-demo-deck%2FGitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_EN.pptx) |
| **PPTX — English** | [⬇ GitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_EN.pptx](https://junwoojeong100.github.io/ghcp-foundry-aks-aca-demo-deck/GitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_EN.pptx) (약 32 MB) |

슬라이드는 Microsoft 의 PowerPoint for the web 으로 열립니다. 영상 위 ▶ 를 누르면 재생되고, 오른쪽 아래 **Notes** 에서 발표 노트를, **Start Slide Show** 에서 전체 화면 발표를 볼 수 있습니다. 영상이 들어 있어 파일이 크므로 처음 열 때는 로딩에 시간이 걸릴 수 있습니다. 웹 뷰어는 자체 글꼴을 쓰므로 줄바꿈이 데스크톱 PowerPoint 와 조금 다를 수 있습니다. 정확한 모양은 PPTX 를 내려받아 확인하세요.

영문판은 한국어판과 같은 21장·같은 구성입니다. 데모 1~5 영상은 [foundry-ghcp-demo-deck](https://github.com/junwoojeong100/foundry-ghcp-demo-deck) 영문판의 **영어 재녹화본**(Copilot CLI 응답, Foundry 샘플 질문·답변까지 화면이 모두 영어)이라, 이 데모들의 수치가 한국어판과 조금 다릅니다(예: Copilot 실행 38.0분·테스트 26 → 100개, Foundry 평가 약 4.5분). 데모 6·9 영상은 원본 녹화에서 **캡션·배속 라벨 같은 편집 오버레이만 영어로 교체**했습니다.

## 데모 구성 (10개)

| # | 영역 | 데모 | 형태 | 슬라이드 |
| --- | --- | --- | --- | --- |
| 1 | GitHub Copilot | 구현·테스트 — 26 → 117 테스트 | ▶ 영상 | 5 |
| 2 | GitHub Copilot | 안전장치 — Hook이 위반을 차단 | ▶ 영상 | 6 |
| 3 | Microsoft Foundry | 에이전트 + 문서 — 근거·출처를 표시 | ▶ 영상 | 8 |
| 4 | Microsoft Foundry | Guardrails — 탈옥을 입구에서 차단 | ▶ 영상 | 9 |
| 5 | Microsoft Foundry | Evaluations — 품질·안전 자동 채점 | ▶ 영상 | 10 |
| 6 | Azure Container Apps | `azd up` 한 번 — Foundry + 앱까지 | ▶ 영상 | 12 |
| 7 | Azure Container Apps | Actions → 새 리비전 — OIDC · 비밀 없음 | ◆ 검증 기록 | 13 |
| 8 | Azure Container Apps | AI 코드 샌드박스 — 격리 · 검사 · 승인 | ◆ 검증 기록 | 14 |
| 9 | AKS | Terraform → AKS — 실제 Azure · 노드 3 Ready | ▶ 영상 | 16 |
| 10 | AKS | kubectl · Portal — HTTP 200까지 확인 | ■ 확인 화면 | 17 |

- **▶ 영상** 실제 화면·실행 녹화입니다. 소리가 없고, 기다리는 구간은 잘라내거나 배속했습니다.
- **◆ 검증 기록** 영상 없이, 실제 배포·검증 결과와 그때 쓴 명령을 정리한 슬라이드입니다. 데모 7은 2026-07-21, 데모 8은 2026-07-24~29 에 실행한 과거 기록이므로 현재 동작은 시연 전에 다시 확인하세요.
- **■ 확인 화면** 실제 실행에서 캡처한 정지 화면입니다.

> 화면의 모델·기능은 구독·리전·시점에 따라 다를 수 있습니다. 데모 8의 ACA Sandboxes 는 덱 작성 시점(2026-11)에 Preview 였습니다. 슬라이드의 소요 시간·개수는 각 데모의 1회 실측·기록이며 서로 직접 비교하는 용도가 아닙니다.

## 출처 · 더 보기

영상과 검증 기록의 원본은 모두 [junwoojeong100](https://github.com/junwoojeong100) 계정의 공개 저장소입니다.

| 데모 | 저장소 | 내용 |
| --- | --- | --- |
| 1–2 | [ghcp_cli_workflow_demo_kit](https://github.com/junwoojeong100/ghcp_cli_workflow_demo_kit) | Copilot CLI 맞춤 에이전트 7개와 Hook 으로 변경 요청 1건을 처리하는 데모 키트 (ShopFlow, 한국어·영어) |
| 1–5 영상 | [foundry-ghcp-demo-deck](https://github.com/junwoojeong100/foundry-ghcp-demo-deck) | Foundry × Copilot 데모 슬라이드 20장 + 화면 녹화 11개(6분 36초), 발표 노트 포함 |
| 6 | [microsoft-foundry-demo](https://github.com/junwoojeong100/microsoft-foundry-demo) | `azd up` 한 번으로 Contoso AI(Container Apps) + Foundry 배포, 관리자 화면은 포털로 시연 |
| 7 | [github-azure-eco](https://github.com/junwoojeong100/github-azure-eco) | Copilot 으로 코딩 → PR 검증 → GitHub Actions(OIDC) → ACA 새 리비전 |
| 8 | [aca-sandbox-labs](https://github.com/junwoojeong100/aca-sandbox-labs) | AI 워크스페이스가 신뢰할 수 없는 코드를 Dynamic Sessions · ACA Sandboxes 에서 격리 실행 |
| 9–10 | [aks-terraform](https://github.com/junwoojeong100/aks-terraform) | AWS 엔지니어를 위한 AKS + Terraform — Lab 00–11, HTML 가이드, 실제 실행 녹화 51분 56초 |
| 입문 | [aks-mini-labs](https://github.com/junwoojeong100/aks-mini-labs) | 컨테이너 기초 → AKS 실습 → CI/CD(Actions·Argo CD). Codespaces 로 바로 시작 |
