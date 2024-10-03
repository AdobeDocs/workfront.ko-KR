---
product-area: projects
navigation-topic: update-work-in-a-project
title: 문제 상태 업데이트
description: 문제 상태를 업데이트하여 문제의 위치와 진행 방법을 다른 사용자에게 알릴 수 있습니다.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 3%

---

# 문제 상태 업데이트

<!--Audited: 01/2024-->

문제 상태를 업데이트하여 문제의 위치와 진행 방법을 다른 사용자에게 알릴 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 기여자 이상</p>
   또는
   <p>현재: 요청 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 문제 상태

Workfront의 문제에 대한 기본 상태는 다음과 같습니다.

* 신규
* 진행 중
* 대기 중인 피드백
* 보류 중
* 해결되지 않음
* 다시 열림
* 마감됨
* 해결됨

Adobe Workfront 관리자는 조직의 문제에 대한 사용자 정의 상태를 추가할 수 있습니다. 또한 문제 유형에 따라 상태를 사용할 수 있도록 설정할 수도 있습니다.

사용자 지정 상태 및 문제 유형에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [문제 만들기](../../../manage-work/issues/manage-issues/create-issues.md)

문제 상태를 수동으로 업데이트하거나 특정 작업이 발생할 때 Workfront에서 자동으로 업데이트하도록 할 수 있습니다.

## 문제 상태 수동 업데이트

Workfront의 다음 영역에서 문제 상태를 업데이트할 수 있습니다.

* 작업 페이지의 문제 헤더입니다.
* 문제를 편집할 때 문제 편집 상자
* 문제 페이지의 세부 정보 섹션.
* 문제 목록 또는 보고서에서 상태 필드가 보기에 표시될 때.
* 문제의 요약 패널에서 확인할 수 있습니다.

문제 헤더에서 문제 상태를 수동으로 업데이트하려면:

1. 상태를 업데이트할 문제로 이동합니다.
1. 문제 헤더의 **상태** 필드를 클릭하고 새 상태를 선택하십시오.
1. 문제 완료의 시각적 표시를 제공하려면 문제 헤더의 **완료율** 아래에 있는 버블을 드래그하거나 두 번 클릭합니다

   또는

   문제 헤더의 버블 내부를 클릭하여 백분율을 입력합니다.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (선택 사항) 업데이트에 대한 추가 정보를 제공하려면 다음 중 하나를 수행합니다.

   * 업데이트에 대한 메모를 추가하려면 **업데이트** 섹션으로 이동하여 **새 댓글**&#x200B;을 클릭한 다음 메모를 입력하세요.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 특정 사용자에게 업데이트에 대한 알림을 보내려면 댓글을 입력할 때 표시되는 **사람 또는 팀 태그 지정** 필드에 이름을 입력하세요. 자세한 내용은 [업데이트에 다른 사용자 태그 지정](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)을 참조하세요.
   * 문제의 커밋 일자를 업데이트하려면 **문제 세부 정보**&#x200B;를 클릭한 다음 **커밋 일자** 필드를 편집합니다. 자세한 내용은 [문제 편집](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md)을 참조하세요.


   >[!IMPORTANT]
   >
   >  문제 할당자만 커밋 일자를 업데이트할 수 있습니다.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## 문제 상태 자동 업데이트

Workfront은 아래 표에 나열된 작업이 발생하면 문제의 기존 상태를 다른 상태로 자동으로 업데이트합니다.

>[!NOTE]
>
>다음 표의 상태는 기본 시스템 상태입니다. Workfront 관리자 또는 그룹 관리자는 Workfront 인스턴스의 상태를 변경할 수 있습니다. Workfront에서 상태를 만들고 관리하는 방법에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>액션</b></td> 
   <td><b>원래 상태</b></td> 
   <td><b>새 상태</b></td> 
  </tr> 
  <tr> 
   <td>문제 완료율을 100%로 업데이트</td> 
   <td>신규 또는 진행 중</td> 
   <td>마감됨</td> 
  </tr> 
  <tr> 
   <td>문제 완료율을 100%에서 더 낮은 숫자로 업데이트</td> 
   <td>마감됨 </td> 
   <td>진행 중</td> 
  </tr> 
  <tr> 
   <td>문제에 연결된 해결 중 오브젝트의 상태 업데이트</td> 
   <td>다양한 상태</td> 
   <td> <p>다양한 상태</p> <p>해결 중인 개체와 문제 상태에 영향을 주는 방법에 대한 자세한 내용은 해결 및 해결 가능한 개체 개요 </a> 문서의 "해결 가능한 개체의 상태와 해결 중인 개체의 상태 동기화" 섹션을 참조하십시오.<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>문제 시작 단추를 클릭하여 할당된 문제에 대한 작업을 수락합니다</span> </td> 
   <td><span>새로 만들기</span> </td> 
   <td> <p>홈 팀 설정의 문제 시작 단추와 연결된 모든 상태입니다. </p> <p>[처리 중] 단추를 [시작 문제] 단추로 바꾸는 방법에 대한 자세한 내용은 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">[처리 중 작업] 단추를 [시작] 단추로 바꾸기</a></span><span>.</span>를 참조하십시오. </p> <p>팁: [문제 시작]을 클릭한 후 <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">실행 취소 단추</span>를 클릭하면 상태가 [새로 만들기]로 되돌아갑니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
