---
title: ' [!DNL Workfront] 기존 커넥터로  [!DNL Adobe Experience Manager] 구성'
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: ' [!DNL Adobe Workfront] 관리자는  [!DNL Workfront] Adobe Experience Manager(AEM) Assets을 통합하고, 조직에서 워크플로우 내의 에셋을 생성, 공유 및 유지 관리할 수 있는 포괄적인 콘텐츠 관리 솔루션을 제공할 수 있습니다.'
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '1855'
ht-degree: 0%

---

# [!DNL Workfront] 레거시 커넥터로 [!DNL Adobe Experience Manager] 구성

<!-- Audited: 4/2025 -->

[!DNL Adobe Workfront] 관리자는 [!DNL Workfront]을(를) [!UICONTROL Adobe Experience Manager(AEM) Assets]과(와) 통합하고, 조직에서 워크플로우 내의 자산 생성, 공유 및 유지 관리를 위한 포괄적인 콘텐츠 관리 솔루션을 제공할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table>
  <tr>
   <td>Adobe Workfront 패키지
   </td>
   <td> <p>Prime 또는 Ultimate</p>
    <p>워크플로 얼티밋</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront 라이선스
   </td>
   <td><p>표준</p>
   <p>플랜</p>
   </td>
  </tr>
   <tr>
   <td>액세스 수준 구성
   </td>
   <td>[!DNL Workfront] 관리자여야 합니다.
   </td>
  </tr>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## [!DNL Workfront for AEM Assets]

[!DNL Workfront for AEM Assets connector]을(를) 사용하면 조직에서 다음을 수행할 수 있습니다.

* AEM 에셋 및 폴더를 [!DNL Workfront]의 프로젝트, 작업, 문제 및 요청에 연결하여 크리에이티브 콘텐츠를 공동 작업하고 관리합니다.

  타사 응용 프로그램과의 문서 통합 구성에 대한 자세한 내용은 [문서 통합 구성](../../administration-and-setup/configure-integrations/configure-document-integrations.md)을 참조하십시오.

