---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '오류 메시지: SAML 2.0 오류: 사용자 식별자를 찾을 수 없음'
description: ADFS에 성공적으로 연결할 수 없습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
TQID: https://experienceleague.adobe.com/H7-Y9pZ-w4K3iEkJTVeHrx1cJJYXHiIMIvO3VoGYq9g
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 9%

---

# 오류 메시지: SAML 2.0 오류: 사용자 식별자를 찾을 수 없음

## 문제

ADFS에 성공적으로 연결할 수 없습니다.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>성공적인 테스트 연결을 설정했지만 여전히 문제가 발생하는 경우 잘못된 속성 매핑이나 페더레이션 ID에 문제가 발생할 수 있습니다. 문의 사항은 고객 지원 센터에 문의하십시오.

## 원인:

ADFS 서버에 대한 클레임이 잘못되었습니다.

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

ADFS 서버에서 이름 ID에 대한 클레임이 있는지 확인합니다.

1. Windows에서는 **[!UICONTROL 시작]** > **[!UICONTROL 관리]** > **[!UICONTROL ADFS 2.0 관리]**&#x200B;를 클릭합니다.\
   [ADFS 2.0 관리] 대화 상자가 표시됩니다.

1. 왼쪽 창에서 **[!UICONTROL 트러스트 관계]** > **[!UICONTROL 신뢰 당사자 트러스트]**&#x200B;를 선택합니다.

1. Adobe Workfront 관련 신뢰 당사자 트러스트를 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 클레임 규칙 편집]**&#x200B;을 선택합니다.
1. 클레임에 **[!UICONTROL 이름 ID]**&#x200B;의 **[!UICONTROL 나가는 클레임 유형]**&#x200B;이 있는지 확인하십시오.

![1.png](assets/1-350x287.png)
