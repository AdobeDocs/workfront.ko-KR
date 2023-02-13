---
title: 향상된 커넥터와 자산 및 폴더를 연결합니다
description: Experience Manager Assets의 자산 또는 폴더를 문서를 지원하는 모든 Workfront 개체에 연결할 수 있습니다.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 향상된 커넥터와 자산 및 폴더를 연결합니다

Experience Manager Assets의 자산 또는 폴더를 문서를 지원하는 모든 Workfront 개체에 연결할 수 있습니다. Experience Manager Assets에서 보낸 자산은 Workfront의 전체 문서 저장소에 포함되지 않습니다. Workfront에서 Experience Manager Assets으로 업로드되고 전송된 문서는 전체 스토리지에 포함됩니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서에서 액세스 이상의 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에

* Experience Manager Enhanced Connector용 Workfront 설치

## Experience Manager Assets에서 자산 연결

Experience Manager Assets에서 Workfront으로 자산을 연결할 수 있습니다. 자산이 연결되면 다음 작업을 수행할 수 있습니다

* [Experience Manager Assets에 연결된 자산 증명](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [문서의 새 버전 업로드](../../../documents/managing-documents/upload-new-document-version.md)

자산을 Experience Manager Assets에 연결하려면

1. 로 이동합니다. **문서** Workfront에서 문서를 추가할 영역.
1. 클릭 **새로 추가**&#x200B;그런 다음 관리자가 설정한 Experience Manager Assets 통합을 선택합니다.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름이 선택될 수 있으므로 Experience Manager Assets에 대해서는 구체적으로 언급되지 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![](assets/select-an-asset.png)

1. 클릭 **링크**.

## Experience Manager Assets에서 폴더 연결

폴더 내의 개별 자산을 볼 수 있는 권한은 Experience Manager Assets 권한에 따라 다릅니다.

폴더를 Experience Manager Assets에 연결하려면

1. 로 이동합니다. **문서** Workfront에서 문서를 추가할 영역.
1. 클릭 **새로 추가**&#x200B;그런 다음 관리자가 설정한 Experience Manager Assets 통합을 선택합니다.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름이 선택될 수 있으므로 Experience Manager Assets에 대해서는 구체적으로 언급되지 않을 수 있습니다.

1. 원하는 폴더를 선택합니다.

   ![](assets/select-a-folder.png)

1. 클릭 **링크**.

## Experience Manager Assets에서 새 버전 연결

Experience Manager Assets에서 새 자산을 가져와 Workfront의 새 버전으로 기존 자산에 추가할 수 있습니다. 문서가 이미 연결되어 있고 새 버전이 Experience Manager Assets에 추가되면 새 버전이 Workfront에 자동으로 나타납니다.

>[!TIP]
>
>로 이동하면 자산의 모든 버전을 볼 수 있습니다 **문서 세부 정보** > **버전**.

Experience Manager Assets에서 새 버전을 연결하려면

1. 로 이동합니다. **문서** Workfront에서 문서를 추가할 영역.
1. 바꿀 자산을 새 버전으로 선택합니다. 연결된 폴더에 자산의 새 버전을 만들 수 없습니다.
1. 클릭 **새로 추가**&#x200B;그런 다음 관리자가 설정한 Experience Manager Assets 통합을 선택합니다.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름이 선택될 수 있으므로 Experience Manager Assets에 대해서는 구체적으로 언급되지 않을 수 있습니다.

1. 원하는 자산을 선택합니다.

   ![](assets/select-an-asset.png)

1. 클릭 **링크**.
