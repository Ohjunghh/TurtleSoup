# 🐢 바다거북 수프 추리 게임

---

## ✨ 개요

**바다거북 수프**는 제한된 정보 속에서 **예/아니오로 답할 수 있는 질문**을 통해 사건의 진실을 추리하는 게임입니다.  
이 프로젝트는 **Gradio**, **Ollama**, **EEVE-korean-10.8B LLM**을 활용하여 웹 환경에서 즐길 수 있도록 제작되었습니다.

---

## 🔧 기술 스택

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-FFB300?style=flat-square&logo=gradio&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square)

## 🔉 사용 LLM
![EEVE-korean-10.8B](https://img.shields.io/badge/EEVE--korean--10.8B-FF69B4?style=flat-square)

---

## 🎮 게임 설명

### 1. 시나리오 기반 추리 게임

- 출제자는 **이야기 형식의 수수께끼(시나리오)** 를 출제합니다.
- 참가자는 이야기의 전말을 알아내기 위해 **예/아니오로 대답 가능한 질문**을 던집니다.
- 질문을 통해 정보를 얻어 사건의 진실을 추리하고 정답을 유추해야 합니다.

### 2. 진행 방식

- 질문은 **최대 20회**까지 가능합니다.
- 정답은 **단 1회만 제출**할 수 있습니다.
- 힌트는 **최대 3회** 요청할 수 있습니다.
---

## 🧩 프롬프트 구조

- **질문**
  - 사용자 질문 → LLM 응답 (다음 중 하나):
    - `예`
    - `아니오`
    - `예/아니오로 대답할 수 없음`
    - `추리와 관련 없는 질문입니다`

- **정답 제출**
  - 사용자가 추리한 답을 입력하면, **의미 기반 비교**를 통해 정답 여부를 판단:
    - `정답입니다!`
    - `오답입니다.`

- **힌트 요청**
  - 사용자가 힌트를 요청하면, LLM이 **직접적인 정답 노출 없이도 본질에 가까운 힌트**를 1문장으로 제공

---

## 📽️ 시연 영상
![Image](https://github.com/user-attachments/assets/06063cf9-07c4-4882-a65f-0fd181609503)
