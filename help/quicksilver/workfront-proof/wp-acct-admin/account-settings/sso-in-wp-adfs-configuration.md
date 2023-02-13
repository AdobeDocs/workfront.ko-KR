---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: '단일 사인온 [!DNL Workfront Proof]: AD FS 구성'''
description: AD 서버의 관리자인 경우 AD FS를 설치 및 구성할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 단일 사인온 [!DNL Workfront Proof]: AD FS 구성

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

AD 서버의 관리자인 경우 AD FS를 설치 및 구성할 수 있습니다.

## AD FS 설치 및 구성

1. 다운로드 [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) 컴퓨터에 연결합니다.
1. 다운로드한 AdfsSetup.exe 파일을 열어 ADFS(Active Directory Federation Services) 설치 마법사를 시작합니다.
1. [서버 역할] 화면에서 옵션 중 하나를 선택합니다(최소 페더레이션 서버가 필요합니다.).
1. AD 서버의 IIS를 인터넷에 노출하지 않으려는 경우(HTTP와 HTTPS의 경우 포트 80 및 443) 먼저 방화벽 뒤에 페더레이션 서버를 설정한 다음 방화벽을 통해 요청을 페더레이션 서버로 전달하는 두 번째 페더레이션 서버 프록시를 빌드할 수 있습니다.
1. AD FS 설정을 완료하면 **[!UICONTROL AD FS 2.0 관리 스냅인을 시작합니다]**&#x200B;를 클릭한 다음 **[!UICONTROL 완료]**. 이 작업이 완료되면 AD FS 2.0 관리 창이 즉시 열립니다. 없는 경우 다음 위치에서 열 수 있습니다. **[!UICONTROL 시작]** > **[!UICONTROL 관리 도구]** > **[!UICONTROL AD FS 2.0 관리]**. AD FS 컨트롤 응용 프로그램입니다.

1. 먼저 AD FS 2.0 Federation Server 구성 마법사를 클릭합니다.
이렇게 하면 AD FS를 구성하고 IIS를 통해 인터넷 및 AD에 모두 연결할 수 있습니다.
1. 새 AD FS 서버를 구성하는 경우 **[!UICONTROL 새 페더레이션 서비스 만들기]**.
1. 선택 **[!UICONTROL 독립형 페더레이션 서버]** (테스트 및 평가 목적).

1. 고가용성 및 로드 밸런싱을 위해 새 페더레이션 서버 팜을 클릭합니다.
1. 페더레이션 서비스 이름을 지정합니다.
기본적으로 구성 마법사는 IIS의 기본 웹 사이트에 바인딩된 SSL 인증서를 검색하고 여기에 지정된 제목 이름을 사용합니다. 와일드카드 인증서를 사용하는 경우 페더레이션 서비스 이름을 입력해야 합니다.
IIS에 구성된 SSL 인증서가 없으면 구성 마법사는 로컬 컴퓨터 인증서 저장소에서 유효한 인증서를 검색합니다. SSL 인증서 드롭다운에 표시됩니다. 인증서가 없으면 IIS의 서버 인증서 생성기를 사용하여 인증서를 만들 수 있습니다.

1. 구성을 계속 진행하고 을 클릭합니다. **[!UICONTROL 닫기]** 완료되면

## 구성 [!DNL Workfront Proof] 단일 사인온

