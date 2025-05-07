---
title: 문서 통합 구성
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Adobe Workfront 관리자는 Workfront에서 문서를 관리하도록 문서 통합을 구성할 수 있습니다.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ec0e2be036ce1298e285ce85cdeddae97cd1f144
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 1%

---

# 문서 통합 구성

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

[!DNL Adobe Workfront] 관리자는 [!UICONTROL Workfront]에서 문서를 관리하도록 문서 통합을 구성할 수 있습니다. 문서가 문서 서비스 응용 프로그램에만 저장되고 [!UICONTROL Workfront] 자체에는 저장되지 않도록 [!UICONTROL Workfront]을(를) 구성할 수도 있습니다. 자세한 내용은 [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)에서 [[!UICONTROL Workfront]에서 외부 클라우드 공급자로 문서 업데이트 및 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider)을 참조하십시오.

>[!NOTE]
>
>[!DNL Workfront Proof]과(와) [!DNL Workfront] 서버 간 통신을 허용하려면 특정 IP 주소를 허용 목록에 추가하다에 추가해야 할 수 있습니다. 허용 목록에 추가하다 자세한 내용은 [방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
       <p>또는</p>
       <p>현재: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 지원되는 통합

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

문서 관리를 위해 다음 통합을 구성할 수 있습니다.

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  [!DNL Workfront Proof]에서 증명을 연결하면 원래 [!DNL Workfront Proof] 내에 만들어진 증명을 [!DNL Workfront] 내에서 사용할 수 있습니다. 현재 플랜의 경우 이 기능을 사용하려면 [!UICONTROL Pro] [!DNL Workfront] 플랜 이상이 필요합니다. 새 플랜의 경우 이 기능은 모든 플랜에서 사용할 수 있습니다. 사용 가능한 다양한 플랜에 대한 자세한 내용은 [Workfront 플랜](https://business.adobe.com/products/workfront/pricing.html)을 참조하십시오.

* [!DNL Microsoft SharePoint]

  [!DNL SharePoint]과(와) 통합에 대한 자세한 내용은 [통합 구성 [!DNL SharePoint] 을(를) 참조하십시오](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* 타사 클라우드 문서 공급자:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google 드라이브]
   * Quip

  >[!TIP]
  >
  >[!DNL Workfront]에 직접 업로드된 문서를 증명하고 승인하는 것과 같은 방식으로 외부 클라우드 공급자에서 연결된 문서를 증명하고 승인할 수 있습니다.

* 기타 문서 공급자(사용자 지정 문서 통합을 통해).

  현재 플랜의 경우 이 기능을 사용하려면 [!UICONTROL Pro] [!DNL Workfront] 플랜 이상이 필요합니다. 새 플랜의 경우 이 기능은 모든 플랜에서 사용할 수 있습니다. 사용 가능한 다양한 플랜에 대한 자세한 내용은 [Workfront 플랜](https://business.adobe.com/products/workfront/pricing.html)을 참조하십시오.

또한 타사 DAM 통합을 통해 [!DNL Workfront] 문서 환경을 개선할 수 있습니다. 사용자가 서비스를 [!DNL Workfront] 계정에 연결하려면 관리자가 이러한 기능을 사용하도록 설정해야 합니다.

## 문서 관리를 위한 통합 구성

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 클라우드 공급자]**&#x200B;를 클릭합니다.

1. (선택 사항) [!DNL Workfront]이(가) 아닌 문서 서비스 응용 프로그램에 문서를 저장하려면 **[!UICONTROL 사용자가 [!DNL Workfront]]에 문서를 저장하지 못하도록 합니다.**

1. 활성화하고자 하는 통합을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

[!DNL Workfront DAM]과의 통합을 설정하는 경우 [!DNL Workfront]에서 문서에 메타데이터를 포함하도록 설정할 수 있습니다. 메타데이터 매핑에 대한 자세한 내용은 [메타데이터 매핑 설정](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md)을 참조하십시오.

## 사용자 정의 문서 통합 구성

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

사용자 정의 문서 통합을 사용하면 [!DNL Workfront] 사용자가 [!DNL Workfront]과(와) 함께 작동하도록 만들어진 경우 실질적으로 모든 시스템에서 [!DNL Workfront]에 파일을 연결할 수 있습니다.

사용자가 사용자 정의 통합을 사용할 수 있도록 하려면 먼저 통합을 빌드해야 합니다. [!DNL Workfront]에 사용할 통합을 만드는 방법에 대한 자세한 내용은 [Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md)를 참조하십시오.

사용자 정의 문서 통합이 빌드되면 사이트의 사용자가 사용할 수 있도록 할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 사용자 지정 통합]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 사용자 지정 통합 추가]**&#x200B;를 클릭합니다.
1. 다음 정보를 입력하여 통합을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>사용자 정의 통합의 이름입니다. 사용자가 Workfront 내에서 통합을 사용할 때 표시되는 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 기본 API URL] </td> 
      <td>API 호출을 위한 기본 HTTP 또는 보안 HTTP URL입니다. For example, <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 인증 유형]</td> 
      <td> <p>사용자 지정 통합에 승인된 API를 호출할 때 사용할 인증 방법입니다.</p> 
       <ul> 
        <li><strong>[!UICONTROL OAuth]</strong>을(를) 선택하는 경우 5단계를 계속합니다.</li> 
        <li><strong>[!UICONTROL ApiKey]</strong>을(를) 선택하는 경우 6단계를 계속합니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) **[!UICONTROL 인증 유형]**&#x200B;에 대해 **[!UICONTROL OAuth]** 인증을 선택한 경우 다음 정보를 입력하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 인증 URL]</td> 
      <td>사용자 인증에 사용되는 전체 URL. [!DNL Workfront]은(는) OAuth 프로비저닝 프로세스의 일부로 이 주소로 사용자를 탐색합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 토큰 끝점 URL]</td> 
      <td>OAuth 토큰을 검색하는 데 사용되는 전체 API URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 ID]</td> 
      <td>이 통합을 위한 OAut 클라이언트 ID.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 클라이언트 암호]</td> 
      <td>이 통합을 위한 OAut 클라이언트 암호.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 요청 매개 변수]</td> 
      <td> <p>모든 API 호출의 쿼리 문자열에 추가할 선택적 값을 입력합니다. 예: access_type=offline.</p> <p>여러 요청 매개 변수를 추가하려면 <strong>+요청 매개 변수 추가</strong>를 클릭하십시오.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >[!UICONTROL 사용자 지정 통합] 페이지 하단에 표시되는 [!DNL Workfront] 리디렉션 URI에는 외부 문서 공급자에 이 통합을 등록하는 데 사용된 URI가 나열됩니다.

