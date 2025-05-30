---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Experience Manager Assets 또는 Assets Essentials와 연결된 폴더 만들기
description: Workfront에 있는 동안 Experience Manager Assets 또는 Assets Essentials와 연결된 폴더를 만들 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: e9c6a01e80d34bc873c9a06ae0782dc65afb2445
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Experience Manager Assets 또는 Assets Essentials와 연결된 폴더 만들기

Workfront에 있는 동안 Experience Manager Assets 또는 Assets Essentials와 연결된 폴더를 만들 수 있습니다. 폴더가 연결되므로, 폴더에 추가된 모든 자산이 Workfront 및 Experience Manager 모두에 자동으로 표시됩니다. 연결된 폴더에 자산이 있는 경우 수동으로 전송할 필요가 없습니다.

에셋이 Experience Manager Assets 또는 Assets Essentials 내의 연결된 폴더에서 삭제되거나 이동되는 경우 Workfront은 프로젝트 > 문서 영역에 에셋 사본을 유지합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>Adobe Workfront 플랜*</strong>
   </td>
   <td>임의
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
   <td>Experience Manager Assets as a Cloud Service 또는 Assets Essentials가 있어야 하며 제품에 사용자로 추가되어야 합니다.
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
   <td>Experience Manager 통합을 구성하려면 Workfront 관리자여야 합니다. 구성된 후 플랜 라이선스가 있는 사용자는 개별 프로젝트에 연결된 폴더를 설정할 수 있습니다.
   </td>
  </tr>
</table>


*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 전제 조건

시작하기 전에,

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.


## 연결된 폴더 만들기

연결된 폴더는 Workfront 관리자가 통합을 설정할 때 지정한 위치에 만들어집니다. 각 통합에는 연결된 폴더에 대해 하나의 폴더 위치만 있을 수 있습니다.

연결된 폴더의 이름은 Portfolio, 프로그램, 연결된 프로젝트를 기반으로 자동으로 생성되며 변경할 수 없습니다. 프로젝트가 Portfolio 또는 프로그램과 연결되어 있지 않으면 연결된 폴더에 프로젝트 이름과 생성 날짜가 표시됩니다.

>[!NOTE]
>
>연결된 폴더 내에 새 문서 또는 증명 버전을 만들 수 없습니다.


연결된 폴더를 만들려면 다음 작업을 수행하십시오.

1. 폴더를 원하는 프로젝트로 이동합니다.
1. **새로 추가**&#x200B;를 선택한 다음 관리자가 설정한 Experience Manager 통합으로 이동합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 이 통합에 사용할 이름을 선택할 수 있으므로 Experience Manager Assets 또는 Assets Essentials에 대해 특별히 언급하지 않을 수 있습니다.

1. **연결된 폴더 만들기**&#x200B;를 선택합니다. 시스템은 통합 설정 시 지정된 위치를 기반으로 Experience Manager에 폴더를 자동으로 생성합니다.
   ![연결된 폴더 만들기](assets/linked-folder.png)
