---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Experience Manager Assets 또는 Assets Essentials과 연결된 폴더 만들기
description: Workfront에서 Experience Manager Assets 또는 Assets Essentials과 연결된 폴더를 만들 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Experience Manager Assets 또는 Assets Essentials과 연결된 폴더 만들기

Workfront에서 Experience Manager Assets 또는 Assets Essentials과 연결된 폴더를 만들 수 있습니다. 폴더가 연결되어 있으므로 폴더에 추가된 모든 자산은 Workfront과 Experience Manager 모두에 자동으로 표시됩니다. 연결된 폴더에 있는 경우 자산을 수동으로 보낼 필요가 없습니다.


## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>Adobe Workfront 플랜*</strong>
   </td>
   <td>모든
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront 라이선스*</strong>
   </td>
   <td>플랜
   </td>
  </tr>
  <tr>
   <td><strong>제품</strong>
   </td>
   <td>Experience Manager Assets as a Cloud Service 또는 Assets Essentials이 있어야 하며, 사용자로 제품에 추가되어야 합니다.
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager 권한</strong>
   </td>
   <td>Experience Manager 통합에서 대상 폴더에 대한 쓰기 액세스 권한이 있어야 합니다.
   </td>
  </tr>
  <tr>
   <td><strong>액세스 수준 구성</strong>
   </td>
   <td>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 <strong>사용자에게 전체 관리자 액세스 권한 부여</strong>.
   </td>
  </tr>
</table>


*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.


## 전제 조건

시작하기 전에

* Workfront 관리자가 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## 연결된 폴더 만들기

연결된 폴더는 통합을 설정할 때 Workfront 관리자가 지정한 위치에 만들어집니다. 각 통합에는 연결된 폴더에 대해 폴더 위치가 하나만 있을 수 있습니다.

연결된 폴더의 이름은 연결된 Portfolio, 프로그램, 프로젝트를 기반으로 자동으로 만들어지며 변경할 수 없습니다. 프로젝트가 Portfolio 또는 프로그램과 연결되어 있지 않으면 연결된 폴더에 프로젝트 이름과 작성 날짜가 표시됩니다.

연결된 폴더를 만들려면:



1. 폴더를 원하는 프로젝트로 이동합니다.
1. 선택 **새로 추가**&#x200B;그런 다음 관리자 설정 Experience Manager 통합으로 이동합니다.
   >[!NOTE]
   >
   >Workfront 관리자는 이 통합의 이름을 선택할 수 있으므로 Experience Manager Assets 또는 Assets Essentials에 대해 특별히 언급하지는 않을 수 있습니다.

1. 선택 **연결된 폴더 만들기**. 통합을 설정할 때 지정된 위치를 기반으로 Experience Manager에 폴더를 자동으로 만듭니다.
   ![연결된 폴더 만들기](assets/linked-folder.png)
