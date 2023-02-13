---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials에서 자산 및 폴더 연결
description: Experience Manager Assets 또는 Assets Essentials의 자산이나 폴더를 문서를 지원하는 모든 Adobe Workfront 개체에 연결할 수 있습니다. Assets Essentials에서 보낸 자산은 Workfront의 전체 문서 저장소에 포함되지 않습니다. Workfront에서 Assets Essentials으로 업로드되고 전송되는 문서는 전체 스토리지에 포함됩니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Experience Manager Assets 또는 Assets Essentials에서 자산 및 폴더 연결

Experience Manager Assets 또는 Assets Essentials의 자산이나 폴더를 문서를 지원하는 모든 Adobe Workfront 개체에 연결할 수 있습니다. Assets Essentials에서 보낸 자산은 Workfront의 전체 문서 저장소에 포함되지 않습니다. Workfront에서 Assets Essentials으로 업로드되고 전송되는 문서는 전체 스토리지에 포함됩니다.

메타데이터 필드는 자산을 Workfront에서 Experience Manager Assets 또는 Assets Essentials으로 보낼 때 먼저 매핑됩니다. Workfront 관리자가 개체 메타데이터 동기화를 활성화한 경우 두 응용 프로그램에서 필드가 변경되면 최신 상태로 유지됩니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p> 모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials이 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager 권한</td> 
    <td>폴더에 대한 쓰기 액세스 권한이 있어야 합니다.</td> 
   </tr>
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에

* Workfront 관리자가 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Experience Manager Assets 또는 Assets Essentials의 자산 연결

Experience Manager Assets 또는 Assets Essentials의 자산을 Workfront에 연결할 수 있습니다. 자산이 연결되면 다음 작업을 수행할 수 있습니다

* [Experience Manager Assets 또는 Assets Essentials에 연결된 자산 증명](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [문서의 새 버전 업로드](../../documents/managing-documents/upload-new-document-version.md)

1. 로 이동합니다. **문서** Workfront에서 문서를 추가할 영역.
1. 선택 **새로 추가**&#x200B;을 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합의 이름을 선택할 수 있으므로 자산 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![](assets/select-an-asset.png)

1. 클릭 **선택**.

## Experience Manager Assets 또는 Assets Essentials의 폴더 연결

폴더 내의 개별 자산을 볼 수 있는 권한은 Experience Manager Assets 또는 Assets Essentials 권한에 따라 다릅니다.

1. 로 이동합니다. **문서** Workfront에서 폴더를 만들 위치입니다.
1. 선택 **새로 추가**&#x200B;을 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합의 이름을 선택할 수 있으므로 자산이나 Assets Essentials에 대해 특별히 언급하지는 않을 수 있습니다.

1. 원하는 폴더를 선택합니다.

   ![](assets/select-a-folder.png)

1. 클릭 **선택**.

## Experience Manager Assets 또는 Assets Essentials의 새 버전 연결

새 자산을 Assets Essentials에서 가져와서 기존 자산에 새 버전으로 추가할 수 있습니다. 문서가 이미 연결되어 있고 새 버전이 Assets Essentials에 추가되면 새 버전이 Workfront에 자동으로 나타납니다.

Assets Essentials에서 새 버전을 연결하려면

1. 로 이동합니다. **문서** Workfront에서 문서를 추가할 영역.
1. 바꿀 자산을 새 버전으로 선택합니다. 연결된 폴더에 자산의 새 버전을 만들 수 없습니다.
1. 선택 **새로 추가** > **버전**&#x200B;을 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합의 이름을 선택할 수 있으므로 자산이나 Assets Essentials에 대해 특별히 언급하지는 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![](assets/select-an-asset.png)

1. 클릭 **선택**.

>[!TIP]
>
>로 이동하면 자산의 모든 버전을 볼 수 있습니다 **문서 세부 정보** > **버전**.
