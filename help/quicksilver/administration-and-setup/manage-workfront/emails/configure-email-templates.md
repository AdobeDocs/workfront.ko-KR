---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: 이메일 템플릿 구성
description: Adobe Workfront 관리자는 미리 알림을 지원하도록 이메일 템플릿을 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: 3d4ba0396c5a59b1109ec70a6e85b77d0d093bf5
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 1%

---

# 이메일 템플릿 구성

Adobe Workfront 관리자는 미리 알림을 지원하도록 이메일 템플릿을 구성할 수 있습니다.

이메일 템플릿에는 미리 알림이 시작될 때 사용자에게 전송된 메시지가 포함됩니다.\
이메일 템플릿이 없으면 미리 알림이 이메일 본문에 빈 콘텐츠로 전달됩니다.

이메일 템플릿은 문제, 작업, 프로젝트 및 타임시트에 대한 미리 알림과 연결할 수 있습니다. 이메일 템플릿을 만들 때 Workfront 관리자는 이메일 콘텐츠와 제목 줄을 제공할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>시스템 관리자</p> </td> 
  </tr> 
 </tbody> 
</table>

## 새 이메일 템플릿 만들기 {#create-a-new-email-template}

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽의 패널에서 을 클릭합니다. **이메일** > **알림**> **이메일 템플릿**.

<!--hidden for tab redesign - August 2023: 
  ![](assets/email-templates-tab-under-setup-email-notifications-area.png)
  -->

1. 클릭 **새 이메일 템플릿**.

1. 다음에서 **새 이메일 템플릿** 나타나는 상자에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td>이메일 템플릿의 제목입니다(필수).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">오브젝트 유형</td> 
      <td>템플릿을 연결할 개체 유형을 지정합니다(필수, 기본적으로 '문제'로 설정됨).</td> 
     </tr>
     <tr> 
      <td role="rowheader">설명</td> 
      <td>템플릿에 대한 설명입니다.</td> 
     </tr>

   <tr> 
      <td role="rowheader">주제 </td> 
      <td>이메일 메시지를 보낼 때 표시되는 제목입니다(필수).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">본문 </td> 
      <td> <p>이메일 메시지를 보낼 때 표시되는 콘텐츠.</p> <p>에 설명된 대로 이메일 콘텐츠에 HTML 형식을 사용할 수 있습니다 <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">이메일 템플릿에 HTML 서식 추가</a> 이 문서에서.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

## 이메일 템플릿에 HTML 서식 추가 {#add-html-formatting-to-an-email-template}

이메일 템플릿에 HTML 태그를 추가하여 사용자 지정 알림을 생성할 수 있습니다.\
에 설명된 대로 이메일 템플릿 만들기 시작 [새 이메일 템플릿 만들기](#create-a-new-email-template).

HTML 서식을 지정하면 다음 섹션에 표시된 대로 이메일 템플릿을 보강할 수 있습니다.

* [Workfront 오브젝트에 대한 링크](#link-to-workfront-objects)
* [HTML을 사용하여 사용자 정의 필드에 연결](#link-to-custom-fields-with-html)
* [HTML 이메일 예](#html-email-examples)

### Workfront 오브젝트에 대한 링크 {#link-to-workfront-objects}

다음을 사용하여 Workfront 필드에 대한 링크를 포함할 수 있습니다. `$$` 와일드카드: 이메일 생성기가 특정 객체와 연관된 데이터베이스에서 값을 찾도록 지시합니다.

예를 들어 작업을 시작하려는 작업의 피할당자에게 경고를 보내는 알림용 이메일 본문은 다음 구조를 따를 수 있습니다.

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

객체에 대한 &quot;와일드카드&quot; 값을 가져오려면 다음 중 하나를 수행합니다.

<!-- Refer to the API Explorer and select the names of your objects from the Fields tab of any object. For more information about the API Explorer, see [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

* 보고서의 텍스트 모드 보기 내에서 찾을 수 있는 &quot;valuefield&quot; 값을 사용합니다. 텍스트 모드 값에 대한 자세한 내용은 [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

  &quot;제목&quot; 값은 이메일 본문에 표시하려는 오브젝트의 이름이 될 수 있습니다.

### HTML을 사용하여 사용자 정의 필드에 연결 {#link-to-custom-fields-with-html}

다음을 사용하여 사용자 링크 및 사용자 정의 필드를 포함할 수 있습니다. **$$** 와일드카드: 이메일 생성기가 객체와 연관된 데이터베이스에서 값을 찾도록 지시합니다. 데이터베이스 속성 참조의 양쪽에 있어야 합니다.

예를 들어, 다음 텍스트를 HTML으로 추가하면 할당된 사용자의 이름이 작업과 연결된 미리 알림에 추가됩니다.

`assignedTo:firstName`

동일한 서식을 사용하여 사용자 정의 필드를 추가하려면 전자 메일 알림에 다음을 추가할 수 있습니다.

`DE:Custom Field As It Appears in Workfront`

예를 들어 게재 날짜라는 사용자 정의 필드에 대한 참조를 포함하는 이메일 템플릿이며 게재 날짜 필드가 작업에 속한다고 가정합니다.

바꾸기 `<your domain>` 대괄호 없이 회사의 Workfront 도메인을 사용하는 경우:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>필드가 프로젝트에 속한 경우 작업을 프로젝트로 바꾸십시오.
>
>`DE:Project:Delivery Date`

### HTML 이메일 예 {#html-email-examples}

* [지연 프로젝트 미리 알림(예)](#late-project-reminder-notification-example)
* [미리 알림을 시작하려고 하는 작업 또는 문제(예)](#task-or-issue-about-to-start-reminder-example)

#### 지연 프로젝트 미리 알림(예) {#late-project-reminder-notification-example}

지연된 프로젝트 미리 알림에 대한 이메일 템플릿을 편집하려면 제목 및 콘텐츠 필드에 대한 이 정보를 고려하십시오.

바꾸기 `<your domain>` 를 중괄호 없이 회사의 Workfront 도메인으로 바꿉니다.

**주제:**

관리하는 프로젝트가 늦어졌습니다.

**콘텐츠:**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

이렇게 하면 다음과 유사한 이메일이 생성됩니다.

![](assets/screen-shot-2016-09-16-at-3.52.54-pm-350x103.png)

#### 미리 알림을 시작하려는 작업 또는 문제 {#task-or-issue-about-to-start-reminder-example}

예정된 작업 또는 문제에 대한 미리 알림을 만들 수도 있습니다.

다음 코드는 작업 또는 문제의 계획된 시작 일자 전 며칠 동안 전송되는 작업 및 문제 미리 알림에 사용할 이메일 템플릿에 포함할 수 있습니다.

바꾸기 `<your domain>` 를 중괄호 없이 회사의 Workfront 도메인으로 바꿉니다.

문제 이메일에 사용하려면 `/task/view.` 작업 항목 링크에서 값 `/issue/view`.

**주제:**

`$$name$$ to start on $$plannedStartDate$$`

**콘텐츠:**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_delivered.png](assets/email-template-delivered.png)

이메일 템플릿이 생성되면에 설명된 대로 사용자는 이메일 템플릿을 미리 알림 과 연결할 수 있습니다 [미리 알림 설정](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
