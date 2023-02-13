---
title: 문서 통합 구성
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 문서 통합 구성
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# 문서 통합 구성

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

로서의 [!DNL Adobe Workfront] 관리자는 문서 통합을 구성하여 문서를 [!UICONTROL Workfront]. 다음을 구성할 수도 있습니다 [!UICONTROL Workfront] 문서 서비스 응용 프로그램에만 저장되고 [!UICONTROL Workfront] 자체. 자세한 내용은 [문서 업데이트 및 연결 위치 [!UICONTROL Workfront] 외부 클라우드 제공업체로](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>사이에 열린 통신을 허용하려면 [!DNL Workfront Proof] 그리고 [!DNL Workfront] 서버에서는 특정 IP 주소를에 추가해야 할 수 허용 목록에 추가하다 있습니다. 자세한 내용은 [방화벽 허용 목록에 추가하다 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 지원되는 통합

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

문서 관리를 위해 다음 통합을 구성할 수 있습니다.

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   증명 연결 [!DNL Workfront Proof] 에서는 원래 내에서 만들어진 증명을 만들 수 있습니다 [!DNL Workfront Proof] 내에서 사용 가능 [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] 이 기능을 사용하려면 계획 이상이 필요합니다. 사용 가능한 다양한 계획에 대한 자세한 내용은 [Workfront 플랜.](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   통합 관련 정보 [!DNL SharePoint]를 참조하십시오. [구성 [!DNL SharePoint] 통합](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* 타사 클라우드 문서 공급자:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!UICONTROL Google 드라이브]

      <!--Quip-->
   >[!TIP]
   >
   >에 바로 업로드된 문서를 증명하고 승인하는 것과 동일한 방법으로 외부 클라우드 공급자로부터 연결된 문서를 증명 및 승인할 수 있습니다 [!DNL Workfront].

* 기타 문서 공급자(사용자 정의 문서 통합을 통해)

   A [!UICONTROL Pro] [!DNL Workfront] 이 기능을 사용하려면 계획 이상이 필요합니다. 사용 가능한 다양한 계획에 대한 자세한 내용은 [[!DNL Workfront] 계획.](https://www.workfront.com/plans)

또한 [!DNL Workfront] 기본 DAM(Digital Asset Management) 시스템이나 타사 DAM 통합을 통해 경험을 문서화합니다. 사용자가 해당 서비스에 연결하려면 관리자가 이러한 기능을 활성화해야 합니다 [!DNL Workfront] 계정이 필요합니다. Workfront DAM에 대한 자세한 내용은 [문서 관리 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## 문서 관리를 위한 통합 구성

1. 에 로그인합니다. [!DNL Workfront] 관리자로.
1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 클라우드 공급자].**

1. (선택 사항) 문서 서비스 응용 프로그램에 저장된 문서에 대한 [!DNL Workfront], 선택 **[!UICONTROL 사용자가 문서를 저장할 수 없음 [!DNL Workfront]].**

1. 활성화할 통합을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

통합을 설정하는 경우 [!DNL Workfront DAM]를 활성화하면 됩니다 [!DNL Workfront] 메타데이터와 문서를 포함시키려면 다음을 수행합니다. 매핑 메타데이터에 대한 자세한 내용은 [메타데이터 매핑 설정](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## 사용자 지정 문서 통합 구성

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

사용자 정의 문서 통합을 통해 [!DNL Workfront] 사용자가 파일을 [!DNL Workfront] 이 시스템이 [!DNL Workfront].

사용자가 사용자 지정 통합을 사용할 수 있도록 하려면 먼저 통합을 빌드해야 합니다. 사용할 통합을 빌드하는 방법에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

사용자 지정 문서 통합이 빌드되면 사이트의 사용자가 이 통합을 사용할 수 있도록 할 수 있습니다.

1. 에 로그인합니다. [!DNL Workfront] 관리자로.
1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 사용자 지정 통합].**

1. 클릭 **[!UICONTROL 사용자 지정 통합 추가]**.
1. 통합을 구성하려면 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>사용자 지정 통합의 이름입니다. Workfront 내에서 통합을 사용할 때 표시되는 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 기본 API URL] </td> 
      <td>API 호출에 대한 기본 HTTP 또는 보안 HTTP URL입니다. 예, <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 인증 유형]</td> 
      <td> <p>사용자 지정 통합에 인증된 API를 호출할 때 사용할 인증 방법입니다.</p> 
       <ul> 
        <li>만약 <strong>[!UICONTROL OAuth]</strong>를 클릭하여 6단계를 계속 진행합니다.</li> 
        <li>만약 <strong>[!UICONTROL ApiKey]</strong>7단계로 진행합니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) 선택한 경우 **[!UICONTROL OAuth]** 에 대한 인증 **[!UICONTROL 인증 유형]**, 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 인증 URL]</td> 
      <td>사용자 인증에 사용되는 전체 URL입니다. [!DNL Workfront] 사용자가 OAuth 프로비저닝 프로세스의 일부로 이 주소로 이동합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 끝점 URL]</td> 
      <td>OAuth 토큰을 검색하는 데 사용되는 전체 API URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>이 통합을 위한 OAut 클라이언트 ID.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>이 통합을 위한 OAut 클라이언트 암호입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 요청 매개 변수]</td> 
      <td> <p>모든 API 호출의 쿼리 문자열에 추가할 선택적 값을 지정합니다. 예를 들어 access_type=offline 입니다.</p> <p>여러 요청 매개 변수를 추가하려면 <strong>+요청 매개 변수 추가</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >다음 [!DNL Workfront] 리디렉션 URI가 [!UICONTROL 사용자 지정 통합] 페이지에는 외부 문서 공급자와 이 통합을 등록하는 데 사용되는 URI가 나열됩니다.

