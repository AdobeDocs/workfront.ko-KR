---
title: 개체를 변환할 때 사용자 지정 양식 데이터 전송
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 작업 항목에 정의된 작업이 너무 크면 더 큰 작업 항목으로 변환할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 개체를 변환할 때 사용자 지정 양식 데이터 전송

조직의 비즈니스 요구 사항에 따라 작업이나 문제에 정의된 작업이 너무 커서 작업이나 문제 내에서 관리할 수 없을 수 있습니다. 이 경우 이러한 필드를 더 큰 작업 항목으로 변환할 수 있습니다.

* 문제를 작업으로 또는 프로젝트로 변환할 수 있습니다
* 작업을 프로젝트로 변환할 수 있습니다

사용자 지정 양식 데이터를 문제에 있는 데이터를 작업 또는 프로젝트로 전송하려면 아래 순서로 이 문서의 두 작업을 완료해야 합니다.

자세한 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md) 또는 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 첫 번째: 사용자 지정 양식 복사 {#first-copy-the-custom-form}

먼저 변환할 작업 또는 문제에 대한 사용자 지정 양식 데이터를 유지해야 합니다. 사용자 지정 양식 데이터는 변환된 항목에 정확히 일치해야 하므로 새 개체에 첨부할 수 있도록 양식을 복제하는 것이 좋습니다.

>[!TIP]
>
>이 상황에서 사용자 지정 양식 데이터를 유지하는 또 다른 방법은 더 큰 개체 유형을 사용자 지정 양식에 추가하는 것입니다. 자세한 내용은 섹션을 참조하십시오 [사용자 지정 양식 편집 시작](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) 기사 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms**.
1. 작업 또는 문제 유형 사용자 지정 양식을 선택한 다음 **복사**.
1. 에서 **사용자 지정 양식** 대화 상자에서 새 양식의 이름을 지정합니다.

1. 에서 **양식 유형** 드롭다운 메뉴에서 새 사용자 지정 양식을 만들 개체 유형을 선택합니다

   **예:** 사용자 지정 양식 데이터를 프로젝트에 전송하려면 프로젝트를 선택합니다.

1. 클릭 **양식 복사**.

   이렇게 복사된 사용자 지정 양식을 작업 또는 프로젝트에 첨부할 수 있습니다.

1. 계속 [두 번째: 문제 또는 작업을 변환하고 사용자 지정 양식 데이터를 전송합니다](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## 두 번째: 문제 또는 작업을 변환하고 사용자 지정 양식 데이터를 전송합니다 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 섹션에 설명된 대로 변환할 문제 또는 작업에 대한 사용자 지정 양식을 복사합니다 [첫 번째: 사용자 지정 양식 복사](#first-copy-the-custom-form) 참조하십시오.
1. 문제 또는 작업을 **사용자 지정 Forms** 옵션이 표시됩니다. 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 문제를 프로젝트로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Adobe Workfront에서 문제를 작업으로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [작업을 프로젝트로 변환](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 에서 **(개체 유형)로 변환** 표시되는 대화 상자에서 **Forms 추가** 드롭다운 메뉴를 클릭하고 이전 섹션에서 복사한 양식을 선택합니다.

   이제 문제의 사용자 지정 필드에 캡처된 정보가 작업의 사용자 지정 양식으로 전송됩니다.

