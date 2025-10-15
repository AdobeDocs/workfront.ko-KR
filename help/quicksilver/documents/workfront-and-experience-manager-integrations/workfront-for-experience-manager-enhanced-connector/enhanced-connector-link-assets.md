---
title: 향상된 커넥터로 에셋 및 폴더 연결
description: Experience Manager Assets의 에셋 또는 폴더를 문서를 지원하는 모든 Workfront 개체에 연결할 수 있습니다.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---


# 향상된 커넥터로 에셋 및 폴더 연결

Experience Manager Assets의 에셋 또는 폴더를 문서를 지원하는 모든 Workfront 개체에 연결할 수 있습니다. Experience Manager Assets에서 보낸 Assets은 Workfront의 전체 문서 스토리지에 포함되지 않습니다. Workfront에서 Experience Manager Assets으로 업로드되고 전송된 문서는 전체 스토리지에 포함됩니다.


>[!NOTE]
>
>향상된 커넥터를 통해 연결된 Excel 파일은 Workfront에서 미리 볼 수 없습니다. 액세스하려면 파일을 다운로드해야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p>
   <p>요청 이상</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 제품</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서에 대한 액세스 권한 이상 보기</p> </td> 
  </tr> 
 </tbody> 
</table>


자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 다음을 수행해야 합니다

* Workfront for Experience Manager 강화 커넥터 설치

## Experience Manager Assets에서 에셋 연결

Experience Manager Assets에서 Workfront으로 자산을 연결할 수 있습니다. 자산이 연결되면 다음과 같은 작업을 수행할 수 있습니다.

* [Experience Manager Assets에 대해 연결된 자산 증명](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [새 문서 버전 업로드](../../../documents/managing-documents/upload-new-document-version.md)

Experience Manager Assets에 자산을 연결하려면 다음 작업을 수행하십시오.

1. 문서를 추가할 Workfront의 **문서** 영역으로 이동합니다.
1. **새로 추가**&#x200B;를 클릭한 다음 관리자가 설정한 Experience Manager Assets 통합을 선택하십시오.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름을 선택할 수 있으므로 Experience Manager Assets에 대해 구체적으로 언급되지 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![자산 선택](assets/select-an-asset.png)

1. **링크**&#x200B;를 클릭합니다.

## Experience Manager Assets에서 폴더 연결

폴더 내의 개별 에셋을 볼 수 있는 권한은 Experience Manager Assets 권한에 따라 다릅니다.

폴더를 Experience Manager Assets에 연결하려면 다음을 수행하십시오.

1. 문서를 추가할 Workfront의 **문서** 영역으로 이동합니다.
1. **새로 추가**&#x200B;를 클릭한 다음 관리자가 설정한 Experience Manager Assets 통합을 선택하십시오.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름을 선택할 수 있으므로 Experience Manager Assets에 대해 구체적으로 언급되지 않을 수 있습니다.

1. 원하는 폴더를 선택합니다.

   ![폴더 선택](assets/select-a-folder.png)

1. **링크**&#x200B;를 클릭합니다.

## Experience Manager Assets에서 새 버전 연결

Experience Manager Assets에서 새 자산을 가져와서 기존 자산에 Workfront의 새 버전으로 추가할 수 있습니다. 문서가 이미 연결되어 있고 Experience Manager Assets에 새 버전이 추가되어 있으면 새 버전이 Workfront에 자동으로 표시됩니다.

>[!TIP]
>
>**문서 세부 정보** > **버전**(으)로 이동하면 자산의 모든 버전을 볼 수 있습니다.

Experience Manager Assets에서 새 버전을 연결하려면 다음을 수행하십시오.

1. 문서를 추가할 Workfront의 **문서** 영역으로 이동합니다.
1. 새 버전으로 바꿀 자산을 선택합니다. 연결된 폴더에 자산의 새 버전을 만들 수 없습니다.
1. **새로 추가**&#x200B;를 클릭한 다음 관리자가 설정한 Experience Manager Assets 통합을 선택하십시오.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름을 선택할 수 있으므로 Experience Manager Assets에 대해 구체적으로 언급되지 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![자산 선택](assets/select-an-asset.png)

1. **링크**&#x200B;를 클릭합니다.
