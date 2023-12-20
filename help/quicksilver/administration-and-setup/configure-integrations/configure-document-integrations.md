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
source-git-commit: ae063189eebb17a3341aabb978ee0f0e03d1e299
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 1%

---

# 문서 통합 구성

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

(으)로 [!DNL Adobe Workfront] 관리자:에서 문서를 관리하도록 문서 통합을 구성할 수 있습니다. [!UICONTROL Workfront]. 다음을 구성할 수도 있습니다. [!UICONTROL Workfront] 문서가 document services 응용 프로그램에만 저장되고 에는 저장되지 않도록 [!UICONTROL Workfront] 그 자체. 자세한 내용은 [에서 문서 업데이트 및 연결 [!UICONTROL Workfront] 외부 클라우드 공급자에게](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) 위치: [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>간의 열린 통신을 허용하려면 [!DNL Workfront Proof] 및 [!DNL Workfront] 서버에 특정 IP 주소를 허용 목록에 추가하다에 추가해야 할 수 있습니다. 자세한 내용은 [허용 목록에 추가하다 방화벽 구성](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 액세스 요구 사항

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음이어야 합니다: [!DNL Workfront] 관리자. 다음에 대한 정보: [!DNL Workfront] 관리자, 참조 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 지원되는 통합

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

문서 관리를 위해 다음 통합을 구성할 수 있습니다.

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  다음에서 증명 연결 [!DNL Workfront Proof] 을 사용하면 원래 내에서 만들어진 증명을 만들 수 있습니다. [!DNL Workfront Proof] 다음 범위 내에서 사용 가능 [!DNL Workfront]. 현재 플랜의 경우 [!UICONTROL Pro] [!DNL Workfront] 이 기능을 사용하려면 계획 이상이 필요합니다. 새 플랜의 경우 이 기능은 모든 플랜에서 사용할 수 있습니다. 사용 가능한 다양한 플랜에 대한 자세한 내용은 [Workfront 플랜](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  와 통합에 대한 자세한 내용 [!DNL SharePoint], 참조 [구성 [!DNL SharePoint] 통합](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* 타사 클라우드 문서 공급자:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google 드라이브]

     <!--Quip-->
  >[!TIP]
  >
  >에 바로 업로드된 문서를 증명하고 승인하는 것과 동일한 방식으로 외부 클라우드 공급자에서 연결된 문서를 증명하고 승인할 수 있습니다 [!DNL Workfront].

* 기타 문서 공급자(사용자 지정 문서 통합을 통해).

  현재 플랜의 경우 [!UICONTROL Pro] [!DNL Workfront] 이 기능을 사용하려면 계획 이상이 필요합니다. 새 플랜의 경우 이 기능은 모든 플랜에서 사용할 수 있습니다. 사용 가능한 다양한 플랜에 대한 자세한 내용은 [Workfront 플랜](https://www.workfront.com/plans).

또한 다음을 향상시킬 수 있습니다 [!DNL Workfront] 기본 DAM(디지털 에셋 관리) 시스템 또는 타사 DAM 통합을 사용하여 경험을 문서화합니다. 사용자가 서비스에 연결하려면 관리자가 이러한 기능을 활성화해야 합니다. [!DNL Workfront] 계정입니다. Workfront DAM에 대한 자세한 내용은 [를 사용하여 문서 관리 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## 문서 관리를 위한 통합 구성

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 클라우드 공급자].**

1. (선택 사항) 가 아닌 문서 서비스 응용 프로그램에 저장된 문서에 [!DNL Workfront], 선택 **[!UICONTROL 사용자가 문서를 저장할 수 없도록 방지 [!DNL Workfront]].**

1. 활성화하고자 하는 통합을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

과의 통합을 설정하는 경우 [!DNL Workfront DAM], 을 활성화할 수 있습니다. [!DNL Workfront] 문서에 메타데이터를 포함합니다. 메타데이터 매핑에 대한 자세한 내용은 [메타데이터 매핑 설정](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## 사용자 정의 문서 통합 구성

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

사용자 정의 문서 통합은 [!DNL Workfront] 파일을 링크할 사용자 [!DNL Workfront] 실제로 모든 시스템에서 사용됩니다(시스템이 작동하는 경우). [!DNL Workfront].

사용자가 사용자 정의 통합을 사용할 수 있도록 하려면 먼저 통합을 빌드해야 합니다. 사용할 통합을 구축하는 방법에 대한 정보 [!DNL Workfront], 참조 [문서 웹후크 API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

사용자 정의 문서 통합이 빌드되면 사이트의 사용자가 사용할 수 있도록 할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 문서]** > **[!UICONTROL 사용자 정의 통합]**.

1. 클릭 **[!UICONTROL 사용자 정의 통합 추가]**.
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
      <td>API 호출을 위한 기본 HTTP 또는 보안 HTTP URL입니다. For example, <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 인증 유형]</td> 
      <td> <p>사용자 지정 통합에 승인된 API를 호출할 때 사용할 인증 방법입니다.</p> 
       <ul> 
        <li>다음을 선택하는 경우 <strong>[!UICONTROL OAuth]</strong>을 클릭하고 5단계를 계속 진행합니다.</li> 
        <li>다음을 선택하는 경우 <strong>[!UICONTROL ApiKey]</strong>를 클릭하고 6단계를 계속합니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) (선택한 경우) **[!UICONTROL OAuth]** 인증 **[!UICONTROL 인증 유형]**&#x200B;를 클릭하고 다음 정보를 입력합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 인증 URL]</td> 
      <td>사용자 인증에 사용되는 전체 URL. [!DNL Workfront] OAuth 프로비저닝 프로세스의 일부로 이 주소로 사용자를 탐색합니다.</td> 
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
      <td> <p>모든 API 호출의 쿼리 문자열에 추가할 선택적 값을 입력합니다. 예: access_type=offline.</p> <p>여러 요청 매개 변수를 추가하려면 <strong>+요청 매개 변수 추가</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >다음 [!DNL Workfront] 맨 아래에 표시되는 리디렉션 URI [!UICONTROL 사용자 정의 통합] 이 통합을 외부 문서 공급자에 등록하는 데 사용되는 URI가 페이지에 나열됩니다.

1. (조건부) (선택한 경우) **[!UICONTROL ApiKey]** 인증 **[!UICONTROL 인증 유형]**&#x200B;사용자 정의 문서 공급자가 발급한 API 키를 입력합니다.

   [!DNL Workfront] 은 이 API 키를 사용하여 문서 공급자에 대해 승인된 API를 호출합니다.

1. 클릭 **[!UICONTROL 저장]** 을 클릭하여 통합을 생성합니다.

## 문서 통합 사용

를 사용하는 방법에 대한 자세한 내용 [!DNL Workfront DAM], 참조 [를 사용하여 문서 관리 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

사용자가 증명을 사용할 수 있는 방법에 대한 자세한 내용은 [증명 만들기](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

사용자가 서드파티 문서 통합을 구성한 후 이를 사용할 수 있는 방법에 대한 자세한 내용은 [외부 애플리케이션에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 구성 [!DNL Workfront] 메타데이터를 보낼 대상 [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

에서 문서를 보낼 때 [!DNL Workfront] 끝 [!DNL Workfront DAM]를 사용하여 해당 문서와 관련된 정보를 보낼 수도 있습니다. 문서에 대한 정보가 매핑됩니다. [!DNL Workfront DAM] 메타데이터로.

정보는 다음 위치에서 한 방향으로만 매핑됩니다. [!DNL Workfront] 끝 [!DNL Workfront DAM] 그리고 문서를 (으)로 업로드할 때만 전송됩니다 [!DNL Workfront DAM]. Workfront 필드를 변경해도 의 메타데이터 필드는 업데이트되지 않습니다. [!DNL Workfront DAM] 문서가 이미 업로드된 후.\
동일한 항목을 매핑할 수 있습니다 [!DNL Workfront] 다양한 분야 [!DNL Workfront DAM] 필드이지만 동일한 필드는 사용할 수 없습니다. [!DNL Workfront DAM] 다중 필드 [!DNL Workfront] 필드.

여러 을(를) 구성해야 하는 경우 [!DNL Workfront] 1로 내보낼 필드 [!DNL Workfront DAM] 필드, 먼저 계산된 사용자 정의 필드를 [!DNL Workfront] 을 눌러 객체의 모든 개별 사용자 정의 필드를 표시합니다. 그런 다음 계산된 지표를 매핑합니다 [!DNL Workfront] 필드 대 1 [!DNL Workfront DAM] 필드.\
계산된 사용자 정의 필드에 대한 자세한 내용은 [사용자 정의 양식에 계산된 데이터 추가](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

매핑은 모든 사용자가 업로드한 모든 문서에 영향을 줍니다 [!DNL Workfront] 끝 [!UICONTROL Workfront] DAM.

로서의 [!DNL Workfront] 관리자, 다음을 활성화해야 합니다. [!DNL Workfront DAM] Workfront에서 메타데이터 매핑 프로세스에 대한 필드를 매핑할 수 있습니다.

구성하려면 [!DNL Workfront] 메타데이터를 보낼 대상 [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. 클릭 **[!UICONTROL 문서]** > **[!UICONTROL 메타데이터 매핑]**.

1. 다음에서 **[!UICONTROL 매핑을 위한 소스 필드 선택]** 필드에서 매핑할 Workfront 필드의 이름을 입력하십시오. [!DNL Workfront DAM]를 클릭한 다음 목록에 표시되면 선택합니다.
1. 다음에서 **[!UICONTROL 매핑할 대상 필드 선택]**&#x200B;를 선택하고 [!DNL Workfront DAM] 선택한 항목의 정보로 채울 필드 [!DNL Workfront] 필드.

   >[!NOTE]
   >
   > 모든 문서가 (으)로 전송됨 [!DNL Workfront DAM] 권한이 있는 사용자가 메타데이터가 [!DNL Workfront] 여기에 매핑된 필드, 업로드할 때 [!DNL Workfront DAM].

1. 클릭 **[!UICONTROL 매핑 추가]**.

1. 계속 추가 [!UICONTROL Workfront] 필드 및 해당 [!DNL Workfront DAM] 필드.

### 매핑된 필드 삭제

{{step-1-to-setup}}

1. 확장 **[!UICONTROL 문서]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 메타데이터 매핑]**.

1. 필드 목록에서 메타데이터 매핑에서 제거할 필드를 선택합니다.
1. 클릭 **[!UICONTROL 삭제]**.

   필드는 메타데이터 매핑에서 제거되고 필드에 포함된 정보는에 전송되지 않습니다. [!DNL Workfront DAM] 업로드한 문서를 사용합니다.
