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
source-git-commit: 7b378fdf3530d5e1c06f09d03c23c31afac6aa47
workflow-type: tm+mt
source-wordcount: '0'
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

## 첫 번째: 사용자 지정 양식에 추가 개체 추가

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **사용자 지정 Forms**.
1. 필요한 양식을 찾은 다음 **편집**.
1. 양식 맨 위에 작업이나 문제를 변환할 개체를 추가합니다.
   >[!INFO]
   >
   >**예**: 사용자 지정 양식 데이터를 프로젝트에 전송하려면 프로젝트를 선택합니다.

1. 클릭 **적용** 아래의 제품에서 사용할 수 있습니다.

1. 계속 [두 번째: 문제 또는 작업을 변환하고 사용자 지정 양식 데이터를 전송합니다](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## 두 번째: 문제 또는 작업을 변환하고 사용자 지정 양식 데이터를 전송합니다 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 섹션에 설명된 대로 변환하고 있는 문제 또는 작업의 사용자 지정 양식에 개체를 추가합니다 [첫 번째: 사용자 지정 양식에 추가 개체 추가](#first-add-additonal-objects-to-the-custom-form) 참조하십시오.
1. 문제 또는 작업을 **사용자 지정 Forms** 필요한 사용자 지정 양식을 선택하기 위해 표시되는 상자의 옵션. 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 문제를 프로젝트로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Adobe Workfront에서 문제를 작업으로 변환](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [작업을 프로젝트로 변환](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 에서 **(개체 유형)로 변환** 표시되는 대화 상자에서 **Forms 추가** 드롭다운 메뉴를 클릭하고 이전 섹션에서 복사한 양식을 선택합니다.

   이제 문제의 사용자 지정 필드에 캡처된 정보가 작업의 사용자 지정 양식으로 전송됩니다.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->