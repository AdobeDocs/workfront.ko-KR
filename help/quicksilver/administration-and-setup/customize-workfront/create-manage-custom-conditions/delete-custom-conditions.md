---
title: 사용자 지정 조건 삭제
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 사용자 지정 조건을 삭제할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 사용자 지정 조건 삭제

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 지정 조건 삭제

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **프로젝트 환경 설정** > **조건**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. 객체 유형의 탭을 선택합니다(**프로젝트**, **작업**, 또는 **문제**)에서 삭제할 조건을 찾습니다.

1. 삭제할 조건을 마우스로 가리킨 다음, **삭제** 아이콘 ![](assets/delete.png) 그것은 맨 오른쪽에 나타납니다.
1. 표시되는 확인 메시지에서 **조건 삭제**.

1. 에서 **조건 삭제** 상자가 표시되면 삭제 중인 조건을 사용하고 있는 모든 프로젝트의 드롭다운 목록에서 새 조건을 선택합니다.

   사용자 지정 조건은 삭제하려는 조건과 동일한 기본 제공 조건과 동일한 경우에만 드롭다운 목록에서 사용할 수 있습니다. 예를 들어, 위험 발생 시 와 동일한 조건을 삭제하는 경우 위험 발생 시에도 동일한 사용자 지정 조건만 선택할 수 있습니다.

1. 클릭 **조건 삭제**.

>[!NOTE]
>
>Target, 위험 및 문제가 있는 기본 제공 조건은 삭제할 수 없습니다. 하지만 이름과 색상을 변경할 수 있습니다.

사용자 지정 조건에 대한 자세한 내용은 [사용자 지정 조건](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
