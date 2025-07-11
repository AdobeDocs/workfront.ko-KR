---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: 시스템 추적 업데이트 개요
description: Adobe Workfront은 개체의 [!UICONTROL 업데이트] 영역에 상태 정보를 기록하여 특정 개체에서 수행되는 활동을 캡처합니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 시스템 추적 업데이트 개요

<!-- Audited: 06/2025-->

[!DNL Adobe Workfront]은(는) 개체의 [!UICONTROL 업데이트] 섹션에 상태 정보를 기록하여 특정 개체에서 수행되는 활동을 캡처합니다.

업데이트 섹션에 대한 자세한 내용은 [업데이트 섹션 개요](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)를 참조하십시오.

[!UICONTROL 업데이트] 영역에는 다음 업데이트 유형이 포함됩니다.

* **사용자 업데이트:** 사용자가 수동으로 입력했습니다. 댓글, 답글 및 메모라고도 합니다. 사용자 업데이트는 오브젝트의 업데이트 섹션의 설명 및 모든 탭에 표시됩니다.

  사용자 업데이트 구성에 대한 자세한 내용은 [사용자 업데이트에 대한 환경 설정 구성](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md)을 참조하십시오.

  ![업데이트](assets/updates-qs-350x125.png)

* **시스템 업데이트:** 시스템에서 자동으로 이루어집니다. 시스템 업데이트에는 항목에 발생한 변경 사항을 설명하는 간단한 메모가 포함되어 있습니다. 시스템 업데이트가 객체의 업데이트 섹션에 있는 시스템 활동 및 모든 탭에 표시됩니다.

  시스템 업데이트 피드와 사용 방법에 대한 자세한 내용은 [시스템 업데이트 구성](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)을 참조하십시오.

  ![시스템 업데이트 예](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## 시스템 추적 업데이트에 대한 고려 사항

업데이트 영역이 있는 모든 개체에 대해 시스템 추적 업데이트를 사용할 수 없습니다.

* [!UICONTROL 업데이트] 영역은 다음 개체에 사용할 수 있습니다.

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

     [!DNL Workfront]에서 스토리는 작업입니다.
   * [!UICONTROL 반복]
   * [!UICONTROL 목표]

     모든 Workfront 패키지에 Workfront 목표가 포함된 것은 아닙니다. 자세한 내용은 [Workfront 목표를 사용하기 위한 요구 사항](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md)을 참조하십시오.
   * 게시판의 [!UICONTROL 카드]

     카드 업데이트에 대한 자세한 내용은 [보드에 연결된 카드 사용](../../../agile/get-started-with-boards/connected-cards.md)을 참조하세요.

* [!DNL Workfront]은(는) 다음 개체에 대한 시스템 업데이트를 추적하지 않습니다.

   * [!UICONTROL 팀]
   * [!UICONTROL 템플릿]
   * [!UICONTROL 템플릿 작업]
   * 임시 [!UICONTROL 카드]
   * [!UICONTROL 반복]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* 사용자 업데이트는 설명 탭에 표시되고 시스템 업데이트는 시스템 활동 및 모두 탭에 표시됩니다.

  시스템 작업 또는 모든 탭이 없는 개체 목록은 [업데이트 섹션 개요](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)를 참조하십시오.

* 시스템 업데이트에 회신을 추가할 수 없습니다. 그러나 2024년 4월 11일 이전에 기존 댓글 달기 환경에서 시스템 활동 레코드에 대한 모든 답글은 시스템 활동 탭에서 읽기 전용으로 채워집니다.

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* [!DNL Workfront] 관리자는 [!UICONTROL 업데이트] 영역에서 시스템이 추적할 변경 유형의 내용을 정의할 수 있습니다. [!UICONTROL 업데이트] 영역이 있는 모든 개체에 구성 가능한 [!UICONTROL 업데이트] 피드가 있는 것은 아닙니다. 다음 개체에는 시스템 추적 업데이트 피드를 캡처하는 [!UICONTROL 업데이트] 영역이 있지만 업데이트 피드를 구성할 수 없습니다.

   * [!UICONTROL 문서]
   * [!UICONTROL 타임시트]
   * [!UICONTROL 반복]
   * [!UICONTROL 목표]


