---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: ' [!DNL Workfront Proof]의 SSO(Single Sign-On): AD FS 구성'
description: AD 서버의 관리자인 경우 AD FS를 설치하고 구성할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: 690b0817dfe4ff200982ffe8d67ad93e563e30ac
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# [!DNL Workfront Proof]의 SSO(Single Sign-On): AD FS 구성

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

AD 서버의 관리자인 경우 AD FS를 설치하고 구성할 수 있습니다.

## AD FS 설치 및 구성

1. 컴퓨터에 Microsoft AD FS 2.0을 다운로드합니다.
1. 다운로드한 AdfsSetup.exe 파일을 열어 ADFS(Active Directory Federation Services) 설치 마법사를 시작합니다.
1. 서버 역할 화면에서 옵션 중 하나를 선택합니다(최소 페더레이션 서버가 필요).
1. AD 서버의 IIS를 인터넷(HTTP 및 HTTPS의 경우 포트 80 및 443)에 노출하지 않으려면 먼저 방화벽 뒤에 페더레이션 서버를 설정한 다음 방화벽을 통해 페더레이션 서버로 요청을 전달하는 두 번째 페더레이션 서버 프록시를 빌드할 수 있습니다.
1. AD FS 설정을 완료했으면 **[!UICONTROL AD FS 2.0 관리 스냅인 시작]**&#x200B;을 선택한 다음 **[!UICONTROL 마침]**&#x200B;을 클릭합니다. 완료되면 AD FS 2.0 관리 창이 바로 열립니다. 그렇지 않으면 **[!UICONTROL 시작]** > **[!UICONTROL 관리 도구]** > **[!UICONTROL AD FS 2.0 관리]**&#x200B;에서 열 수 있습니다. 이는 기본 AD FS 컨트롤 응용 프로그램입니다.

1. AD FS 2.0 페더레이션 서버 구성 마법사를 클릭하여 시작합니다.
이렇게 하면 AD FS를 구성하고 IIS를 통해 인터넷에 연결하고 AD에 연결하는 데 도움이 됩니다.
1. 새 AD FS 서버를 구성하는 경우 **[!UICONTROL 새 페더레이션 서비스 만들기]**&#x200B;를 선택하십시오.
1. 테스트 및 평가 목적으로 **[!UICONTROL 독립 실행형 페더레이션 서버]**&#x200B;를 선택하십시오.

1. 고가용성 및 로드 밸런싱을 사용하려면 새 페더레이션 서버 팜을 클릭합니다.
1. 페더레이션 서비스 이름을 지정하십시오.
기본적으로 구성 마법사는 IIS의 기본 웹 사이트에 바인딩된 SSL 인증서를 검색하고 여기에 지정된 주체 이름을 사용합니다. 와일드카드 인증서를 사용하는 경우 페더레이션 서비스 이름을 입력해야 합니다.
IIS에 구성된 SSL 인증서가 없으면 구성 마법사가 로컬 컴퓨터 인증서 저장소에서 유효한 인증서를 검색합니다. SSL 인증서 드롭다운에 표시됩니다. 인증서가 없으면 IIS의 서버 인증서 생성기를 사용하여 인증서를 만들 수 있습니다.

1. 구성을 계속하고 완료되면 **[!UICONTROL 닫기]**&#x200B;를 클릭하십시오.

## [!DNL Workfront Proof] Single Sign-On 구성 중

[!DNL Workfront Proof] 관리자인 경우 [!DNL Workfront Proof]측에서 Single Sign-On을 구성할 수 있습니다. 자세한 내용은 [Single Sign-On in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md)을 참조하세요.

1. **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**&#x200B;을 클릭한 다음 **[!UICONTROL Single Sign-On]** 탭을 엽니다.

