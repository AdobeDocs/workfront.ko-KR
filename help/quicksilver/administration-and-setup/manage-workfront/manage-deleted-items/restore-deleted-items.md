---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 삭제된 항목 복원
description: Workfront 관리자인 경우 지난 30일 동안 프로젝트, 작업, 문제, 문서 및 템플릿이 삭제된 경우 Adobe Workfront에서 복원할 수 있습니다. 30일 후에는 이러한 항목이 영구적으로 삭제되며 복원할 수 없습니다.
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 2%

---

# 삭제된 항목 복원

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront 관리자인 경우 지난 30일 동안 프로젝트, 작업, 문제, 문서 및 템플릿이 삭제된 경우 Adobe Workfront에서 복원할 수 있습니다. 30일 후에는 이러한 항목이 영구적으로 삭제되며 복원할 수 없습니다.

객체를 복원하면 모든 하위 객체와 필드도 복원됩니다. 예를 들어 프로젝트를 복원하면 프로젝트의 모든 작업, 문제, 문서, 시간, 메모, 할당 및 사용자 지정 데이터도 복원됩니다.

그룹 관리자는 자신이 관리하는 그룹에 대해 이러한 객체를 복원할 수도 있습니다.

>[!IMPORTANT]
>
>* 보고서, 대시보드, 사용자, 그룹, 팀 또는 반복을 삭제하면 복원할 수 없습니다.
>* 그룹에서는 그룹 관리자가 아닌 다른 사람이 오브젝트의 문서 영역에 직접 문서를 업로드할 때 Workfront 관리자만 문서를 복원할 수 있습니다.
>
>* 작업 또는 문제를 이동하고 작업 또는 문제에 첨부된 문서도 이동하지 않도록 선택하면 해당 문서가 삭제되고 30일 동안 휴지통에 보관됩니다. 관리자는 이를 복원할 수 있으며 이동된 작업 또는 문제에 다시 연결됩니다. 작업 또는 문제가 이동된 후 삭제된 경우 해당 문서를 복원하는 관리자의 사용자 페이지에 있는 문서 영역에 해당 문서가 복원됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트, 작업 또는 문제를 복원할 때 복구되는 정보

프로젝트, 작업 또는 문제를 복원하면 다음과 같은 관련 정보가 함께 복구됩니다.

* 업데이트 영역의 댓글 및 답글
* 승인
* 할당
* 사용자 정의 양식
* 대기열 설정
* 스코어카드, 목표 및 위험을 포함한 비즈니스 사례
* 프로젝트 팀
* 일자
* 문제
* 작업
* 하위 작업
* 상태
* 재무 정보:

   * 과금 기록
   * 청구 요금
   * 경비

* 타임라인 정보:

   * 전임 작업
   * 작업 제한 사항
   * 기간 유형

* 기준선

  작업 기준선은 상위 프로젝트 또는 작업을 복원할 때는 복구되지만 개별적으로 삭제된 작업을 복원할 때는 복구되지 않습니다.

* 시간(및 시간 ID)

  삭제된 항목에 시간을 복원할지 여부는 타임시트 및 시간에 대한 환경 설정을 구성할 때 선택한 설정에 따라 다릅니다. 자세한 내용은 [개체가 삭제되고 복원될 때 시간에 대한 영향 구성](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md)을 참조하십시오.

* 항목의 URL

  복원되면 항목의 URL은 그대로 유지됩니다. 직원들이 항목에 대한 브라우저 책갈피를 만든 경우 유효한 책갈피로 유지됩니다.

* 액세스 및 권한

  항목이 삭제되기 전에 해당 항목에 액세스한 사용자는 항목이 복원된 후 다시 액세스할 수 있습니다.

