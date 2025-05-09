---
title: 개체를 변환할 때 사용자 정의 양식 데이터 전송
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 작업 항목에 정의된 작업이 너무 커지면 더 큰 작업 항목으로 변환할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 개체를 변환할 때 사용자 정의 양식 데이터 전송

조직의 비즈니스 요구 사항에 따라 작업 또는 문제에 정의된 작업이 너무 커져 작업 또는 문제 내에서 관리할 수 없습니다. 이 경우 더 큰 작업 항목으로 변환할 수 있습니다.

* 문제를 작업 또는 프로젝트로 전환할 수 있습니다.
* 작업을 프로젝트로 전환할 수 있습니다.

문제에서 작업 또는 프로젝트로 사용자 정의 양식 데이터를 전송하려면 이 문서의 두 작업을 아래 순서로 완료해야 합니다.

자세한 내용은 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md) 또는 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 첫 번째: 사용자 정의 양식에 추가 오브젝트 추가

{{step-1-to-setup}}

1. **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 필요한 양식을 찾은 다음 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
1. 양식 맨 위에서 작업 또는 문제를 전환하려는 개체를 추가합니다.

   >[!INFO]
   >
   >**예**: 사용자 지정 양식 데이터를 프로젝트로 전송하려면 [프로젝트]를 선택하십시오.

1. 양식 맨 아래에 있는 **적용**&#x200B;을 클릭합니다.

1. [초로 계속 진행: 문제 또는 작업을 전환하고 사용자 지정 양식 데이터를 전송](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data)합니다.

## 두 번째: 문제 또는 작업을 전환하고 사용자 정의 양식 데이터를 전송합니다 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 변환 중인 문제 또는 작업에 대한 사용자 정의 양식에 개체를 추가합니다. 자세한 내용은 [먼저 이 문서의 사용자 정의 양식에 개체를 추가](#first-add-additonal-objects-to-the-custom-form)합니다.
1. 표시되는 상자에서 **사용자 지정 Forms** 옵션을 사용하여 문제 또는 작업을 전환하여 필요한 사용자 지정 양식을 선택하십시오. 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront에서 문제를 프로젝트로 전환](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Adobe Workfront에서 문제를 작업으로 전환](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [작업을 프로젝트로 전환](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 표시되는 **변환 대상(개체 유형)** 대화 상자에서 **Forms 추가** 드롭다운 메뉴를 클릭하고 이전 섹션에서 복사한 양식을 선택합니다.

   문제의 사용자 정의 필드에 캡처된 정보가 이제 작업의 사용자 정의 양식으로 전송됩니다.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->