1. **SSO URL** 상자에 엔티티 ID를 붙여 넣으십시오.
다음은 엔티티 ID의 예입니다.
http://*&lt;adfs.your-company.com>*/adfs/services/trust
엔티티 ID는 페더레이션 메타데이터 XML 파일에서 찾을 수 있습니다.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. 페더레이션 메타데이터는 AD FS 2.0 스냅인 > 서비스 > 끝점 폴더에 있습니다. 메타데이터 섹션에서 페더레이션 메타데이터 유형이 있는 메타데이터 섹션을 찾습니다. 메타데이터를 보려면 이 끝점을 브라우저에 붙여 넣습니다. {adfs.your-company.com}을(를) 자신의 세부 정보로 바꾼 후 https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml 링크로 직접 이동할 수도 있습니다.
1. **[!UICONTROL 로그인 URL]** 상자에 SSO 로그인을 붙여 넣으십시오.
1. 다음은 SSO 로그인의 예입니다.
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. 이 링크는 페더레이션 메타데이터 XML 파일에서 찾을 수 있습니다.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. **[!UICONTROL 로그아웃 URL]** 상자에 링크를 입력하고 저장합니다.
다음은 로그아웃 URL의 예입니다.
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. AD FS 관리자 > 트러스트 관계 > 신뢰 당사자 트러스트 - ProofHQ 속성으로 이동합니다.
   1. 끝점 아래에 있는 [!UICONTROL 추가 및 항목]을(를) 클릭합니다. 자세한 내용은 다음과 같습니다.

      * 끝점 유형 = SAML 로그아웃
      * 바인딩 = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * 이 단계는 AD FS에서 신뢰 당사자 트러스트(아래 참조)를 구성한 후에 완료할 수 있습니다.
   1. **[!UICONTROL 인증서 지문]** 상자에 인증서의 데이터를 입력합니다.
   1. ADFS 2.0 스냅인으로 이동하여 서비스 > 인증서 > 토큰 서명으로 이동합니다.
   1. 인증서를 보려면 이 항목을 마우스 오른쪽 버튼으로 클릭하십시오.
   1. [!UICONTROL 인증서 세부 정보] 탭에서 지문을 복사하여 **[!UICONTROL Workfront Proof Single Sign-On]** 구성 탭에 붙여넣습니다.

   1. 지문 문자는 콜론 또는 공백으로 구분할 수 있지만 이러한 문자는 제거하는 것이 좋습니다. SSO(Single Sign-On) 구성에 문제가 있으면 고객 지원 팀에 문의하십시오.


## 신뢰 당사자 트러스트 추가

구성이 완료되면 AD FS의 신뢰 당사자 트러스트 섹션에서 작업해야 합니다.

1. **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]** 폴더로 이동한 다음 **[!UICONTROL 신뢰 당사자 트러스트 추가]**&#x200B;를 클릭하여 구성 마법사를 시작합니다.

1. 데이터 소스를 선택합니다.
[!DNL ProofHQ] 계정의 모든 메타데이터는 다음과 같은 링크 아래에 있습니다.
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
신뢰 당사자 트러스트 대부분을 구성합니다.

   >[!NOTE]
   >
   >* URL에서 연결을 설정하는 데 문제가 있는 경우 메타데이터를 파일로 저장하고 파일에서 데이터를 가져오도록 선택합니다.
   >* [!DNL ProofHQ] 계정에 전체 사용자 지정 도메인(예: www.your-proofing.com)이 구성된 경우 전체 &quot;{yoursubdomain}.proofhq.com&quot; 부분을 고유한 도메인으로 교체하여 [!DNL ProofHQ] 메타데이터 링크를 만듭니다.


## 클레임 규칙 구성

신뢰 당사자 트러스트 구성이 완료되면 설정을 완료하도록 클레임 규칙을 구성할 준비가 되었습니다. ProofHQ에 대한 두 가지 클레임 규칙(전자 메일 및 이름 ID)을 구성합니다.

1. **[!UICONTROL 클레임 규칙 편집]** 대화 상자를 엽니다.
1. **[!UICONTROL ProofHQ 신뢰 당사자 트러스트]**(으)로 이동한 다음 **[!UICONTROL 클레임 규칙 편집]**(1)을 클릭합니다.\
   트러스트 구성이 끝난 후 이 옵션을 선택한 경우 팝업이 자동으로 열립니다.

1. **[!UICONTROL 규칙 추가]**(2)를 클릭하여 클레임 구성 창을 엽니다.

   * 전자 메일(LDAP 속성을 클레임 규칙 템플릿으로 보내기)
   * NameID(들어오는 클레임 규칙 템플릿 변환)
