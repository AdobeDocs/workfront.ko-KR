---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: 프로젝트 소유자 및 스폰서 개요
description: 프로젝트에 대한 프로젝트 소유자 및 프로젝트 스폰서를 지정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 111c776af19fbc2982c14cc9d3b3778d37bc0be3
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# 프로젝트 소유자 및 스폰서 개요

<!-- Audited: 1/2024 -->

프로젝트에 대한 프로젝트 소유자 및 프로젝트 스폰서를 지정할 수 있습니다.

프로젝트 소유자는 정시 및 예산으로 프로젝트를 완료할 책임이 있는 개인입니다.

프로젝트 스폰서는 프로젝트에 투자된 자원이 있는 프로젝트의 중요한 이해 관계자입니다. 일반적으로 프로젝트 완료는 프로젝트 스폰서에게 도움이 됩니다.

프로젝트의 프로젝트 소유자 또는 스폰서를 업데이트하는 방법에 대한 자세한 내용은 [프로젝트 소유자 및 스폰서 업데이트](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md)를 참조하십시오.

## 프로젝트 소유자

프로젝트 또는 템플릿에 프로젝트 소유자를 지정하여 프로젝트 관리자를 지정할 수 있습니다.

한 프로젝트에 대해 하나의 프로젝트 소유자만 정의할 수 있습니다.

프로젝트 소유자 필드를 사용하여 다음 작업을 수행할 수 있습니다.

* 한 명의 사용자만 프로젝트 소유자로 지정할 수 있습니다.
* 프로젝트 소유자를 프로젝트의 시간 승인자로 지정할 수 있습니다.
* 프로젝트, 태스크 또는 문제 승인 프로세스를 정의할 때 프로젝트 소유자를 일반 승인자로 지정할 수 있습니다. 승인에 대한 자세한 내용은 [승인 프로세스 편집](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)을 참조하십시오.

  >[!IMPORTANT]
  >
  >프로젝트 소유자에게 승인을 할당하고 아무도 프로젝트 소유자로 지정되지 않으면, 승인 권한은 설정 영역의 고객 정보 섹션에 표시된 대로 기본 Workfront 관리자에게 재할당됩니다. 자세한 내용은 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.
  >


* 프로젝트 소유자에게만 전달되는 특정 알림을 활성화할 수 있습니다.

  전자 메일 알림에 대한 자세한 내용은 문서 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)의 섹션 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify)을 참조하십시오.

* 보고서나 목록에 프로젝트 소유자 필드를 표시할 수 있습니다.

  또한 프로젝트 소유자 필드를 보기, 그룹화 또는 프롬프트에 표시할 수 있습니다.

  예를 들어, 다음 텍스트 모드 표현식을 필터에 복사하여 로그인한 사용자가 소유한 프로젝트를 표시할 수 있습니다. 

  ```
  ownerID=$$USER.ID
  ```

보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 프로젝트 스폰서

시스템의 모든 사용자를 프로젝트 스폰서로 지정할 수 있습니다. 프로젝트 스폰서는 일반적으로 프로젝트의 진행 상황을 알아야 하는 관리자, 경영진 또는 이해 관계자입니다.

프로젝트 스폰서를 할당할 때 다음 사항을 고려하십시오.

* 프로젝트 스폰서는 프로젝트에 대한 추가 액세스 권한을 획득하지 않지만 프로젝트의 이메일 알림에 추가됩니다. 알림에 대한 자세한 내용은 문서 [시스템의 모든 사용자를 위한 이벤트 알림 구성](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)을 참조하십시오.

* 프로젝트 스폰서를 하나만 지정할 수 있습니다.
* 프로젝트, 태스크 또는 문제 승인 프로세스를 정의할 때 프로젝트 스폰서를 일반 승인자로 지정할 수 있습니다. 승인에 대한 자세한 내용은 [승인 프로세스 편집](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)을 참조하십시오.

  >[!IMPORTANT]
  >
  >프로젝트 스폰서에게 승인을 할당하고 아무도 프로젝트의 스폰서로 지정되지 않으면 승인은 프로젝트 소유자에게 재지정됩니다. 아무도 프로젝트의 소유자로 지정되지 않은 경우 승인이 Workfront 관리자에게 할당됩니다.

* 보고서 또는 목록에 프로젝트 스폰서 필드를 표시할 수 있습니다.

  또한 프로젝트 스폰서 필드를 보기, 그룹화 또는 프롬프트에 표시할 수 있습니다.

  예를 들어, 다음 텍스트 모드 표현식을 필터에 복사하여 로그인한 사용자가 후원하는 프로젝트를 표시할 수 있습니다.

  ```
  sponsorID=$$USER.ID
  ```

   

  보고서 만들기에 대한 자세한 내용은 문서 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
