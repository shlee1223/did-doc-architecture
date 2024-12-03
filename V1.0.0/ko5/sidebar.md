- 아키텍처
  - [소프트웨어 아키텍처](/V1.0.0/docs/architecture/Software%20Architecture_ko.md)
- 컨셉
  - [JSON 직렬화](/V1.0.0/docs/concepts/JSON_serialization_ko.md)
  - [VP 제출](/V1.0.0/docs/concepts/Presentation%20of%20VP_ko.md)
  - [사용자 등록](/V1.0.0/docs/concepts/User%20Registration_ko.md)
  - [VC 발급](/V1.0.0/docs/concepts/VC%20Issuance_ko.md)
  - [블록체인 연동](/V1.0.0/docs/concepts/blockchain_access_ko.md)
  - [Open DID 구성도](/V1.0.0/docs/concepts/components_ko.md)
  - [Wallet 생명 주기](/V1.0.0/docs/concepts/life_cycle_ko.md)
  - [PII 관리](/V1.0.0/docs/concepts/manage_pii_ko.md)
  - [Open DID Token](/V1.0.0/docs/concepts/token_ko.md)
  - [월렛 설명](/V1.0.0/docs/concepts/wallet_ko.md)
  - [월렛 인터페이스](/V1.0.0/docs/concepts/wallet_interface_ko.md)
  - [월렛 잠금](/V1.0.0/docs/concepts/wallet_lock_policy_ko.md)
  - [월렛 정책](/V1.0.0/docs/concepts/wallet_policy_ko.md)
  - [월렛 소프트웨어 아키텍쳐](/V1.0.0/docs/concepts/wallet_sw_architecture_ko.md)
- 데이터 표준
  - 데이터 스펙
    - [데이터 명세서](/V1.0.0/docs/data%20standard/data%20specification/Data%20Specification_ko.md)
  - DID Document 포맷
    - [DID Document 포맷](/V1.0.0/docs/data%20standard/did%20document%20format/DID%20Document%20format_ko.md)
  - Verifiable Credential 포맷
    - [Profile 포맷](/V1.0.0/docs/data%20standard/verifiable%20credential%20format/Profile%20format_ko.md)
    - [VC Schema 포맷](/V1.0.0/docs/data%20standard/verifiable%20credential%20format/VC%20Schema%20format_ko.md)
    - [VC 포맷](/V1.0.0/docs/data%20standard/verifiable%20credential%20format/VC%20format_ko.md)
    - [VP 포맷](/V1.0.0/docs/data%20standard/verifiable%20credential%20format/VP%20format_ko.md)
- 가이드
  - API
    - [OpenDID API 문서 작성 가이드](/V1.0.0/docs/guide/api/API%20Documentation%20Writing%20Guide_ko.md)
  - 문서
    - [write_document_guide](/V1.0.0/docs/guide/docs/write_document_guide.md)
  - [용어집](/V1.0.0/docs/guide/glossary.md)
  - OSD
    - [OpenDID Schema Definition Language](/V1.0.0/docs/guide/osd/OpenDID%20Schema%20Definition%20Language_ko.md)
- 규약
  - [OpenDID 코드 적용 규약 참고 가이드](/V1.0.0/docs/rules/coding_style_ko.md)
  - [커밋 메시지 가이드라인](/V1.0.0/docs/rules/git_code_commit_rule_ko.md)
- 보안
  - [중간자 공격](/V1.0.0/docs/security/MitM_ko.md)
  - [인증 및 보안채널 생성](/V1.0.0/docs/security/authentication_ko.md)
- **OmniOne Open DID**
  - [GitHub Repository](https://github.com/OmniOneID)
  - [Community](https://opendid.omnione.net/community)

<script>
  function goToEnglishLanguage() {
    // 현재 URL을 가져옵니다.
    const currentUrl = window.location.href;
  
    // 현재 경로 (pathname)와 쿼리 문자열 (search) 분리
    const pathname = window.location.pathname;
    const search = window.location.search;

    // 쿼리 문자열에서 'ko'를 'en'으로 치환
    const newSearch = search.replace(/_ko/g, '').replace(/\/ko\//g, '\/en\/');
  
    // 새로운 URL을 생성 (기존의 프로토콜, 호스트, 경로, 쿼리 문자열을 모두 합침)
    const newUrl = window.location.origin + newPathname + newSearch + window.location.hash;
  
    // 만약 현재 URL과 새로 만든 URL이 다르면 리디렉션
    if (currentUrl !== newUrl) {
      window.location.href = newUrl;
    }
  }
</script>
<form onsubmit="return goToEnglishLanguage();" target="_blank">
  <input type="submit" value="Go to English Language" style="cursor: pointer;margin-top:12px;padding:6px;width:250px;background-color:#FFFFFF;border:1px solid #0374B5;border-radius:.25rem;color:#0374B5;display:inline-block;font-family:system-ui,sans-serif;text-align:center;text-decoration:none;font-size:16px;-webkit-text-size-adjust:none;mso-hide:all;" />
</form>