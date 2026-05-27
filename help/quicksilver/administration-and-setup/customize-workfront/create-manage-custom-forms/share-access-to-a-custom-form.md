---
title: 사용자 정의 양식 공유
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 정의 양식에 대한 액세스 권한을 구성하여 해당 양식을 보고, 공유하고, 편집할 수 있는 사용자를 제어할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 3e6ae76eea2e12fc7fc3a45dad753261a7bad628
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 2%

---

# 사용자 정의 양식 공유

{{preview-fast-release-general}}

사용자 정의 양식에 대한 액세스 권한을 구성하여 개인, 역할, 그룹, 팀, 회사, 비즈니스 프로필 등 해당 양식을 보고, 공유하고, 편집할 수 있는 사용자를 제어할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr>  
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 양식에 액세스 {#access-to-custom-forms}

기본적으로 새 사용자 정의 양식을 만들어 다른 사용자가 오브젝트에 첨부하면 해당 오브젝트에 할당된 모든 사용자가 양식을 보고 작성할 수 있습니다. 여기에는 기여자 또는 요청 라이선스를 가진 사용자와 외부 사용자가 포함됩니다.

그러나 사용자 정의 양식이 아직 첨부되지 않은 객체에서는 다음 중 하나가 참이 아닌 경우 사용자가 사용자 정의 Forms 드롭다운 메뉴에서 첨부할 수 없습니다(플래너 액세스 수준이 있는 경우에도).

* <span class="preview">누군가 사용자 정의 양식을 &quot;시스템의 모든 사용자가 보고 첨부할 수 있음&quot;으로 공유했습니다</span>
* 누군가 사용자 정의 데이터에 첨부 가 선택된 상태로 보기 이상의 권한을 부여한 사용자 또는 해당 팀, 작업 역할, 그룹, 회사 또는 비즈니스 프로필과 사용자 정의 양식을 공유했습니다
* 사용자는 Standard 또는 Plan 라이선스를 보유하고 있으며 액세스 수준을 통해 사용자 정의 양식에 대한 관리자 액세스 권한을 부여받습니다

<!--

## Share a custom form from the list of forms

Rather than leaving a custom form in the default sharing state (described in [Access to custom forms](#access-to-custom-forms) in this article), you can configure specific levels of access to the form for certain users, job roles, groups, teams, and companies.

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Select the custom form, then click ![Share icon](assets/share-icon.png).
1. In the box that displays, under **Give custom form access to**, start typing the name of the user, team, job role, group, company, or business profile you want to share the custom form with, then press **Enter** when the name displays.
1. To adjust access for the user, team, job role, group, company, or business profile you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>This option provides the ability to view and fill out the custom form on objects. At the object level, users must also have at least Contribute access with the <strong>Edit custom form</strong> advanced setting enabled. For example, if the form is attached to a project, users must have Contribute access to that project, or they will not be able to fill out the form.</p>
      
      <p><b>NOTE</b>: For users with Light and Contributor licenses (or Work, Review, and Request licenses), this is the highest available option.</p>
      
      <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow the following:</p> 
       <ul> 
        <li><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</li> 
        <li> <p><strong>Share</strong>: Ability to share the custom form with others in the system</p> <p>Users with a Light or Contributor license (or Work, Review, or Request license) can share a custom form only through the API or a custom forms report.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage it</td> 
      <td> <p>This option available only for users with a Standard or Plan license. </p> <p>In addition to being able to add the form to objects they have access to edit, users can also fully edit the custom form, including adding, editing, and deleting fields.</p> <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow following:</p> 
       <ul> 
        <li> <p><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</p> </li> 
        <li><strong>Delete</strong>: Delete the custom form from the system</li> 
        <li><strong>Share</strong>: Share the custom form with others in the system</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Repeat Steps 4-5 to add other names to the list and configure their options.
1. (Optional) If you want to limit access to the custom form (on objects where it's attached) to those you have specified in the previous steps, click the gear icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) in the upper right corner of the sharing box, then click **Remove system-wide access**.

   If you change your mind, you can click **Make this visible system-wide** (the default option).

   >[!NOTE]
   >
   >* When you make a custom form visible system-wide, you allow users only to see and fill it out on objects they are assigned to, not to attach it to other objects. You can grant the ability to attach the custom form to objects using the option "Attach to custom data" explained under step 5.
   >* Most organizations want to ensure that everyone in the system can fill out a custom form when it's attached to objects they work on and view its data in reports. If this is true for your organization, we recommend that you use **Make this visible system-wide**. When the option is configured this way, "Visible System-Wide" displays in the dialog box:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >If you are concerned about a custom form where users might enter sensitive data when it is attached to certain objects, limiting sharing for those *objects* might be better rather than limiting access to the form itself.

1. Click **Save**.

-->

## 사용자 정의 양식 공유

사용자 정의 양식을 기본 공유 상태([사용자 정의 양식에 대한 액세스](#access-to-custom-forms)에서 설명)로 두는 대신 특정 사용자, 작업 역할, 그룹, 팀, 회사 및 비즈니스 프로필에 대해 양식에 대한 특정 액세스 수준을 구성할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 목록에서 사용자 정의 양식을 선택한 다음 ![공유 아이콘](assets/share-icon.png)을 클릭합니다.

   또는

   사용자 정의 양식을 열거나 새 사용자 정의 양식을 만듭니다. 그런 다음 양식 디자이너의 오른쪽 상단에서 **공유**&#x200B;를 클릭합니다.

1. 공유 상자의 **사용자 정의 양식 액세스 권한 부여**&#x200B;에서 사용자 정의 양식을 공유할 사용자, 팀, 작업 역할, 그룹, 회사 또는 비즈니스 프로필의 이름을 입력한 다음 이름이 표시되면 **Enter**&#x200B;를 누릅니다.
1. 방금 추가한 사용자, 팀, 작업 역할, 그룹, 회사 또는 비즈니스 프로필에 대한 액세스를 조정하려면 이름 오른쪽에 있는 드롭다운 메뉴를 클릭한 다음 사용 가능한 다음 옵션 중 하나와 고급 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보기</td> 
      <td> <p>이 옵션은 개체에서 사용자 정의 양식을 보고 작성하는 기능을 제공합니다. 개체 수준에서 사용자는 <strong>사용자 정의 양식 편집</strong> 고급 설정을 사용하는 적어도 Contribute 액세스 권한을 가지고 있어야 합니다. 예를 들어 양식이 프로젝트에 첨부된 경우 사용자는 해당 프로젝트에 대한 기여 액세스 권한이 있어야 합니다. 그렇지 않으면 양식을 작성할 수 없습니다.</p>

   <p><b>참고</b>: Light 및 Contributor 라이선스가 있는 사용자(또는 작업, 검토 및 요청 라이선스)의 경우 이 옵션을 사용할 수 있습니다.</p> <p>다음을 허용할지 여부를 지정하려면 <strong>고급 설정</strong>을 클릭하십시오.</p> 
       <ul> 
        <li><strong>사용자 정의 데이터에 첨부</strong>: 관리 액세스 권한이 있는 프로젝트, 작업 및 문제에 사용자 정의 양식을 첨부할 수 있습니다.</li> 
        <li> <p><strong>공유</strong>: 사용자 정의 양식을 시스템의 다른 사용자와 공유하는 기능</p> <p>라이트 또는 기여자 라이선스(또는 작업, 검토 또는 요청 라이선스)가 있는 사용자는 API 또는 사용자 정의 양식 보고서를 통해서만 사용자 정의 양식을 공유할 수 있습니다.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">관리</td> 
      <td> <p>이 옵션은 Standard 또는 Plan 라이선스가 있는 사용자만 사용할 수 있습니다. </p> <p>편집할 수 있는 액세스 권한이 있는 오브젝트에 양식을 추가할 수 있을 뿐만 아니라 필드를 추가, 편집 및 삭제하는 등 사용자 정의 양식을 완전히 편집할 수도 있습니다.</p> <p>다음을 허용할지 여부를 지정하려면 <strong>고급 설정</strong>을 클릭하십시오.</p> 
       <ul> 
        <li> <p><strong>사용자 정의 데이터에 첨부</strong>: 관리 액세스 권한이 있는 프로젝트, 작업 및 문제에 사용자 정의 양식을 첨부할 수 있습니다.</p> </li> 
        <li><strong>삭제</strong>: 시스템에서 사용자 정의 양식을 삭제합니다.</li> 
        <li><strong>공유</strong>: 사용자 정의 양식을 시스템의 다른 사용자와 공유합니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 5-6단계를 반복하여 목록에 다른 이름을 추가하고 해당 옵션을 구성합니다.
1. (선택 사항) 이전 단계에서 지정한 사용자 정의 양식에 대한 액세스를 제한하려면 **액세스 권한이 있는 사용자**&#x200B;의 드롭다운 화살표를 클릭한 다음 **초대된 사용자만 액세스할 수 있음**&#x200B;을 선택합니다.

   마음이 바뀌면 **시스템의 모든 사용자가 볼 수 있음**&#x200B;을 선택할 수 있습니다.

   >[!NOTE]
   >
   >* 사용자 정의 양식을 시스템 전체에 표시할 때 사용자는 다른 오브젝트에 첨부하지 않고 할당된 오브젝트에 대해서만 보고 채울 수 있습니다. 6단계에서 설명한 &quot;사용자 정의 데이터에 첨부&quot; 옵션을 사용하여 사용자 정의 양식을 오브젝트에 첨부할 수 있는 기능을 부여할 수 있습니다.
   >* 대부분의 조직에서는 시스템에서 작업 중인 오브젝트에 사용자 정의 양식을 첨부하고 보고서에서 해당 데이터를 볼 때 모든 사용자가 사용자 정의 양식을 작성할 수 있도록 하고자 합니다. 조직에 대해 true인 경우 **시스템의 모든 사용자가 볼 수 있음**&#x200B;을 사용하는 것이 좋습니다.
   >* <span class="preview">**시스템의 모든 사용자가 보고 연결할 수 있음**&#x200B;을 선택하면 모든 사용자가 다른 개체에 양식을 첨부할 수 있습니다.</span>
   >
   >미리 보기 환경의 <span class="preview">샘플 이미지:</span>
   >![사용자 정의 양식 공유](assets/share-custom-forms-all-can-attach.png)
   >   
   >프로덕션 환경의 샘플 이미지:
   >![사용자 정의 양식 공유](assets/share-custom-form-in-designer.png)
   >   
   >사용자 정의 양식을 특정 개체에 첨부할 때 사용자가 중요한 데이터를 입력할 수 있는 경우 양식 자체에 대한 액세스를 제한하는 것보다 해당 *개체*&#x200B;에 대한 공유를 제한하는 것이 더 효과적일 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

## 사용자 정의 양식에 대한 액세스 제거

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭합니다.
1. 목록에서 사용자 정의 양식을 선택한 다음 ![공유 아이콘](assets/share-icon.png)을 클릭합니다.
1. 공유 상자에서 양식에 더 이상 액세스하지 않으려는 사용자, 팀, 역할, 그룹, 회사 또는 비즈니스 프로필 이름 오른쪽에 있는 드롭다운 메뉴를 클릭하고 **제거**&#x200B;를 선택합니다.
1. (선택 사항) 제거할 다른 이름에 대해 이전 단계를 반복합니다.
1. **저장**&#x200B;을 클릭합니다.