* [!DNL AEM Digital Asset Managemen]t(DAM) 리포지토리와 통합하여 [!DNL Workfront]을(를) 사용하여 DAM에 저장된 디지털 에셋을 관리하고 공유할 수 있습니다.

  문서 및 에셋 폴더 연결에 대한 자세한 내용은   [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* 두 애플리케이션의 메타데이터를 결합하고 에셋에 적용합니다.
* 자산에 대한 모든 것을 포함하는 통신 스트림을 봅니다. [!DNL Workfront] 또는 [!UICONTROL AEM Assets]에서 자산에 대한 업데이트 및 댓글이 다른 응용 프로그램과 동기화되어 자산에 대한 포괄적인 통신 기록을 수립합니다.

  [!DNL Workfront]에서 댓글을 작성하는 방법에 대한 자세한 내용은 [문서에 업데이트 추가](../../documents/managing-documents/add-update-documents.md)를 참조하십시오.

## [!DNL AEM Assets] 커넥터를 설치하기 위한 필수 구성 요소

[!DNL Workfront]AEM Assets[!UICONTROL 용 &#x200B;] 커넥터를 설치하려면 먼저 다음 필수 구성 요소를 충족하는지 확인하십시오.

* [!UICONTROL AEM Assets]이(가) 설치 및 구성되었습니다. 버전 6.5 이상 [!UICONTROL AEM Assets] 설치에 대한 자세한 내용은 [[!DNL Adobe Experience Manager] 설명서](https://experienceleague.adobe.com/en/docs/experience-manager)를 참조하세요.
* (조건부) 방화벽 규칙이 예상대로 트래픽을 허용하지 않는 경우 클러스터의 IP 주소 및/또는 도메인을 허용 목록에 추가하다에 추가하십시오. 허용 목록에 추가하다 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

## [!DNL Workfront for AEM Assets] 커넥터 패키지 설치 {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>다음 지침은 [!DNL Workfront with AEM Assets]향상된 커넥터[[!DNL Workfront for Experience Manager] 로 대체된 &#x200B;](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md) 레거시 커넥터에 대한 것입니다. 자세한 내용은 계정 담당자에게 문의하십시오.

[!DNL Workfront for AEM Assets] 커넥터를 설치하려면 [!UICONTROL CRX 패키지 관리자]를 사용하여 커넥터를 패키지로 AEM에 가져와야 합니다.

1. 이미 AEM을 설치한 워크스테이션에서 [!DNL Workfront for AEM Assets] Connector 설치 파일을 다운로드합니다.

   [!DNL Workfront for AEM Assets] 담당자로부터 [!DNL Workfront] 커넥터를 가져올 수 있습니다.

1. 관리자 계정을 사용하여 AEM에 로그인합니다.
1. **[!UICONTROL 도구]** > **[!UICONTROL 배포]** > **[!UICONTROL 패키지]**&#x200B;를 클릭합니다. [!UICONTROL CRX 패키지 관리자]가 열립니다.

1. **[!UICONTROL 패키지 업로드].** 클릭

1. **[!UICONTROL 패키지 업로드]** 대화 상자에서 **[!UICONTROL Workfront 커넥터]** 패키지를 찾아 선택한 다음 **[!UICONTROL 확인]**&#x200B;을 클릭합니다. 패키지가 [!UICONTROL CRX 패키지 관리자]에 표시됩니다.

1. **[!UICONTROL 설치].** 클릭

1. **[!UICONTROL 패키지]** 대화 상자에서 고급 설정을 무시하고 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.
1. (선택 사항) 커넥터가 성공적으로 설치되었는지 확인하려면 [!UICONTROL 활동 로그]에 다음 문이 표시되는지 확인하십시오.

   ```
   Package installed in <time>
   ```

1. [!UICONTROL CRX 패키지 관리자]를 닫습니다. 커넥터가 설치되어 있으므로 [!DNL AEM Assets]을(를) [!DNL Workfront]과(와) 통합하도록 구성할 수 있습니다.

1. [과(와) 통합하려면  [!DNL AEM Assets] 구성 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)을(를) 계속합니다.

## [!DNL AEM Assets]과(와) 통합하도록 [!DNL Workfront] 구성 {#configure-aem-assets-to-integrate-with-workfront}

커넥터를 설치한 후 커넥터 패키지를 AEM으로 가져오고 [!DNL Workfront]의 문서와 연결하도록 AEM을 구성하십시오.

커넥터 설치에 대한 자세한 내용은 [커넥터 패키지 설치 [!DNL Workfront for AEM Assets] 를 참조하십시오](#install-the-workfront-for-aem-assets-connector-package).

* [전제 조건](#prerequisites)
* [&#x200B; [!DNL Workfront]과(와) AEM 통합](#integrate-aem-with-workfront)
* [[!UICONTROL AEM 외부화 구성]](#configure-the-aem-externalizer)

### 전제 조건 {#prerequisites}

시작하기 전에 workfront 서비스에 대한 권한을 활성화해야 합니다.

1. AEM에서 **[!UICONTROL 도구]** > **[!UICONTROL 보안]** > **[!UICONTROL 권한]**(으)로 이동합니다.
1. 왼쪽 상단 모서리에서 &#x200B; 드롭다운 메뉴에서 **[!UICONTROL 사용자]**&#x200B;를 선택하고 *[!UICONTROL 검색]* 필드에 **[!UICONTROL workfront-service]**&#x200B;을(를) &#x200B; 입력합니다. [!UICONTROL workfront-service] 사용자를 선택하십시오.
1. 화면 오른쪽에서 **[!UICONTROL ACE 추가]**&#x200B;를 선택하여 새 항목을 만듭니다.
1. {&#x200B;0}새 항목 추가{1&#x200B;} 창에서 **[!UICONTROL 경로]** 필드&#x200B;의 확인란 아이콘을 선택하고 다음 폴더를 선택합니다. **[!UICONTROL /conf]**&#x200B;**
1. **권한** 필드에 다음을 입력하십시오. *jcr:read*
1. 오른쪽 상단 모서리에서 **추가**&#x200B;를 선택합니다.
1. (선택 사항) 더 많은 항목을 만들려면 위의 단계를 반복합니다.

### [!DNL Workfront]과(와) AEM 통합 {#integrate-aem-with-workfront}

1. AEM Assets에 관리자로 로그인합니다.
1. **[!UICONTROL 도구]** > **[!UICONTROL 클라우드 서비스]** > **[!UICONTROL Workfront 통합 구성]** > **[!UICONTROL 글로벌-Workfront].**&#x200B;**&#x200B;**&#x200B;을 클릭합니다.

1. (조건부) 아직 만들지 않은 경우 [!DNL Workfront] 클라우드 구성 파일을 만듭니다.

   1. [!DNL Global-Workfront] 페이지의 오른쪽 상단 모서리에서 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.
   1. **[!UICONTROL Workfront URL]** 상자에서 [!DNL Workfront] 인스턴스의 URL을 지정하십시오.

      예를 들어 [!DNL https]://`<account>`.my.workfront.com입니다. 여기서 `<account>`은(는) AEM과의 통합에 사용하는 계정입니다.

   1. {&#x200B;0}기본 폴더&#x200B;**[!UICONTROL 필드에서 확인란 아이콘을 선택합니다.]**
   1. 드롭다운 메뉴에서 [!DNL Workfront] 개체에 연결된 문서가 저장된 경로를 선택합니다.
   1. 표시되는 AEM 모달에서 [!DNL Workfront] 개체에 연결된 문서가 있는 폴더의 경로를 따릅니다. 폴더를 선택한 다음 오른쪽 상단의 **[!UICONTROL 선택]**&#x200B;을 누릅니다.

      루트 /content/dam/ 아래에 있는 모든 폴더에 연결할 수 있습니다.

   1. **[!UICONTROL Workfront API 키]** 상자에서 [!UICONTROL Workfront] API 키를 지정합니다.

      [!DNL Workfront] API 키를 검색하려면

      1. 브라우저 탭을 열고 [!DNL Workfront] 계정에 [!DNL Workfront] 관리자로 로그인합니다.

      {{step-1-to-setup}}

      1. **[!UICONTROL 시스템]** > **[!UICONTROL 고객 정보]**&#x200B;를 클릭합니다.

         API 키를 이미 생성한 경우 [!DNL Workfront] API 키가 **사용자의 API 키** 레이블 아래에 표시됩니다.

      1. (조건부) API 키를 아직 생성하지 않은 경우 다음 중 하나를 생성해야 합니다.

         1. **[!UICONTROL API 키 설정]** 섹션에서 **[!UICONTROL 생성 후 API 키가 만료됩니다]** 옵션이 **없음**(으)로 설정되어 있는지 확인하십시오.

            만료 기간을 선택하면 API 키가 만료된 후 커넥터의 작동이 중지됩니다. 그런 다음 API 키를 다시 생성하고 [!DNL Workfront] 구성을 업데이트해야 합니다.

         1. **[!UICONTROL 사용자의 API 키]** 레이블에서 **[!UICONTROL API 키 생성]**&#x200B;을 클릭합니다. [!DNL Workfront]에 대한 API 키가 생성되어 표시됩니다.
      1. API 키를 클립보드에 복사합니다.
      1. AEM 커넥터의 브라우저 탭을 열고 **[!DNL Workfront API Key]** 상자에서 복사한 API 키를 붙여넣습니다.
   1. (조건부) **[!UICONTROL 통합 구성]** 페이지의 왼쪽 위 모서리에 있는 [!UICONTROL [!DNL Workfront]고급] 탭을 클릭하고 해당하는 경우 다음 옵션을 선택합니다.

      **[!UICONTROL 컬렉션 찾아보기 허용]:**&#x200B;조직에서 [!DNL Workfront] 사용자가 [!DNL Workfront] 개체에 AEM Assets 컬렉션을 연결할 수 있도록 허용하는 경우 이 옵션을 선택하십시오.

      **[!UICONTROL 사용자 Federated ID]:** 조직에서 Workfront에 로그인할 때 Federated ID 또는 SSO(Single Sign-On)를 사용하는 경우 이 옵션을 선택하십시오.

      **[!UICONTROL 전자 메일 도메인 무시]:** AEM 사용자가 사용자 ID에서 도메인 이름을 사용하지 않는 경우 이 옵션을 선택합니다.

      **[!UICONTROL 액세스 제한]** 이 옵션을 선택하여 허용 목록에 추가해야 하는 적절한 [!DNL Workfront] IP 주소를 지정합니다. 허용 목록에 추가하다허용 목록에 추가하다 에 대한 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

   1. Workfront 통합 구성 페이지의 왼쪽 상단 모서리에서 **[!UICONTROL 기본]** 탭을 클릭한 다음 **[!UICONTROL 연결]**&#x200B;을 클릭합니다.

      >[!NOTE]
      >
      >변경 사항을 적용하는 데 시간이 걸릴 수 있습니다. 번들을 다시 시작하면 프로세스 속도가 빨라질 수 있습니다.



1. (조건부) [!DNL Workfront] 클라우드 구성 파일을 이미 만든 경우 **[!UICONTROL 전역-[!DNL Workfront]]**&#x200B;을(를) 선택한 다음 왼쪽 상단 모서리에서 **[!UICONTROL 속성]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL 키 생성],**&#x200B;을 클릭하여 AEM API 키를 생성한 다음 AEM API 키를 클립보드에 복사합니다.

   나중에 [!UICONTROL AEM]을(를) [!UICONTROL AEM Assets]과(와) 통합하도록 구성할 때 Workfront API 키가 필요합니다. 자세한 내용은 [AEM 에셋과 통합하도록 Workfront 구성](#configure-workfront-to-integrate-with-aem-assets)을 참조하십시오.

1. 오른쪽 상단에서 **[!UICONTROL 저장]**&#x200B;을 클릭합니다. [!UICONTROL 전역-[!DNL Workfront]] 창이 표시됩니다.

   ![Properties.png](assets/properties-350x117.png)

1. (선택 사항) AEM과 [!DNL Workfront] 간의 양방향 통신을 동기화합니다.

   1. **[!UICONTROL 전역-[!DNL Workfront]].** 클릭
   1. 창의 왼쪽 상단 모서리에서 **[!UICONTROL 속성]**&#x200B;을 클릭합니다. **[!UICONTROL [!DNL Workfront]통합 구성]** 페이지가 표시됩니다.

      ![속성2.png](assets/properties2-350x444.png)

   1. (선택 사항) [!UICONTROL AEM Assets]과(와) [!DNL Workfront] 간의 댓글 동기화를 사용하려면 **[!UICONTROL 댓글 동기화 사용]**&#x200B;을 클릭하세요.

      >[!IMPORTANT]
      >
      >자산을 동기화하려면 [!UICONTROL 문서 동기화]를 사용하도록 설정해야 합니다.

   1. (선택 사항) 주석 동기화를 끄려면 **[!UICONTROL 주석 동기화 사용 안 함].**&#x200B;을 클릭하세요.

      또는

      AEM 인스턴스에 등록된 [!UICONTROL NOTE CREATE] 이벤트 구독을 삭제합니다.

      이벤트 구독에 대한 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md)를 참조하십시오.

1. [계속 [!UICONTROL AEM 외부화를 구성]](#configure-the-aem-externalizer)합니다.

### [!UICONTROL AEM 외부화 구성] {#configure-the-aem-externalizer}

[!UICONTROL AEM 외부화]을(를) 사용하면 AEM에서 [!DNL Workfront]에서 사용할 수 있는 형식으로 URL을 전달할 수 있습니다. 올바르게 구성되지 않은 경우 [!DNL Workfront]에서 AEM API를 호출할 수 없으며 Workfront에서 AEM 문서를 연결하는 URL이 작동하지 않습니다.

1. AEM에서 **[!UICONTROL 도구]** > **[!UICONTROL 작업]** > **[!UICONTROL 웹 콘솔]**&#x200B;을 클릭합니다.

1. **[!UICONTROL OSGI]**&#x200B;를 클릭한 다음 드롭다운 메뉴에서 **[!UICONTROL 구성]**&#x200B;을 클릭합니다.

1. 구성 목록에서 {&#x200B;0}일 CQ 링크 외부화&#x200B;**[!UICONTROL 를 선택합니다.]** **[!UICONTROL 외부화]** 페이지가 표시됩니다.

1. **[!UICONTROL 도메인]** 섹션에서 **[!UICONTROL 작성자]** 필드에 나열된 도메인이 AEM 사용자가 외부에서 액세스할 수 있는 도메인 이름인지 확인하십시오.

   [!UICONTROL 작성자] 필드의 도메인 이름은 AEM 인스턴스의 URL 줄에 나열된 도메인과 일치해야 합니다.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (조건부) 필요한 경우 **[!UICONTROL 작성자]** 필드에서 도메인을 업데이트합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 이제 [!UICONTROL AEM Assets]이(가) 문서를 [!DNL Workfront]과(와) 연결하도록 구성되었습니다.

1. [과(와) 통합하려면  [!DNL Workfront] 구성 [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets)을(를) 계속합니다.

## [!DNL Workfront]과(와) 통합하도록 [!DNL AEM assets] 구성 {#configure-workfront-to-integrate-with-aem-assets}

[!UICONTROL AEM Assets용 &#x200B;]Workfront 설치[&#x200B; 커넥터 패키지 설치[!UICONTROL 에 설명된 대로 &#x200B;]AEM Assets용 Workfront](#install-the-workfront-for-aem-assets-connector-package) 커넥터를 설치하고 [!UICONTROL AEM Assets]을(를) 구성([와 통합하도록 [!UICONTROL AEM Assets]에 설명된 대로 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)을) 한 후에는 [!DNL Workfront]과(와) [!DNL Workfront] 사이에 문서를 연결하도록 [!DNL AEM Assets]을(를) 구성해야 합니다.

1. 관리자로 Workfront에 로그인합니다.

   >[!TIP]
   >
   >[!UICONTROL Workfront]에서는 AEM 통합 전용 [!UICONTROL Workfront] 관리자를 만들 것을 권장합니다. 사용자에게 [!UICONTROL Workfront] 관리자 액세스 수준을 할당하는 방법에 대한 자세한 내용은 [특정 영역에 대한 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)를 참조하십시오.

{{step-1-to-setup}}

1. **[!UICONTROL 문서]** > **[!UICONTROL 사용자 지정 통합]을 클릭합니다.**

1. **[!UICONTROL 사용자 지정 통합 추가]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 이름]** 상자에 사용자 지정 통합 이름을 입력합니다.

   사용자가 [!UICONTROL Workfront] 내에서 통합을 사용할 때 표시되는 이름입니다.

1. **[!UICONTROL 기본 API URL]** 상자에 AEM 인스턴스의 URL을 입력합니다.

   기본 API URL은 AEM 인스턴스의 URL 뒤에 /bin/webhooks/api/ 경로가 옵니다.

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. **[!UICONTROL 인증 유형]** 드롭다운 메뉴에서 **[!UICONTROL ApiKey].**&#x200B;을(를) 선택합니다.

1. {&#x200B;0}API 키&#x200B;**[!UICONTROL 상자에]** AEM Assets[!UICONTROL 을(를) 구성할 때 복사한 AEM API 키를 붙여 넣습니다.]
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
1. (선택 사항) 통합이 [!UICONTROL Active]&#x200B;(으)로 표시되어 있는지 확인하십시오.\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront]이(가) [!DNL AEM Assets]에서 작동하도록 구성되었습니다.

   AEM의 자산에 액세스하려면 커넥터를 사용해야 하는 각 [!DNL Workfront] 사용자를 AEM의 사용자로 설정해야 합니다. 사용자 만들기에 대한 자세한 내용은 [커넥터를 사용하도록 사용자 설정](#set-up-users-to-use-the-connector)을 참조하십시오.

## 커넥터를 사용할 사용자 설정 {#set-up-users-to-use-the-connector}

사용자가 커넥터에 액세스하려면 AEM에 사용자 프로필이 있어야 하며 [!DNL Workfront]만들기[!UICONTROL &#x200B; 및 &#x200B;]삭제[!UICONTROL &#x200B; 권한을 포함하는 액세스 수준이 있는 &#x200B;] 그룹에 속해 있어야 합니다.

[!DNL Workfront] 권한에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하십시오.

* [&#x200B; [!DNL AEM assets]에서 사용자 설정](#set-up-users-in-aem-assets)

### [!DNL AEM assets]에서 사용자 설정 {#set-up-users-in-aem-assets}

1. [!DNL AEM Assets]에 Workfront 관리자로 로그인합니다.
1. **[!UICONTROL 도구]** > **{&#x200B;3}{4&#x200B;}보안** > **[!UICONTROL 사용자]**&#x200B;를 클릭합니다.**&#x200B;**

1. (조건부) 사용자에게 AEM에 사용자 프로필이 없는 경우 AEM 사용자 프로필을 만듭니다.

   1. **[!UICONTROL 사용자 만들기].**&#x200B;를 클릭합니다
   1. 사용자의 개인 정보를 입력합니다.

      ![64NewUser.png](assets/64newuser-350x524.png)

      필수 필드는 **ID** 필드뿐입니다. 사용자의 AEM ID는 사용자의 [!DNL Workfront] 이메일 주소인 [!DNL Workfront] ID와 일치해야 합니다.

      AEM을 **[!UICONTROL 과(와) 통합하도록 구성할 때]**&#x200B;이메일 도메인 무시[!DNL Workfront] 옵션을 선택한 경우 AEM ID가 [!DNL Workfront] 이메일 주소와 일치하지 않습니다.

1. (조건부) 사용자에게 AEM 프로필이 있는 경우 사용자의 AEM 프로필을 엽니다.

   1. {&#x200B;0}사용자&#x200B;**[!UICONTROL 를 클릭합니다.]** **[!UICONTROL 사용자 관리]** 페이지가 표시됩니다.

   1. 추가할 사용자를 클릭한 다음 **[!UICONTROL 속성]**&#x200B;을 클릭합니다. 사용자의 설정 페이지가 표시됩니다.

1. **[!UICONTROL 그룹]** 탭을 클릭합니다.

   ![그룹 탭](assets/groupstab.png)

1. 사용자가 [!DNL Workfront]만들기&#x200B;**[!UICONTROL 및]**&#x200B;삭제&#x200B;**[!UICONTROL 권한을 포함하는 액세스 수준이 있는 하나 이상의]** 그룹에 속해 있는지 확인하십시오.

   1. 기존 그룹에 사용자를 추가하려면 **[!UICONTROL 그룹 이름 입력]** 상자에 그룹 이름을 입력한 다음 드롭다운 메뉴에 표시될 때 그룹을 선택합니다.

      또는

      사용자가 멤버인 그룹을 선택하려면 **[!UICONTROL 이 사용자가 멤버인 그룹]** 섹션에서 그룹을 선택하십시오.

1. **[!UICONTROL 저장].** 클릭