1. (조건부) 선택한 경우 **[!UICONTROL ApiKey]** 에 대한 인증 **[!UICONTROL 인증 유형]**&#x200B;를 지정하는 경우 사용자 지정 문서 공급자가 발급한 API 키를 지정합니다.

   [!DNL Workfront] 는 이 API 키를 사용하여 문서 공급자에 대해 인증된 API를 호출합니다.

1. 클릭 **[!UICONTROL 저장]** 통합을 생성합니다.

## 문서 통합 사용

사용자가 다음을 사용할 수 있는 방법에 대한 자세한 정보 [!DNL Workfront DAM]를 참조하십시오. [문서 관리 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

사용자 언어 교정 사용 방법에 대한 자세한 내용은 [증명 만들기](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

사용자가 타사 문서 통합을 구성한 후 이를 사용하는 방법에 대한 자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 구성 [!DNL Workfront] 메타데이터를 로 보냅니다. [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

에서 문서를 보낼 때 [!DNL Workfront] to [!DNL Workfront DAM]를 눌러 해당 문서와 관련된 정보를 전송할 수도 있습니다. 문서에 대한 정보가 [!DNL Workfront DAM] 을 메타데이터로 포함합니다.

정보는 단방향으로만 매핑되며 [!DNL Workfront] to [!DNL Workfront DAM] 문서가 업로드될 때만 전송됩니다 [!DNL Workfront DAM]. Workfront 필드의 향후 변경 사항은 의 메타데이터 필드를 업데이트하지 않습니다 [!DNL Workfront DAM] 문서가 이미 업로드된 후.\
동일한 [!DNL Workfront] 다양한 [!DNL Workfront DAM] 필드는 사용할 수 없습니다 [!DNL Workfront DAM] 여러 필드 [!DNL Workfront] 필드.

여러 항목을 구성해야 하는 경우 [!DNL Workfront] 한 개로 내보내기 위한 필드 [!DNL Workfront DAM] 필드, 먼저 계산된 사용자 지정 필드를 [!DNL Workfront] 개체의 모든 개별 사용자 지정 필드를 표시합니다. 그런 다음 계산된 지표를 매핑합니다 [!DNL Workfront] 필드를 하나로 [!DNL Workfront DAM] 필드.\
계산된 사용자 지정 필드에 대한 자세한 내용은 [사용자 지정 양식에 계산된 데이터 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

매핑은 [!DNL Workfront] to [!UICONTROL Workfront] DAM.

로서의 [!DNL Workfront] 관리자, 활성화 [!DNL Workfront DAM] Workfront에서 메타데이터 매핑 프로세스에 대한 필드를 매핑할 수 있습니다. 사용 방법에 대한 자세한 정보 [!DNL Workfront DAM]를 참조하십시오. [메타데이터를에 보내도록 Workfront 구성 [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

구성하려면 [!DNL Workfront] 메타데이터를 로 보냅니다. [!DNL Workfront DAM]:

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 문서]** > **[!UICONTROL 메타데이터 매핑]**.

1. 에서 **[!UICONTROL 매핑할 소스 필드 선택]** 필드에서 매핑할 Workfront 필드의 이름을 입력합니다 [!DNL Workfront DAM]그런 다음 목록에 표시되면 선택합니다.
1. 에서 **[!UICONTROL 매핑할 Target 필드 선택]**&#x200B;에서 을(를) 선택합니다. [!DNL Workfront DAM] 입력하려는 필드 [!DNL Workfront] 필드.

   >[!NOTE]
   >
   > 보낸 모든 문서 [!DNL Workfront DAM] 그렇게 할 수 있는 권한이 있는 사용자가 자신의 메타데이터를 [!DNL Workfront] 필드가 업로드되면 여기에 매핑된 필드 [!DNL Workfront DAM].

1. 클릭 **[!UICONTROL 매핑 추가]**.

1. 계속 추가 [!UICONTROL Workfront] 필드 및 해당 [!DNL Workfront DAM] 필드.

### 매핑된 필드 삭제

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 확장 **[!UICONTROL 문서]**&#x200B;를 클릭한 다음 **[!UICONTROL 메타데이터 매핑]**.

1. 필드 목록에서 메타데이터 매핑에서 제거할 필드를 선택합니다.
1. 클릭 **[!UICONTROL 삭제]**.

   필드는 메타데이터 매핑에서 제거되고 필드에 포함된 정보는 로 전송되지 않습니다 [!DNL Workfront DAM] 업로드한 문서 사용.
