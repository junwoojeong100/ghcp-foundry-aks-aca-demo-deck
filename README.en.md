# GitHub Copilot × Microsoft Foundry × ACA · AKS — AI app development & operations, in demos

A demo-first deck (**21 slides**). It shows the whole journey — build (GitHub Copilot), add intelligence (Microsoft Foundry), deploy and operate (Azure Container Apps · AKS) — not with slides but with **real running screens and validation records**. The slides embed **7 screen-recording videos** (about 4 min 50 s in total) and carry English speaker notes. (한국어판: [README.md](README.md))

## Open in the browser — no download

| | |
| --- | --- |
| **Slides — English** (21 slides, 7 videos embedded) | [📑 Open in the browser](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fjunwoojeong100.github.io%2Fghcp-foundry-aks-aca-demo-deck%2FGitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_EN.pptx) |
| **PPTX — English** | [⬇ GitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_EN.pptx](https://junwoojeong100.github.io/ghcp-foundry-aks-aca-demo-deck/GitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_EN.pptx) (about 32 MB) |
| Korean edition | [📑 Slides](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fjunwoojeong100.github.io%2Fghcp-foundry-aks-aca-demo-deck%2FGitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_KO.pptx) · [⬇ PPTX](https://junwoojeong100.github.io/ghcp-foundry-aks-aca-demo-deck/GitHub_Copilot_Foundry_ACA_AKS_Demo_Deck_KO.pptx) (about 32 MB) |

The slides open in Microsoft's PowerPoint for the web. Click ▶ on a video to play it; open **Notes** at the bottom right for the speaker notes and **Start Slide Show** for full-screen presenting. Because the videos are embedded the file is large, so the first load can take a while. The web viewer uses its own fonts, so line breaks can differ slightly from desktop PowerPoint — download the PPTX to see the exact layout.

## The 10 demos

| # | Area | Demo | Format | Slide |
| --- | --- | --- | --- | --- |
| 1 | GitHub Copilot | Build & test — 26 → 100 tests | ▶ Video | 5 |
| 2 | GitHub Copilot | Safeguard — a Hook blocks the violation | ▶ Video | 6 |
| 3 | Microsoft Foundry | Agent + documents — cites evidence and sources | ▶ Video | 8 |
| 4 | Microsoft Foundry | Guardrails — jailbreak blocked at the door | ▶ Video | 9 |
| 5 | Microsoft Foundry | Evaluations — automatic quality & safety scoring | ▶ Video | 10 |
| 6 | Azure Container Apps | One `azd up` — Foundry and the app | ▶ Video | 12 |
| 7 | Azure Container Apps | Actions → new revision — OIDC · no secrets | ◆ Validation record | 13 |
| 8 | Azure Container Apps | AI code sandbox — isolate · inspect · approve | ◆ Validation record | 14 |
| 9 | AKS | Terraform → AKS — real Azure · 3 nodes Ready | ▶ Video | 16 |
| 10 | AKS | kubectl · Portal — verified up to HTTP 200 | ■ Verification screens | 17 |

- **▶ Video** Real screen/run recordings. No sound; waits are cut or sped up.
- **◆ Validation record** No video — a slide summarizing the real deployment and validation results and the commands used. Demo 7 ran on 2026-07-21 and demo 8 on 2026-07-24~29, so these are past records; re-check current behavior before demoing.
- **■ Verification screens** Still captures from a real run.

> Models and features on screen vary by subscription, region and time. ACA Sandboxes in demo 8 was in Preview when this deck was written (2026-11). The durations and counts on the slides are single measured runs/records of each demo and are not meant for direct comparison with each other.

## About the English edition

- Same 21 slides and structure as the Korean edition; slide text and speaker notes are translated.
- **Demos 1–5 are English re-recordings.** The Copilot CLI session (demos 1–2) and the Foundry portal session (demos 3–5, sample questions and answers included) come from the English edition of [foundry-ghcp-demo-deck](https://github.com/junwoojeong100/foundry-ghcp-demo-deck), so everything on screen is English. Their figures come from those English runs and differ slightly from the Korean edition — for example the Copilot run (38.0 min, tests 26 → 100) and the Foundry evaluation (about 4.5 min).
- Demos 6 and 9 are the original recordings (`azd up`, Terraform → AKS); **only the production overlays (captions, speed badges, step panel) were replaced with English**. Demos 7, 8 and 10 are validation records and screens.
- Font: Aptos (included with Microsoft 365).

## Sources · more

The originals of the videos and validation records are all public repositories of [junwoojeong100](https://github.com/junwoojeong100).

| Demo | Repository | What it is |
| --- | --- | --- |
| 1–2 | [ghcp_cli_workflow_demo_kit](https://github.com/junwoojeong100/ghcp_cli_workflow_demo_kit) | A demo kit that handles one change request with 7 Copilot CLI custom agents and Hooks (ShopFlow, Korean and English) |
| 1–5 videos | [foundry-ghcp-demo-deck](https://github.com/junwoojeong100/foundry-ghcp-demo-deck) | Foundry × Copilot demo deck: 20 slides + 11 screen recordings (7 min 1 s), with speaker notes — English edition |
| 6 | [microsoft-foundry-demo](https://github.com/junwoojeong100/microsoft-foundry-demo) | Deploy Contoso AI (Container Apps) + Foundry with one `azd up`; admin screens are shown in the portal |
| 7 | [github-azure-eco](https://github.com/junwoojeong100/github-azure-eco) | Code with Copilot → PR validation → GitHub Actions (OIDC) → new ACA revision |
| 8 | [aca-sandbox-labs](https://github.com/junwoojeong100/aca-sandbox-labs) | An AI workspace runs untrusted code in isolation on Dynamic Sessions · ACA Sandboxes |
| 9–10 | [aks-terraform](https://github.com/junwoojeong100/aks-terraform) | AKS + Terraform for AWS engineers — Labs 00–11, HTML guide, 51 min 56 s real-run recording |
| Intro | [aks-mini-labs](https://github.com/junwoojeong100/aks-mini-labs) | Container basics → AKS labs → CI/CD (Actions · Argo CD). Start right away in Codespaces |