* 문서(증명 문서 포함)

  문서 및 문서 버전을 복원할 때에는 다음 사항을 고려하십시오.

   * 개별적으로 삭제된 문서는 개별적으로 복원할 수 있습니다.

     상위 프로젝트, 작업 또는 문제와 함께 삭제된 문서는 상위 항목을 복원할 때 복구되지만 개별적으로 복원할 수는 없습니다.

   * 문서가 복원되면 문서 또는 문서 증명의 모든 버전이 복원됩니다.\
     개별적으로 삭제된 문서 또는 문서 증명의 개별 버전은 복구할 수 없습니다.

## 프로젝트, 작업 또는 문제를 복원할 때 복구되지 않는 정보

프로젝트, 작업 또는 문제를 복원할 때 다음과 같은 관련 정보도 함께 복구되지 않습니다.

* 좋아요 수
* 보증서
* 요청 대기열의 수신 이메일 주소
* 즐겨찾기

  삭제하기 전에 즐겨찾기 메뉴에 추가한 프로젝트, 작업 또는 문제는 복원한 후에도 즐겨찾기 메뉴에 다시 나타나지 않습니다.

* 오브젝트 해결 중

  해결 중인 개체는 **원래 문제를 유지하고 해결 방법을 이** &lt;**(프로젝트** 또는 **작업)**> 옵션과 함께 구성된 전환된 문제입니다. 상위 프로젝트 또는 작업을 삭제하면 더 이상 해당 문제를 프로젝트 또는 작업에 연결하는 링크가 없으므로 이 문제는 해결 중인 개체로 식별되지 않습니다. 상위 항목을 복원하면 링크가 복원되지 않습니다.

  Workfront 관리자 또는 그룹 관리자가 전환할 때 해결 오브젝트와 일치하도록 문제를 구성하는 방법에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 및 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)을 참조하십시오.

  문제 변환에 대한 자세한 내용은 [Adobe Workfront의 문제 변환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.

## 항목 복원

{{step-1-to-setup}}

1. **휴지통** > **최근에 삭제됨**&#x200B;을 클릭합니다.
1. 복원할 항목 유형에 따라 **프로젝트**, **작업**, **문제**, **템플릿** 또는 **문서** 탭을 클릭합니다.

   항목은 기본적으로 **삭제 날짜** 열을 기준으로 정렬됩니다.

1. 복원할 항목을 최대 10개까지 선택합니다.

   하위 작업을 삭제하면 목록에 표시됩니다.

   상위 작업을 삭제하면 상위 작업만 목록에 표시됩니다. 그러나 상위 작업을 복원하면 모든 하위 작업이 복원됩니다.

1. 선택한 항목을 원래 위치로 복원하려면 **복원**&#x200B;을 클릭하세요.
1. (선택 사항) 복원된 항목을 빠르게 보려면 [복원된 항목 보기](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md)의 단계를 따릅니다.

   항목을 복원한 후 수행되는 작업에 대한 자세한 내용은 이 문서의 [항목을 복원한 후 수행되는 작업](#what-happens-after-you-restore-items) 섹션을 참조하십시오.

## 항목을 복원하면 어떻게 됩니까? {#what-happens-after-you-restore-items}

* 작업 및 하위 작업을 복원하면 삭제되기 전의 순서로 표시됩니다.

  그러나 작업을 삭제하는 동안 다른 작업의 순서가 변경되면 작업이 작업 또는 하위 작업 목록의 맨 아래에 복원될 수 있습니다.

* 항목을 복원한 후:

   * 성공 여부를 알려주는 메시지가 표시됩니다.

     이메일 알림도 받습니다. 여러 항목을 복원한 경우 이메일에 해당 항목이 나열됩니다.

   * 프로젝트, 작업 또는 문제의 업데이트 영역과 상위 개체의 업데이트 영역에 댓글이 표시됩니다.

     문서 또는 템플릿을 복원할 때에는 이러한 문제가 발생하지 않습니다.

## 복원된 증명

누군가 증명이 포함된 문서를 복원할 때, 증명에 대한 증명 활동 페이지에 증명을 복원한 실제 사용자 대신 조직의 인스턴스에 대해 나열된 첫 번째 활성 Workfront 관리자 이름(프로필 ID 순서)이 표시될 수 있습니다.
