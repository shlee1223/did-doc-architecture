<!-- Individual documents may be merged in the future, so the table of contents is not used. -->

# Wallet SW Archtecture
CA(Certified App)는 신뢰 가능한 월랫 기능을 제공하기 위해서 유저 등록, VC 발급, VP 제출 등 WalletAPI, Utility, Communication, DataModel SDK를 참조하여 각 프로토콜 별 기능을 구현할 수 있다.

아래 각 기능에 대한 자세한 내용은 프로토콜 문서(경로…)를 참고한다.

1. 유저 등록 프로토콜
2. VC 발급 프로토콜
3. VP 제출 프로토콜

![wallet_sw_archetecture](./images/wallet_sw_architecture.svg)

### 1. SDK 설명
상기 SDK구조는 OpenDID의 클라이언트의 인가앱과 월랫 소프트웨어 관계 구조도이며 아래는 각 SDK별 대표 클래스를 설명한다.


| SDK Group          | Classes          | Features                                                       |
|---------------------|------------------|----------------------------------------------------------------|
| WalletAPI SDK       | WalletService     | - 유저 등록, VC발급, VP 제출 비즈니스 로직 처리<br>- 서명 값을 이용한 Proof 생성 |
|                     | WalletCore        | - key, DID/VC, VP 생성<br>- sign                             |
|                     | LockManager       | - Wallet 타입 및 상태 변경                                   |
|                     | WalletToken       | - walletToken 생성, 검증                                      |
|                     | DBManager         | - User정보, WalletToken, CA list 관리                        |
| CoreWallet SDK      | KeyManager        | - 사용자 키 생성, 인증, 서명                                  |
|                     | DIDManager        | - DIDDocument 생성 관리                                       |
|                     | VCManager         | - VC 생성 관리                                               |
| Communication SDK   | NetworkClient     | - CA와 Wallet 공통 통신 모듈                                  |
| Utility SDK         | DigestUtils       | - hash 공통 유틸                                             |
|                     | MultibaseUtils    | - 인/디코딩 공통 유틸                                        |
|                     | CryptoUtils       | - 랜덤값 및 키쌍 생성, 암/복호화 공통 유틸                  |
| DataModel SDK       | VO Objects        | - 데이터 포맷 및 직렬화/역직렬화                              |
| CA SDK              | URLScheme         | - 단독 Wallet과 연결                                          |
|                     | CAUtils           | - 월렛과 TAS 접근 Token 생성<br>- 세션키 생성               |

<br>