1. (조건부) **[!UICONTROL 인증 유형]**&#x200B;에 대해 **[!UICONTROL ApiKey]** 인증을 선택한 경우 사용자 지정 문서 공급자가 발급한 API 키를 입력하십시오.

   [!DNL Workfront]은(는) 이 API 키를 사용하여 문서 공급자에 대해 승인된 API를 호출합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭하여 통합을 만듭니다.

## 문서 통합 사용

사용자가 증명을 사용하는 방법에 대한 자세한 내용은 [증명 만들기](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md)를 참조하십시오.

사용자가 서드파티 문서 통합을 구성한 후 이를 사용할 수 있는 방법에 대한 자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)을 참조하십시오.

### [!UICONTROL [!DNL Workfront] DAM] (으)로 메타데이터를 보내도록 [!DNL Workfront] 구성 {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

[!DNL Workfront]에서 [!DNL Workfront DAM]&#x200B;(으)로 문서를 보낼 때 해당 문서와 관련된 정보를 보낼 수도 있습니다. 문서에 대한 정보가 [!DNL Workfront DAM]에 메타데이터로 매핑되어 있습니다.

정보는 [!DNL Workfront]에서 [!DNL Workfront DAM]&#x200B;(으)로 단방향 매핑되며 문서가 [!DNL Workfront DAM]&#x200B;(으)로 업로드될 때만 전송됩니다. 문서가 이미 업로드된 후에는 Workfront 필드를 변경해도 [!DNL Workfront DAM]의 메타데이터 필드가 업데이트되지 않습니다.\
동일한 [!DNL Workfront] 필드를 다양한 [!DNL Workfront DAM] 필드에 매핑할 수 있지만 여러 [!DNL Workfront] 필드에 동일한 [!DNL Workfront DAM] 필드를 사용할 수는 없습니다.

