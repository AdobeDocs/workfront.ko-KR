---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 향상된 커넥터를 사용하여 문서 보내기
description: Workfront에서 Experience Manager Assets으로 문서를 보낼 수 있습니다. Workfront에서 Experience Manager Assets으로 업로드되고 전송된 문서는 전체 문서 저장소에 대해 계속 계산됩니다. Experience Manager Assets에서 연결된 자산은 전체 스토리지에 포함되지 않습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# 향상된 커넥터를 사용하여 문서 보내기

Workfront에서 Experience Manager Assets으로 문서를 보낼 수 있습니다. Workfront에서 Experience Manager Assets으로 업로드되고 전송된 문서는 전체 문서 저장소에 대해 계속 계산됩니다. Experience Manager Assets에서 연결된 자산은 전체 스토리지에 포함되지 않습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
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
   <td> <p>문서에서 액세스 수준 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에

* Experience Manager Enhanced Connector용 Workfront을 설치합니다.

## Experience Manager Assets으로 문서 보내기

사용자가 Workfront에서 Experience Manager Assets으로 문서를 전송하면 매핑된 메타데이터가 문서에 따라 전송됩니다. 구성된 경우, 변경 사항이 있을 때마다 메타데이터가 지속적으로 동기화됩니다.

문서를 보내려면

1. 로 이동합니다. **문서** Workfront에서 영역을 선택하고 전송할 문서를 선택합니다.
1. 클릭 **보내기**&#x200B;그런 다음 관리자가 설정한 Experience Manager Assets 통합을 선택합니다.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름이 선택될 수 있으므로 Experience Manager Assets에 대해서는 구체적으로 언급되지 않을 수 있습니다.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 자산을 이동할 위치를 선택하고 을 클릭합니다 **폴더 선택**.
1. 원하는 대상을 찾으면 을 클릭합니다 **저장**.

## Experience Manager Assets에 새 버전 보내기

이전에 Workfront에 업로드한 문서에 새 버전을 추가할 수 있습니다. 자세한 내용은 [문서의 새 버전 업로드](../../../documents/managing-documents/upload-new-document-version.md). 최신 버전이 업로드되면 Experience Manager Assets으로 보낼 수 있습니다. Workfront의 매핑된 필드가 변경되면 새 버전이 Experience Manager Assets을 전송할 때 메타데이터를 업데이트합니다.

최신 버전을 보내려면

1. 로 이동합니다. **문서** Workfront에서 영역을 설정하고 문서를 찾습니다.
1. 클릭 **보내기**&#x200B;그런 다음 관리자가 설정한 Experience Manager Assets 통합을 선택합니다.

   >[!NOTE]
   >
   >이 통합을 위해 모든 이름이 선택될 수 있으므로 Experience Manager Assets에 대해서는 구체적으로 언급되지 않을 수 있습니다.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. **저장**&#x200B;을 클릭합니다. 새 버전이 이전 버전과 동일한 위치에 저장됩니다.
