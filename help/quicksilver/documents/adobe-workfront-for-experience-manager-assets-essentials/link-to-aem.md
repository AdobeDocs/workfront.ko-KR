---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials에서 에셋 및 폴더 연결
description: Experience Manager Assets 또는 Assets Essentials의 에셋 또는 폴더를 문서를 지원하는 모든 Adobe Workfront 개체에 연결할 수 있습니다. Assets Essentials에서 전송된 Assets은 Workfront의 전체 문서 스토리지에 포함되지 않습니다. Workfront에서 Assets Essentials로 업로드되고 전송되는 문서는 전체 스토리지에 포함됩니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Experience Manager Assets 또는 Assets Essentials에서 에셋 및 폴더 연결

Experience Manager Assets 또는 Assets Essentials의 에셋 또는 폴더를 문서를 지원하는 모든 Adobe Workfront 개체에 연결할 수 있습니다. Assets Essentials에서 전송된 Assets은 Workfront의 전체 문서 스토리지에 포함되지 않습니다. Workfront에서 Assets Essentials로 업로드되고 전송되는 문서는 전체 스토리지에 포함됩니다.

메타데이터 필드는 에셋을 Workfront에서 Experience Manager Assets 또는 Assets Essentials로 전송할 때 먼저 매핑됩니다. Workfront 관리자가 오브젝트 메타데이터 동기화를 활성화한 경우 두 애플리케이션에서 변경된 필드가 최신 상태로 유지됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p> 임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials가 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager 권한</td> 
    <td>폴더에 대한 쓰기 액세스 권한이 있어야 합니다.</td> 
   </tr>
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 전제 조건

시작하기 전에,

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

## Experience Manager Assets 또는 Assets Essentials에서 에셋 연결

Experience Manager Assets 또는 Assets Essentials에서 Workfront에 에셋을 연결할 수 있습니다. 자산이 연결되면 다음과 같은 작업을 수행할 수 있습니다.

* [Experience Manager Assets 또는 Assets Essentials에 대해 연결된 에셋 증명](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [새 문서 버전 업로드](../../documents/managing-documents/upload-new-document-version.md)

1. 문서를 추가할 Workfront의 **문서** 영역으로 이동합니다.
1. **새로 추가**&#x200B;를 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택하십시오.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Assets 또는 Assets Essentials에 대해 구체적으로 언급하지 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![자산 선택](assets/select-an-asset.png)

1. **선택**&#x200B;을 클릭합니다.

## Experience Manager Assets 또는 Assets Essentials에서 폴더 연결

폴더 내의 개별 에셋을 볼 수 있는 권한은 Experience Manager Assets 또는 Assets Essentials 권한을 기반으로 합니다.

1. 폴더를 원하는 Workfront의 **문서** 영역으로 이동합니다.
1. **새로 추가**&#x200B;를 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택하십시오.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Assets 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

1. 원하는 폴더를 선택합니다.

   ![폴더 선택](assets/select-a-folder.png)

1. **선택**&#x200B;을 클릭합니다.

## Experience Manager Assets 또는 Assets Essentials에서 새 버전 연결

Assets Essentials에서 새 에셋을 가져와서 기존 에셋에 새 버전으로 추가할 수 있습니다. 문서가 이미 연결되어 있고 Assets Essentials에 새 버전이 추가되어 있는 경우 새 버전이 Workfront에 자동으로 표시됩니다.

Assets Essentials에서 새 버전을 연결하려면 다음을 수행하십시오.

1. 문서를 추가할 Workfront의 **문서** 영역으로 이동합니다.
1. 새 버전으로 바꿀 자산을 선택합니다. 연결된 폴더에 자산의 새 버전을 만들 수 없습니다.
1. **새로 추가** > **버전**&#x200B;을 선택한 다음 관리자가 설정한 Experience Manager 통합을 선택합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Assets 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![자산 선택](assets/select-an-asset.png)

1. **선택**&#x200B;을 클릭합니다.

>[!TIP]
>
>**문서 세부 정보** > **버전**(으)로 이동하면 자산의 모든 버전을 볼 수 있습니다.
