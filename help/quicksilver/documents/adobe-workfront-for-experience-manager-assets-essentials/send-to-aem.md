---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials로 문서 보내기
description: Workfront에서 Experience Manager Assets 또는 Assets Essentials로 문서를 전송할 수 있습니다. Workfront에서 Assets Essentials로 업로드되고 전송된 문서는 여전히 전체 문서 스토리지에 대해 계산됩니다. Assets Essentials에서 연결된 Assets은 전체 스토리지에 포함되지 않습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 2%

---

# Experience Manager Assets 또는 Assets Essentials로 문서 보내기

Workfront에서 Experience Manager Assets 또는 Assets Essentials로 문서를 전송할 수 있습니다. Workfront에서 Assets Essentials로 업로드되고 전송된 문서는 여전히 전체 문서 스토리지에 대해 계산됩니다. Assets Essentials에서 연결된 Assets은 전체 스토리지에 포함되지 않습니다.

이 통합을 통해 Experience Manager으로 전송된 Assets의 크기 제한은 **5GB**&#x200B;입니다.

미리보기 환경에서 이 통합을 통해 Experience Manager으로 전송된 Assets의 크기 제한은 **30GB**&#x200B;입니다.

>[!NOTE]
>
>이 기능은 새 문서 영역에서 사용할 수 없습니다.<br>
>조직에서 엔터프라이즈 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. 거기에서 Experience Manager Assets으로 에셋을 보낼 수 있습니다. 자세한 내용은 [Frame.io 통합에 Adobe Experience Manager 사용](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)을 참조하십시오.

## 메타데이터

메타데이터 필드는 에셋을 Workfront에서 Experience Manager Assets 또는 Assets Essentials로 전송할 때 먼저 매핑됩니다. 상위 개체에 대해 매핑하도록 구성된 메타데이터도 전송됩니다. 메타데이터 매핑 구성에 대한 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

>[!INFO]
>
>**예** 작업에 첨부된 에셋을 처음 보낼 때 작업 메타데이터는 프로젝트, 포트폴리오 및 프로그램과 같은 상위 개체의 매핑된 메타데이터뿐만 아니라 Experience Manager Assets 또는 Assets Essentials에도 매핑됩니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials가 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager 권한</td> 
    <td>폴더에 대한 쓰기 액세스 권한이 있어야 합니다.</td> 
   </tr>
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>View access or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

Before you begin,

* Your Workfront Administrator must configure an Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) or [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Send a Document from Workfront

When a user sends a document from Workfront to Experience Manager Assets or Assets Essentials, mapped metadata transfers along the document. After the document is sent, changes made to the document&#39;s metadata in Workfront are not reflected in Assets or Assets Essentials. If a mapped field in Workfront is changed, you must send a new version of the document with the updated metadata to Assets or Assets Essentials. To set up or edit metadata, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) or [Configure the Experience Manager Assets Essentials integration](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

To send a document:

1. Go to the **Documents** area in Workfront, and select the document you want to send.
1. Click **Send to**, then choose the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Assets or Assets Essentials.

   ![Send to](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Choose where you want the asset to go, then click **Select Folder**.
1. When you find your desired destination, click **Save**.

## Send a new version

You can add a new version to a document you have previously uploaded to Workfront. For more information, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to Assets Essentials. If a mapped field in Workfront has changed, the new version updates the metadata in Assets Essentials when it sends.

>[!IMPORTANT]
>
>Before you upload a new version to Workfront, we recommend renaming the file. 이전 버전과 정확히 동일한 파일 이름의 새 버전을 업로드하는 경우 Workfront에서 가장 최근 버전만 다운로드할 수 있습니다. 파일 이름과 관계없이 Experience Manager Assets 또는 Assets Essentials에서 모든 버전을 다운로드할 수 있습니다.

최신 버전을 보내려면

1. Workfront의 **문서** 영역으로 이동하여 문서를 찾습니다.
1. **전송 대상**&#x200B;을 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택하십시오.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Assets 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

   ![전송 대상](assets/copy-of-send-to-in-toolbar-350x149.png)

1. **저장**&#x200B;을 클릭합니다. 새 버전이 이전 버전과 동일한 위치에 저장됩니다.

## Experience Manager Assets에서 연결된 폴더로 문서 이동

>[!NOTE]
>
>이 기능은 Experience Manager Assets as a Cloud Service에서만 사용할 수 있습니다. Experience Manager Assets Essentials에서는 사용할 수 없습니다.

문서와 연결된 폴더가 모두 동일한 문서 목록(예: 프로젝트의 문서 영역)에 있는 경우 문서를 Experience Manager Assets의 연결된 폴더로 이동할 수 있습니다.

1. 이동할 문서를 찾습니다.
1. 이동할 연결된 Experience Manager Assets 폴더로 문서를 끌어다 놓습니다.

문서를 이동하는 동안에는 문서 옵션을 사용할 수 없습니다. 문서가 Experience Manager Assets으로 이동되면 은 더 이상 Workfront의 문서 목록에 표시되지 않습니다.

>[!NOTE]
>
> 문서를 이동하는 동안 문서에 대해 수행한 작업이나 편집 내용은 Experience Manager Assets의 문서에 표시되지 않으므로 손실됩니다.

