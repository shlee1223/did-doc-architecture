# OmniOne Open DID 강의 시리즈
> OmniOne Open DID를 쉽게 이해할 수 있도록 강의 시리즈를 준비했습니다.<br>
> 이 시리즈는 DID는 물론 Open DID에 대한 전반적인 이해를 위해 많은 도움이 될 것입니다.

---

목차
--
- [OmniOne Open DID 강의 시리즈 : 입문자용](#omnione-open-did-강의-시리즈--입문자용)
  - [1강. DID 기초 소개](#1강-did-기초-소개)
  - [2강. Open DID 플랫폼 구성요소](#2강-open-did-플랫폼-구성요소)
  - [3강. Open DID 신뢰환경](#3강-open-did-신뢰환경)
  - [4강. 사용자 등록](#4강-사용자-등록)
  - [5강. VC 발급](#5강-vc-발급)
  - [6강. VP 제출](#6강-vp-제출)
  - [부록. Open DID GitHub Repository 구성 및 소개](#부록-open-did-github-repository-구성-및-소개)
- [OmniOne Open DID 강의 시리즈 : 실습 튜토리얼](#omnione-open-did-강의-시리즈--실습-튜토리얼)
  - [1강. Open DID 실습 교육 개요](#1강-open-did-실습-교육-개요)
  - [2-1강. Open DID 서버 설치 (Orchestrator)](#2-1강-open-did-서버-설치-orchestrator)
  - [2-2강. Open DID 서버 설치 (Gradle)](#2-2강-open-did-서버-설치-gradle)
  - [2-3강. Open DID 서버 설치 (IDE)](#2-3강-open-did-서버-설치-ide)
  - [2-4강. Open DID 서버 설치 (Docker)](#2-4강-open-did-서버-설치-docker)
- [더 많은 강의가 곧 공개됩니다...]

<br>

## OmniOne Open DID 강의 시리즈 : 입문자용

---

### 1강. DID 기초 소개
<iframe width="450" height="250" src="https://www.youtube.com/embed/98qFzeEC55Y?si=G1pjU8XJhwWeRb36" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

이 영상은 DID(Decentralized Identifier)의 기본 개념을 이해하는데 도움을 줍니다.

📚 **이번 강의에서 다루는 내용**
- DID(Decentralized Identifier)와 DID Document
- VC(Verifiable Credential)와 VP(Verifiable Presentation)
- 월렛(Wallet)과 ZKP(Zero-Knowledge Proof)
- DID·VC·VP의 관계와 활용 흐름
- Blockchain의 역할과 Issuer·Holder·Verifier 구조

---

### 2강. Open DID 플랫폼 구성요소
<iframe width="450" height="250" src="https://www.youtube.com/embed/06J0Bptnt9A?si=Uii23XyUHxXPCj80" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

이 영상은 Open DID 플랫폼 구성요소를 이해하는데 도움을 줍니다.

📚 **이번 강의에서 다루는 내용**
- Open DID 개요 및 특징
- Open DID 구성요소 개념
- Open DID 기본 구성요소(Ledger, Server, Client)
- Open DID 전체 구성요소(TAS, Issuer, Verifier 등)
- Open DID 전체 흐름(5단계)

---

### 3강. Open DID 신뢰환경
<iframe width="450" height="250" src="https://www.youtube.com/embed/FA3lEZNU_lw?si=a8Egc5Bi6TxeuefN" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

이 영상은 Open DID 신뢰환경을 이해하는데 도움을 줍니다.

📚 **이번 강의에서 다루는 내용**
- Open DID 신뢰환경 개요
- Open DID 신뢰환경 아키텍처
- Open DID 신뢰환경 핵심요소
- Open DID 신뢰환경 구축 절차
- Open DID 보안요소

---

### 4강. 사용자 등록
<iframe width="450" height="250" src="https://www.youtube.com/embed/mHeJMnLwZMY?si=NG9FuSra_bZHq08A" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

이 영상은 Open DID 사용자 등록을 이해하는데 도움을 줍니다.

📚 **이번 강의에서 다루는 내용**
- Open DID 사용자 등록 개요
- Open DID 사용자 등록 관련 개념 복습
- Open DID 월렛 등록 절차
- Open DID 사용자 등록 절차

---

### 5강. VC 발급
<iframe width="450" height="250" src="https://www.youtube.com/embed/aIX_6uo4y_8?si=t_HXHPbBRLqhTJfl" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

이 영상은 Open DID VC 발급의 개념 및 절차를 이해하는데 도움을 줍니다.

📚 **이번 강의에서 다루는 내용**
- Open DID VC 발급 개요
- Open DID VC 발급 관련 개념 복습
- Open DID VC 발급 절차
- Open DID VC 발급 관련 실 사용 사례

---

### 6강. VP 제출
<iframe width="450" height="250" src="https://www.youtube.com/embed/w0ddiJ4vMhU?si=C1kRMbezMsaCtc74" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

이 영상은 Open DID VP 제출의 개념 및 절차를 이해하는데 도움을 줍니다.

📚 **이번 강의에서 다루는 내용**
- Open DID VP 제출 개요
- Open DID VP 제출 관련 개념 복습
- Open DID VP 제출 절차
- Open DID VP 제출 관련 실 사용 사례

---

### 부록. Open DID GitHub Repository 구성 및 소개
<iframe width="450" height="250" src="https://www.youtube.com/embed/6dSL28uKgGk?si=kTlo9VkASK7Er9-e" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

이 영상은 Open DID GitHub Repository의 전체 구조를 이해하는데 도움을 줍니다.

📚 **이번 강의에서 다루는 내용**
- Open DID GitHub Repository 구성 개요
- Open DID GitHub Repository 구성 - Server
- Open DID GitHub Repository 구성 - Mobile
- Open DID GitHub Repository 구성 - Document
- Open DID GitHub Repository 전체 구성

<br>

## OmniOne Open DID 강의 시리즈 : 실습 튜토리얼

---

### 1강. Open DID 실습 교육 개요
<iframe width="450" height="250" src="https://www.youtube.com/embed/00xW3fn0RBQ?si=pYFh0kstyYpVGnnH" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

OpenDID 실습 교육의 전체 흐름과 학습 목표를 소개합니다.

📚 **이번 강의에서 다루는 내용**
- OpenDID 실습 전체 흐름 이해
- User 등록 → VC 발급 → VP 제출 최종 결과 소개
- OpenDID 아키텍처 구성 요소 및 역할
- DID, VC, VP 등 핵심 용어 정리
- 설치 방식(Orchestrator/Gradle/IDE/Docker) 선택 안내

⚠️ 본 강의는 Open DID 릴리즈 버전 2.0.0.0 버전 기준입니다.

---

### 2-1강. Open DID 서버 설치 (Orchestrator)
<iframe width="450" height="250" src="https://www.youtube.com/embed/B3MuPBrrddE?si=WfNkEK6zqyGYgKb9" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

Orchestrator를 이용한 서버 설치 방법을 실습합니다.

📚 **이번 강의에서 다루는 내용**
- Orchestrator 기반 Open DID 서버 구성
- 서버 설치 및 기본 설정 절차
- 서버 구동 및 상태 확인
- 실습에 필요한 사전 환경 점검

⚠️ 본 강의는 Open DID 릴리즈 버전 2.0.0.0 버전 기준입니다.

---

### 2-2강. Open DID 서버 설치 (Gradle)
<iframe width="450" height="250" src="https://www.youtube.com/embed/Gsd_rgnVO4I?si=8ypT8rp6aQsS2VdM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

Gradle 빌드를 통해 직접 서버를 설치하고 구동하는 방법을 실습합니다.

📚 **이번 강의에서 다루는 내용**
- Gradle 기반 서버 설치 개요
- 프로젝트 폴더 구조 및 설정 파일 이해
- Gradle 빌드 및 서버 실행
- 서버 구동 결과 확인

⚠️ 본 강의는 Open DID 릴리즈 버전 2.0.0.0 버전 기준입니다.

---

### 2-3강. Open DID 서버 설치 (IDE)
<iframe width="450" height="250" src="https://www.youtube.com/embed/wEXOBSXu6Is?si=myfQcn1psy636FsO" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

IntelliJ IDEA를 활용해 개발 환경에서 서버를 설치하고 실행하는 방법을 실습합니다.

📚 **이번 강의에서 다루는 내용**
- IDE 기반 서버 실행 환경 구성
- 프로젝트 구조 및 설정 파일 확인
- IDE 빌드 및 서버 실행
- 실행 결과 및 로그 확인

⚠️ 본 강의는 Open DID 릴리즈 버전 2.0.0.0 버전 기준입니다.

---

### 2-4강. Open DID 서버 설치 (Docker)
<iframe width="450" height="250" src="https://www.youtube.com/embed/pTwI3pzldS4?si=ZpoC0jEcxk-vpLda" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="padding-right: 100px;"></iframe>

Docker 컨테이너 기반으로 서버를 구성하는 방법을 실습합니다.

📚 **이번 강의에서 다루는 내용**
- Docker 기반 서버 구성 개요
- Docker Image 생성 방법
- Docker Compose를 이용한 서버 실행
- 컨테이너 상태 및 로그 확인

⚠️ 본 강의는 Open DID 릴리즈 버전 2.0.0.0 버전 기준입니다.

---