여러 [!DNL Workfront] 필드를 구성하여 하나의 [!DNL Workfront DAM] 필드로 내보내야 하는 경우 먼저 [!DNL Workfront]에서 계산된 사용자 지정 필드를 만들어 개체의 모든 개별 사용자 지정 필드를 표시하십시오. 그런 다음 계산된 [!DNL Workfront] 필드를 하나의 [!DNL Workfront DAM] 필드에 매핑합니다.\
계산된 사용자 지정 필드에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

매핑은 [!DNL Workfront]에서 [!UICONTROL Workfront] DAM으로 사용자가 업로드한 모든 문서에 영향을 줍니다.

[!DNL Workfront] 관리자는 메타데이터 매핑 프로세스에 대한 필드를 매핑하려면 먼저 Workfront에서 [!DNL Workfront DAM]을(를) 활성화해야 합니다.

메타데이터를 [!DNL Workfront DAM]&#x200B;(으)로 보내도록 [!DNL Workfront]을(를) 구성하려면:

{{step-1-to-setup}}

1. **[!UICONTROL 문서]** > **[!UICONTROL 메타데이터 매핑]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 매핑을 위한 Source 필드 선택]** 필드에서 [!DNL Workfront DAM]에 매핑할 Workfront 필드의 이름을 입력한 다음 목록에 표시되면 선택합니다.
1. **[!UICONTROL 매핑할 대상 필드 선택]**&#x200B;에서 선택한 [!DNL Workfront] 필드의 정보로 채울 [!DNL Workfront DAM] 필드를 선택합니다.

   >[!NOTE]
   >
   > 권한이 있는 사용자가 [!DNL Workfront DAM]에게 보낸 모든 문서는 [!DNL Workfront DAM]에 업로드할 때 여기에 매핑된 [!DNL Workfront] 필드로 메타데이터를 업데이트했습니다.

1. **[!UICONTROL 매핑 추가]**&#x200B;를 클릭합니다.

1. [!UICONTROL Workfront] 필드 및 해당 [!DNL Workfront DAM] 필드를 계속 추가합니다.

### 매핑된 필드 삭제

{{step-1-to-setup}}

1. **[!UICONTROL 문서]**&#x200B;를 확장한 다음 **[!UICONTROL 메타데이터 매핑]**&#x200B;을 클릭합니다.

1. 필드 목록에서 메타데이터 매핑에서 제거할 필드를 선택합니다.
1. **[!UICONTROL 삭제]**&#x200B;를 클릭합니다.

   메타데이터 매핑에서 필드가 제거되며 이 필드에 포함된 정보는 업로드된 문서와 함께 [!DNL Workfront DAM]&#x200B;(으)로 전송되지 않습니다.


## 제한 사항

### Google 드라이브 통합

* 연결된 폴더가 Workfront에 추가되면 폴더의 파일이 더 이상 자동으로 추가되지 않습니다.
   * 파일 없이 Google 폴더를 Workfront에 추가한 다음 개별 파일을 Workfront에 추가할 수 있습니다. 파일은 Workfront의 Google 폴더에 자동으로 추가됩니다.
또는
   * Workfront에서 문서 폴더를 만든 다음 Google 폴더에서 모든 파일을 선택하고 Workfront 폴더에 추가할 수 있습니다.


* Google 드라이브 문서 통합은 Google 드라이브의 내 드라이브 영역에서 파일 추가를 지원합니다. 공유 드라이브에서는 폴더나 이미지를 추가할 수 없습니다. [Google 공유 드라이브](https://support.google.com/a/users/answer/7212025?hl=en)에 대해 자세히 알아보세요.
