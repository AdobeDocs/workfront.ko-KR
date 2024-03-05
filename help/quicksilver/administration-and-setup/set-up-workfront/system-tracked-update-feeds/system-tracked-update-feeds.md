---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: 시스템 추적 업데이트
description: Adobe Workfront은 객체의 상태 정보를 기록하여 특정 객체에서 수행되는 활동을 캡처합니다 [!UICONTROL 업데이트] 영역입니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: d76ab0e165d280f84718b52cc72a9b4c152a0897
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# 시스템 추적 업데이트

{{highlighted-preview}}

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] 의 객체에 상태 정보를 기록하여 특정 객체에서 수행되는 활동을 캡처합니다. [!UICONTROL 업데이트] 영역입니다.

다음 [!UICONTROL 업데이트] 영역에는 다음과 같은 유형의 업데이트가 포함됩니다.

* **사용자 업데이트:** 사용자가 수동으로 입력합니다. 댓글, 답글 및 메모라고도 합니다.

  사용자 업데이트 구성에 대한 자세한 내용은 [사용자 업데이트에 대한 환경 설정 구성](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **시스템 업데이트:** 시스템에서 자동으로 만들어집니다. 시스템 업데이트에는 항목에 발생한 변경 사항을 설명하는 간단한 메모가 포함되어 있습니다.

  시스템 업데이트 피드 및 업데이트 피드를 활성화하는 방법에 대한 자세한 내용은 [시스템 업데이트 구성](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## 시스템 추적 업데이트에 대한 고려 사항

업데이트 영역이 있는 모든 개체에 대해 시스템 추적 업데이트를 사용할 수 없습니다.

* 다음 [!UICONTROL 업데이트] 영역은 다음 개체에 사용할 수 있습니다.

   * [!UICONTROL 프로젝트]
   * [!UICONTROL 작업]
   * [!UICONTROL 문제]
   * [!UICONTROL Portfolio]
   * [!UICONTROL 프로그램]
   * [!UICONTROL 사용자]
   * [!UICONTROL 템플릿]
   * [!UICONTROL 템플릿 작업]
   * [!UICONTROL 팀]
   * [!UICONTROL 문서]
   * [!UICONTROL 타임시트]
   * [!UICONTROL 스토리]

     위치 [!DNL Workfront]스토리 는 작업입니다.
   * [!UICONTROL 반복]
   * [!UICONTROL 목표]

     에 액세스하려면 추가 라이선스가 있어야 합니다. [!UICONTROL 목표] 영역입니다. 자세한 내용은 [Workfront 목표 사용 요구 사항](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL 카드] 게시판에서

     카드 업데이트에 대한 자세한 내용은 [보드에서 연결된 카드 사용](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] 은 다음 개체에 대한 시스템 업데이트를 추적하지 않습니다.

   * [!UICONTROL 팀]
   * [!UICONTROL 템플릿]
   * [!UICONTROL 템플릿 작업]
   * 애드혹 [!UICONTROL 카드]
   * [!UICONTROL 반복]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* 다음은 새 주석 달기 경험과 기존 주석 달기 경험의 차이점입니다.

   * 새 댓글 달기 경험을 사용할 때 사용자 업데이트는 댓글 탭에 표시되고 시스템 업데이트는 시스템 활동 탭에 표시됩니다.

     새 댓글 달기 환경에 대한 자세한 내용은 [새 댓글 달기 환경](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * <span class="preview">새 댓글 달기 경험을 사용할 때 시스템 업데이트에 댓글을 추가할 수 없습니다. 그러나 기존 댓글 달기 경험의 시스템 활동 레코드에 대한 모든 답글은 새 댓글 달기 경험에서 읽기 전용으로 시스템 활동 탭에 채워집니다.</span>
   * 기존 댓글 달기 경험을 사용하는 경우 시스템 및 사용자 업데이트가 하나의 연속 피드에 표시됩니다.

   * 기존 댓글 달기 경험을 사용하는 경우 사용자는 기본적으로 시스템 업데이트를 보거나 표시하지 않도록 선택할 수 있습니다. 새 댓글 달기 환경을 사용할 때는 시스템 업데이트를 비활성화할 수 없습니다.

     시스템 업데이트 표시를 비활성화하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [시스템 업데이트 활성화 또는 비활성화](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) 이 문서에서 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfront은 다음 개체에 대해 시스템에서 추적한 업데이트를 기록하지만 표시를 비활성화하는 옵션이 없습니다.

   * [!UICONTROL Portfolio]
   * [!UICONTROL 프로그램]
   * [!UICONTROL 반복]

* [!DNL Workfront] 관리자는 시스템에서 추적해야 하는 변경 유형을 [!UICONTROL 업데이트] 영역입니다. 이 있는 모든 개체가 [!UICONTROL 업데이트] 영역에도 구성 가능 [!UICONTROL 업데이트] 피드. 다음 개체에는 [!UICONTROL 업데이트] 시스템에서 추적한 업데이트 피드를 캡처하지만 구성 가능한 업데이트 피드가 없는 영역입니다.

   * [!UICONTROL 문서]
   * [!UICONTROL 타임시트]
   * [!UICONTROL 반복]
   * [!UICONTROL 목표]


