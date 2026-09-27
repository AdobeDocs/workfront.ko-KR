---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 액세스 수준에서 외부 사용자 라이선스 유형 누락
description: 설정의 액세스 수준에 외부 사용자 라이선스 유형이 더 이상 표시되지 않습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
TQID: 'https://experienceleague.adobe.com/g65Yq7r0Hvr6ZyC2niVw4Dnbil37epPeoyfQVOWOiy8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 14%
---
# 액세스 수준에서 외부 사용자 라이선스 유형 누락

## 문제

설정의 액세스 수준에 외부 사용자 라이선스 유형이 더 이상 표시되지 않습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 솔루션

1. **[!UICONTROL 설정]** > **[!UICONTROL 시스템]** > **[!UICONTROL 환경 설정]**(으)로 이동합니다.

1. **[!UICONTROL 보안]** 섹션에서 **[!UICONTROL 전자 메일 주소를 사용하여 Workfront 계정이 없는 사람들과 공동 작업]** 옵션이 활성화되어 있는지 확인하십시오.

   이 옵션을 활성화하지 않으면 외부 사용자가 액세스 수준 설정에 나타나지 않습니다.
