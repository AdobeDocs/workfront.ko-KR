---
title: 구성 [!DNL Workfront] with [!DNL Adobe Experience Manager] 레거시 커넥터
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 로서의 [!DNL Adobe Workfront] 관리자, [!DNL Workfront] AEM(Adobe Experience Manager) Assets를 사용하면 조직에서 워크플로우 내에서 자산을 생성, 공유 및 유지 관리할 수 있는 포괄적인 컨텐츠 관리 솔루션을 제공할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1893'
ht-degree: 0%

---

# 구성 [!DNL Workfront] with [!DNL Adobe Experience Manager] 레거시 커넥터

로서의 [!DNL Adobe Workfront] 관리자, [!DNL Workfront] with [!UICONTROL Adobe Experience Manager (AEM) 자산] 또한 워크플로우 내에서 자산을 생성, 공유 및 유지 관리할 수 있는 포괄적인 컨텐츠 관리 솔루션을 조직에 제공합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## [!DNL Workfront for AEM Assets]

다음 [!DNL Workfront for AEM Assets connector] 조직에서 다음을 수행할 수 있습니다.

* 의 프로젝트, 작업, 문제 및 요청에 AEM 자산 및 폴더를 연결하여 크리에이티브 컨텐츠를 공동 작업하고 관리할 수 있습니다 [!DNL Workfront].

   타사 애플리케이션과의 설명서 통합 구성에 대한 자세한 내용은  [문서 통합 구성](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* 와 통합 [!DNL AEM Digital Asset Managemen]t(DAM) 저장소, 사용 가능 [!DNL Workfront] DAM에 저장된 디지털 자산을 관리하고 공유할 수 있습니다.

   문서 및 자산 폴더 연결에 대한 자세한 내용은   [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* 두 애플리케이션의 메타데이터를 자산에 결합하고 적용합니다.
* 자산에 대한 모든 포함 통신 스트림을 봅니다. 의 자산에 대한 업데이트 및 주석 [!DNL Workfront] 또는 [!UICONTROL AEM Assets] 는 다른 애플리케이션과 동기화되어 자산에 대한 포괄적인 통신 기록을 수립합니다.

   설명 작성에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오. [문서에 업데이트 추가](../../documents/managing-documents/add-update-documents.md).

## 설치 사전 요구 사항 [!DNL AEM Assets] 커넥터

를 설치하기 전에 [!DNL Workfront] 커넥터 [!UICONTROL AEM Assets]를 채울 때는 다음 전제 조건을 충족해야 합니다.

* [!UICONTROL AEM Assets] 설치 및 구성, 버전 6.5 이상 설치에 대한 자세한 정보 [!UICONTROL AEM Assets]를 참조하고 [[!DNL Adobe Experience Manager] 설명서](https://experienceleague.adobe.com/docs/experience-manager.html).
* (조건부) 방화벽 규칙이 트래픽을 예상대로 허용하지 않는다면 클러스터의 IP 주소 및/또는 도메인을에 허용 목록에 추가하다 추가하십시오. 자세한 내용은 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 설치 [!DNL Workfront for AEM Assets] 커넥터 패키지 {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>다음 지침은 [!DNL Workfront with AEM Assets] 로 대체된 레거시 커넥터 [[!DNL Workfront for Experience Manager] 향상된 커넥터](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). 자세한 내용은 계정 담당자에게 문의하십시오.

를 설치하려면 [!DNL Workfront for AEM Assets] 커넥터 를 사용하여 커넥터를 AEM으로 패키지로 가져와야 합니다 [!UICONTROL CRX 패키지 관리자].

1. 이미 AEM을 설치한 워크스테이션에서 를 다운로드합니다. [!DNL Workfront for AEM Assets] 커넥터 설치 파일입니다.

   이 파일을 가져올 수 있습니다 [!DNL Workfront for AEM Assets] 커넥터 [!DNL Workfront] 담당자.

1. 관리자 계정을 사용하여 AEM에 로그인합니다.
1. 클릭 **[!UICONTROL 도구]** > **[!UICONTROL 배포]** > **[!UICONTROL 패키지]**.

   다음 [!UICONTROL CRX 패키지 관리자] 엽니다.

1. 클릭 **[!UICONTROL 패키지 업로드].**

1. 에서 [!UICONTROL 패키지 업로드] 대화 상자에서 을 찾아 선택합니다 [!UICONTROL Workfront 커넥터] 패키지 를 클릭한 다음 **[!UICONTROL 확인]**.\
   패키지는 [!UICONTROL CRX 패키지 관리자].

1. 클릭 **[!UICONTROL 설치].**

1. 설정 [!UICONTROL 패키지] 대화 상자에서 고급 설정을 무시하고 를 클릭합니다 **[!UICONTROL 설치]**.
1. (선택 사항) 커넥터가 성공적으로 설치되었는지 확인하려면 [!UICONTROL 활동 로그]:

   ```
   Package installed in <time>
   ```

1. 닫기 [!UICONTROL CRX 패키지 관리자].

   커넥터가 설치되었으며 이제 구성할 수 있습니다 [!DNL AEM Assets] 을 통합 [!DNL Workfront].

1. 계속 [구성 [!DNL AEM Assets] 을 통합 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## 구성 [!DNL AEM Assets] 을 통합 [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

커넥터를 설치한 후 커넥터 패키지를 AEM으로 가져오고 AEM에서 문서에 연결하도록 구성합니다. [!DNL Workfront].

커넥터 설치에 대한 자세한 내용은  [설치 [!DNL Workfront for AEM Assets] 커넥터 패키지](#install-the-workfront-for-aem-assets-connector-package).

* [전제 조건](#prerequisites)
* [AEM과 통합 [!DNL Workfront]](#integrate-aem-with-workfront)
* [구성 [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### 전제 조건 {#prerequisites}

시작하기 전에 workfront 서비스에 대한 권한을 활성화해야 합니다.

1. AEM에서 **[!UICONTROL 도구]**> **[!UICONTROL 보안]**> **[!UICONTROL 권한]**.
1. 왼쪽 상단 모서리에서 **[!UICONTROL 사용자]**&#x200B;드롭다운 &#x200B; 메뉴에서 을(를) 입력하고 을(를) 입력합니다. *[!UICONTROL workfront 서비스]* 에서 **[!UICONTROL 검색]**&#x200B;필드&#x200B;. 을(를) 선택합니다 [!UICONTROL workfront 서비스] 사용자.
1. 화면 오른쪽에서 을(를) 선택합니다. **[!UICONTROL ACE 추가]** 새 항목을 만들려면
1. 에서&#x200B;**[!UICONTROL 새 항목 추가]**&#x200B;창&#x200B;에서 확인란 아이콘을 선택합니다 **[!UICONTROL 경로]**&#x200B;필드&#x200B;을 선택하고 폴더를 선택합니다. */conf*
1. 권한 필드에 다음을 입력합니다. *jcr:read*
1. 선택 **[!UICONTROL 추가]**&#x200B;오른쪽 &#x200B; 상단 모서리에서
1. (선택 사항) 단계를 반복하여 항목을 더 만듭니다.

### AEM과 통합 [!DNL Workfront] {#integrate-aem-with-workfront}

1. 관리자로 AEM Assets에 로그인합니다.
1. 클릭 **[!UICONTROL 도구]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Workfront 통합 구성]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (조건부) 아직 작성하지 않았다면 [!DNL Workfront] 클라우드 구성 파일.

   1. 클릭  **[!UICONTROL 만들기]** 오른쪽 위 모서리에서 [!DNL Global-Workfront] 페이지.
   1. 에서 **[!UICONTROL Workfront URL]** 상자에 사용할 URL을 지정합니다 [!DNL Workfront] 인스턴스.

      예, [!DNL https]:/`<account>`.my.workfront.com, 여기서 `<account>` 는 AEM과의 통합에 사용하는 계정입니다.

   1. 에서&#x200B;**[!UICONTROL 기본 폴더]** 필드에서 확인란 아이콘을 선택한 다음 드롭다운 메뉴에서 링크된 문서의 경로를 선택합니다 [!DNL Workfront] 개체는 저장됩니다.
   1. 표시되는 AEM 모달에서 연결된 문서를 사용하여 폴더의 경로를 따릅니다 [!DNL Workfront] 개체. 폴더를 선택하고 키를 누릅니다 **[!UICONTROL 선택]**&#x200B;오른쪽 위&#x200B;에 있습니다.

      루트 /content/dam/ 아래의 폴더에 연결할 수 있습니다.

   1. 에서 **[!UICONTROL Workfront API 키]** 상자에서 다음을 지정합니다 [!UICONTROL Workfront] API 키.

      를 검색하려면 [!DNL Workfront] API 키:

      1. 브라우저 탭을 열고 [!DNL Workfront] 계정으로서 [!DNL Workfront] 관리자
      1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

      1. 클릭 **[!UICONTROL 시스템]** >**[!UICONTROL 고객 정보]**.

         이미 API 키를 생성한 경우 [!DNL Workfront] API 키는 사용자의 API 키 레이블 아래에 표시됩니다.

      1. (조건부) API 키를 아직 생성하지 않은 경우 API 키를 생성해야 합니다.

         1. 에서 **[!UICONTROL API 키 설정]** 섹션에서 다음을 확인합니다 **[!UICONTROL 생성 후 API 키는에 만료됩니다.]** 옵션이 없음으로 설정되어 있습니다.

            만료 기간을 선택하면 API 키가 만료된 후 커넥터의 작동이 중지됩니다. 그런 다음 API 키를 다시 생성하고 을 업데이트해야 합니다 [!DNL Workfront] 구성.

         1. 아래에 **[!UICONTROL 사용자의 API 키]** 레이블, **[!UICONTROL API 키 생성]**.

            용 API 키 [!DNL Workfront] 및 가 생성됩니다.
      1. API 키를 클립보드에 복사합니다.
      1. AEM Connector 및 의 브라우저 탭을 엽니다. **[!DNL Workfront API Key]** 상자에 복사한 API 키를 붙여넣습니다.
   1. (조건부) **[!UICONTROL 고급]** 탭의 왼쪽 위 모서리에 있는 [!UICONTROL [!DNL Workfront] 통합 구성] 페이지를 선택하고 해당하는 경우 다음 옵션을 선택합니다.

      **[!UICONTROL 컬렉션 검색 허용]:**&#x200B;조직에서 허용하는 &#x200B; 경우 이 옵션을 선택합니다 [!DNL Workfront] AEM Assets 컬렉션을 [!DNL Workfront] 개체.

      **[!UICONTROL 사용자 Federated ID]:** 조직에서 Workfront에 로그인할 때 Federated ID 또는 SSO(Single Sign-On)를 사용하는 경우 이 옵션을 선택합니다.

      **[!UICONTROL 전자 메일 도메인 무시]:** AEM 사용자가 사용자 ID에서 도메인 이름을 사용하지 않는 경우 이 옵션을 선택합니다.

      **[!UICONTROL 액세스 제한]:** 적절한 옵션을 지정하려면 이 옵션을 선택합니다 [!DNL Workfront] 에 추가해야 하는 IP 허용 목록에 추가하다 주소입니다. 에 대한 자세한 허용 목록에 추가하다 내용은 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. 을(를) 클릭합니다. **[!UICONTROL 기본]** Workfront 통합 구성 페이지의 왼쪽 위 모서리에 있는 탭을 클릭한 다음 **[!UICONTROL Connect]**.

      >[!NOTE]
      >
      >변경 사항을 적용하려면 시간이 걸릴 수 있습니다. 번들을 다시 시작하면 프로세스의 속도가 빨라질 수 있습니다.



1. (조건부) 이미 [!DNL Workfront] 클라우드 구성 파일, **[!UICONTROL 글로벌[!DNL Workfront]]**&#x200B;를 클릭한 다음 왼쪽 위 모서리에서 **[!UICONTROL 속성]**.

1. 다음을 클릭하여 AEM API 키를 생성합니다. **[!UICONTROL 키 생성],** 그런 다음 AEM API 키를 클립보드에 복사합니다.

   나중에 구성할 때 AEM API 키가 필요합니다 [!UICONTROL Workfront] 을 통합 [!UICONTROL AEM Assets]. 자세한 내용은 [AEM 자산과 통합하도록 Workfront 구성](#configure-workfront-to-integrate-with-aem-assets).

1. 오른쪽 위 모서리에서 을(를) 클릭합니다. **[!UICONTROL 저장]**.

   다음 [!UICONTROL 글로벌[!DNL Workfront]] 창이 표시됩니다.

   ![Properties.png](assets/properties-350x117.png)

1. (선택 사항) AEM과 간의 양방향 통신을 동기화합니다 [!DNL Workfront].

   1. 클릭 **[!UICONTROL 글로벌[!DNL Workfront]].**
   1. 창의 왼쪽 위 모서리에서 **[!UICONTROL 속성]**.

      다음 [!UICONTROL [!DNL Workfront] 통합 구성] 페이지가 표시됩니다.

      ![Properties2.png](assets/properties2-350x444.png)

   1. (선택 사항) 사이에 주석을 동기화할 수 있습니다 [!UICONTROL AEM Assets] 및 [!DNL Workfront]를 클릭합니다. **[!UICONTROL 주석 동기화 사용]**.

      >[!IMPORTANT]
      >
      >활성화 [!UICONTROL 문서 동기화] 자산을 동기화합니다.

   1. (선택 사항) 주석 동기화를 해제하려면 **[!UICONTROL 주석 동기화 사용 안 함].**

      또는

      삭제 [!UICONTROL 참고 만들기] AEM 인스턴스에 등록된 이벤트 구독입니다.

      이벤트 가입에 대한 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md).

1. 계속 [구성 [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### 구성 [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

다음 [!UICONTROL AEM Externalizer] 에서는 AEM에서 사용할 수 있는 형식으로 URL을 전달할 수 있습니다. [!DNL Workfront]. 제대로 구성되지 않으면 [!DNL Workfront] AEM API를 호출할 수 없으며 Workfront에서 AEM 문서를 연결하는 URL이 작동하지 않습니다.

1. AEM에서 **[!UICONTROL 도구]** > **[!UICONTROL 작업]** >**[!UICONTROL 웹 콘솔]**.

1. 클릭 **[!UICONTROL OSGI]**&#x200B;를 클릭한 다음 **[!UICONTROL 구성]** 를 클릭합니다.

1. 구성 목록에서 을 선택합니다&#x200B;.**[!UICONTROL Day CQ Link Externalizer].**

   다음 [!UICONTROL 외부 도우미] 페이지가 표시됩니다.

1. 에서 **[!UICONTROL 도메인]** 섹션에서 [!UICONTROL 작성자] 필드는 AEM 사용자가 외부에서 액세스할 수 있는 도메인 이름입니다.

   의 도메인 이름 [!UICONTROL 작성자] 필드는 AEM 인스턴스의 URL 행에 나열된 도메인과 일치해야 합니다.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (조건부) 필요한 경우 [!UICONTROL 작성자] 필드.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   [!UICONTROL AEM Assets] 이제 가 문서를 [!DNL Workfront]

1. 계속 [구성 [!DNL Workfront] 을 통합 [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## 구성 [!DNL Workfront] 을 통합 [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

를 설치한 후 [!UICONTROL Workfront for AEM Assets] 커넥터(에 설명된 대로) [설치 [!UICONTROL Workfront for AEM Assets] 커넥터 패키지](#install-the-workfront-for-aem-assets-connector-package)) 및 configure 를 참조하십시오. [!UICONTROL AEM Assets] 에 설명된 대로 [구성[!UICONTROL  AEM Assets] 을 통합 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), 다음을 구성해야 합니다. [!DNL Workfront] 문서 간 연결 [!DNL Workfront] 및 [!DNL AEM Assets].

1. 에 로그인합니다. [!DNL Workfront] 로서의 [!UICONTROL Workfront] 관리자

   >[!TIP]
   >
   >[!UICONTROL Workfront] 권장 사항 [!UICONTROL Workfront] AEM 통합을 위한 전용 관리자 할당에 대한 자세한 정보 [!UICONTROL Workfront] 사용자에 대한 관리자 액세스 레벨은 [특정 영역에 대한 관리자 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 문서]**> **[!UICONTROL 사용자 지정 통합].**

1. 클릭 **[!UICONTROL 사용자 지정 통합 추가]**.
1. 에서 **[!UICONTROL 이름]** 상자에서 사용자 지정 통합의 이름을 지정합니다.

   내에서 통합을 사용할 때 사용자에게 표시되는 이름입니다 [!UICONTROL Workfront]; 예를 들어 *&quot;[!DNL AEM Assets]&quot;* 참조하십시오.

1. 에서 **[!UICONTROL 기본 API URL]** 상자에서 AEM 인스턴스의 URL을 지정합니다.

   기본 API URL은 AEM 인스턴스의 URL 뒤에 오는 경로로 구성됩니다. /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. 에서 **[!UICONTROL 인증 유형]** 드롭다운 메뉴에서 **[!UICONTROL ApiKey].**

1. 에서&#x200B;**[!UICONTROL API 키]** 상자를 열고 구성할 때 복사한 AEM API 키를 붙여넣습니다. [!UICONTROL AEM Assets].
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
1. (선택 사항) 통합이 표시되었는지 확인합니다 [!UICONTROL 활성].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] 이제 이 [!DNL AEM Assets].

   AEM의 자산에 액세스하려면 각 [!DNL Workfront] 커넥터를 사용해야 하는 사용자는 AEM에서 사용자로 설정해야 합니다. 사용자 만들기에 대한 내용은  [커넥터를 사용하도록 사용자 설정](#set-up-users-to-use-the-connector).

## 커넥터를 사용하도록 사용자 설정 {#set-up-users-to-use-the-connector}

사용자가 커넥터에 액세스하려면 AEM에 사용자 프로필이 있고 [!DNL Workfront] 액세스 수준을 포함하는 그룹 [!UICONTROL 만들기] 및 [!UICONTROL 삭제] 사용 권한.

에 대한 자세한 정보 [!DNL Workfront] 사용 권한: [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [에서 사용자 설정 [!DNL AEM assets]](#set-up-users-in-aem-assets)

### 에서 사용자 설정 [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. 에 로그인합니다. [!DNL AEM Assets] 로서의 [!DNL Workfront] 관리자
1. 클릭 **[!UICONTROL 도구]** >**&#x200B;**&#x200B;**[!UICONTROL 보안]** >**[!UICONTROL 사용자]**.

1. (조건부) 사용자에게 AEM에 사용자 프로필이 없는 경우 AEM 사용자 프로필을 만듭니다.

   1. 클릭 **[!UICONTROL 사용자 만들기].**
   1. 사용자의 개인 정보를 입력합니다.

      ![64NewUser.png](assets/64newuser-350x524.png)

      유일한 필수 필드는 ID 필드입니다. 사용자의 AEM ID가 다음과 일치해야 합니다 [!DNL Workfront] 사용자의 ID [!DNL Workfront] 이메일 주소.

      을(를) 선택한 경우 [!UICONTROL 전자 메일 도메인 무시] 와 통합하도록 AEM을 구성한 경우 옵션 [!DNL Workfront]를 입력하면 AEM ID가 [!DNL Workfront] 이메일 주소.

1. (조건부) 사용자에게 AEM 프로필이 있는 경우 사용자의 AEM 프로필을 엽니다.

   1. 클릭&#x200B;**[!UICONTROL 사용자].**

      다음 [!UICONTROL 사용자 관리] 페이지가 표시됩니다.

   1. 추가할 사용자를 클릭한 다음 **[!UICONTROL 속성]**.

      사용자의 설정 페이지가 표시됩니다.

1. 을(를) 클릭합니다. **[!UICONTROL 그룹]** 탭.

   ![](assets/groupstab.png)

1. 사용자가 하나 이상의 항목에 속하는지 확인 [!DNL Workfront] 액세스 수준을 포함하는 그룹 [!UICONTROL 만들기] 및 [!UICONTROL 삭제] 사용 권한.

   1. 사용자를 기존 그룹에 추가하려면 **[!UICONTROL 유형 그룹 이름]** 상자를 선택한 다음 드롭다운 메뉴에 그룹이 나타날 때 그룹을 선택합니다.

      또는

      사용자가 구성원으로 있는 그룹을 선택하려면 **[!UICONTROL 이 사용자가 구성원으로 있는 그룹]** 섹션을 참조하십시오.

1. **[!UICONTROL 저장]을 클릭합니다.**