만약 [!DNL Workfront Proof] 관리자는 [!DNL Workfront Proof] 합니다. 자세한 내용은 [단일 사인온 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**&#x200B;를 열고 **[!UICONTROL 단일 사인온]** 탭.

1. 에서 **SSO URL** 상자에 엔티티 ID를 붙여넣습니다.
다음은 엔티티 ID의 예입니다. http://*&lt;adfs.your-company.com>*/adfs/services/trust 엔티티 ID가 페더레이션 메타데이터 XML 파일에 있습니다.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. 페더레이션 메타데이터는 AD FS 2.0 스냅인 > 서비스 > 끝점 폴더에 있습니다. 메타데이터 섹션에서 페더레이션 메타데이터 유형을 사용하는 메타데이터를 찾습니다. 메타데이터를 보려면 이 엔드포인트를 브라우저에 붙여 넣습니다. 다음 링크로 직접 이동할 수도 있습니다. https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml {adfs.your-company.com}을(를) 사용자 고유의 세부 정보로 바꾼 후
1. 에서 **[!UICONTROL 로그인 URL]** 상자에 SSO 로그인을 붙여 넣습니다.
1. 다음은 SSO 로그인의 예입니다.
1. http://*&lt;adfs.your-company.com>*/adfs/ls
1. 이 링크는 페더레이션 메타데이터 XML 파일에 있습니다.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. 에서 **[!UICONTROL 로그아웃 URL]** 상자에 링크를 입력하고 저장합니다.
다음은 로그아웃 URL의 예입니다. https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. AD FS 관리자 > 트러스트 관계 > 신뢰 당사자 트러스트 - ProofHQ 속성으로 이동합니다.
   1. 엔드포인트에서 [!UICONTROL 및 항목 추가] 다음 세부 사항을 참조하십시오.

      * 끝점 유형 = SAML 로그아웃
      * 바인딩 = POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * AD FS에서 신뢰 당사자 트러스트를 구성한 후 이 단계를 완료할 수 있습니다(아래 참조).
   1. 에서 **[!UICONTROL 인증서 지문]** 상자에 인증서의 데이터를 입력합니다.
   1. ADFS 2.0 스냅인으로 이동하여 서비스 > 인증서 > 토큰 서명으로 이동합니다.
   1. 인증서를 보려면 이 항목을 마우스 오른쪽 단추로 클릭하십시오.
   1. 에서 [!UICONTROL 인증서 세부 정보] Tab 키를 눌러 Thumbprint를 복사한 다음 **[!UICONTROL Workfront 증명 단일 사인온]** 구성 탭.

   1. 지문 문자는 콜론 또는 공백으로 분리할 수 있지만 제거하는 것이 좋습니다. 단일 사인온 구성에 문제가 있는 경우 고객 지원 팀에 문의하십시오.


## 신뢰 당사자 트러스트 추가

구성이 완료되면 AD FS의 신뢰 당사자 트러스트 섹션에서 작업해야 합니다.

1. 다음으로 이동 **[!UICONTROL 신뢰 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]** 폴더를 클릭한 다음 **[!UICONTROL 신뢰 당사자 트러스트 추가]** 구성 마법사를 시작하려면 다음을 수행하십시오.

1. 데이터 소스를 선택합니다.
사용자의 모든 메타데이터 [!DNL ProofHQ] 계정은 다음과 같은 링크 아래에 있습니다. https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq 이 옵션을 사용하면 대부분의 신뢰 당사자 트러스트를 구성합니다.

   >[!NOTE]
   >
   >* URL에서 연결을 설정하는 데 문제가 있는 경우 메타데이터를 파일로 저장하고 파일에서 데이터를 가져오도록 선택합니다.
   >* 사용자 지정 도메인(예: www.your-proofing.com)이 [!DNL ProofHQ] 계정을 사용하여 &quot;{yoursubdomain}.proohq.com&quot; 전체 부분을 고유한 도메인으로 바꿉니다 [!DNL ProofHQ] 메타데이터 링크.



## 클레임 규칙 구성

신뢰 당사자 트러스트 구성이 완료되면 설정을 완료하도록 클레임 규칙을 구성할 수 있습니다. ProofHQ에 대해 두 가지 클레임 규칙을 구성합니다. 이메일 및 이름 ID.

1. 를 엽니다. **[!UICONTROL 클레임 규칙 편집]** 대화 상자
1. 이동 **[!UICONTROL ProofHQ 신뢰 당사자 트러스트]**&#x200B;를 클릭한 다음 **[!UICONTROL 클레임 규칙 편집]** (1).\
   신뢰 구성 종료 시 이 옵션을 선택한 경우 팝업이 자동으로 열립니다.

1. 클릭 **[!UICONTROL 규칙 추가]** (2) 청구구성창을 엽니다.

   * 전자 메일(LDAP 속성을 클레임 규칙 템플릿으로 전송)
   * NameID(들어오는 클레임 규칙 템플릿 변환)
