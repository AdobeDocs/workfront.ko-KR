---
title: 재무 데이터에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 통해 Workfront의 재무 데이터에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 5%

---


# 등급 카드에 대한 액세스 권한 부여

{{highlighted-preview-article-level}}

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 사용자의 액세스 수준을 통해 등급 카드에 대한 사용자의 액세스 권한을 정의할 수 있습니다.

요율 카드에 대한 자세한 내용은 [요율 카드 관리](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td>워크플로 얼티밋</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>표준</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 등급 카드에 대한 액세스 권한 부여에 대한 고려 사항

Workfront에서 등급 카드에 대한 액세스 권한을 사용자에게 부여할 때 다음 사항을 고려하십시오.

* 프로젝트에 비율 카드를 첨부하려면 사용자에게 비율 카드, 프로젝트 및 재무 데이터에 대한 편집 액세스 권한이 있어야 합니다.
* 요금 카드에 대한 액세스 권한이 없고 재무 데이터에 대한 편집 액세스 권한이 있는 사용자는 프로젝트에 요금 카드를 첨부할 수 없지만, 다른 소스에서 온 프로젝트의 다른 청구 요금을 편집할 수 있습니다.

## 사용자 정의 액세스 수준을 사용하여 등급 카드에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 등급 카드 오른쪽의 ![](assets/gear-icon-settings.png)보기&#x200B;**또는**&#x200B;편집&#x200B;**단추에서 톱니바퀴 아이콘**&#x200B;을(를) 클릭한 다음 **설정을 미세 조정**&#x200B;에서 부여할 기능을 선택합니다.

   ![속도 카드 액세스 조정](assets/rate-card-access-fine-tune.png)

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나(예: [작업에 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md))를 계속 사용하십시오.
1. 완료되면 **저장**&#x200B;을 클릭하세요.

   액세스 수준이 만들어지면 사용자에게 이를 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

## 공유 요금 카드에 액세스

[요금 카드 공유](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md)에 설명된 대로 다른 사용자에게 사용 권한을 부여하여 요금 카드를 공유할 수 있습니다.

다른 사용자와 객체를 공유할 때 객체에 대한 수신자의 권한은 다음 두 가지 사항의 조합으로 결정됩니다.

* 객체에 대해 수신자에게 부여하는 권한
* 개체 유형에 대한 수신자의 액세스 수준 설정입니다.
