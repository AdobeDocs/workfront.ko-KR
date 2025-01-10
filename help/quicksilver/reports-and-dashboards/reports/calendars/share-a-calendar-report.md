---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 캘린더 보고서 공유
description: 다른 사용자와 캘린더를 공유할 수 있으며 공개적으로 사용할 수 있도록 하여  [!DNL Adobe Workfront] 라이선스가 없는 사람이 캘린더를 볼 수 있도록 합니다.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: d90459cb4f6fb1960552f0ab174e963582312b5c
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# 캘린더 보고서 공유

다른 사용자와 캘린더를 공유할 수 있으며 공개적으로 사용할 수 있도록 하여 [!DNL Adobe Workfront] 라이선스가 없는 사람이 캘린더를 볼 수 있도록 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: 밝게</p>
       <p>또는</p>
       <p>현재: 검토</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!UICONTROL 보고서], [!UICONTROL 대시보드] 및 [!UICONTROL 달력]에 대한 [!UICONTROL 보기] 이상 액세스</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>공유 액세스 권한이 있는 캘린더 보고서에 대한 [!UICONTROL 보기] 이상 권한</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Workfront]명의 사용자와 캘린더 공유 {#share-a-calendar-with-workfront-users}

캘린더를 공유하는 것은 다른 오브젝트를 공유하는 것과 비슷합니다. [!DNL Adobe Workfront]에서 개체를 공유하는 방법에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

사용자가 공유한 캘린더가 캘린더 이름 옆에 별표(&#42;)로 표시됩니다.

[!DNL Workfront] 내의 일정을 공유하려면:

1. 공유할 캘린더로 이동합니다.
1. **[!UICONTROL 일정 작업]**&#x200B;을 클릭한 다음 **[!UICONTROL 공유]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 일정 액세스 권한 부여]** 필드에서 일정을 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.\
   권한 설정에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하세요.

1. (선택 사항) 달력에 대한 액세스 권한을 부여할 각 사용자, 팀, 역할 또는 그룹에 대해 3단계를 반복합니다.
1. 드롭다운 메뉴를 클릭하여 3단계에서 추가한 각 사용자, 팀, 역할, 그룹 또는 회사에 대한 권한을 지정한 다음 부여할 권한 수준을 선택합니다.

   * **[!UICONTROL 보기]:** 사용자는 일정을 검토하고 공유할 수 있습니다.

     ![보기 액세스 권한과 일정 공유](assets/calendar-share-view-permissions-350x249.png)

   * **[!UICONTROL 관리]:** 사용자는 캘린더에 대한 전체 액세스 권한을 가지며, 액세스 수준에서 부여된 관리 권한과 모든 보기 권한을 제외합니다.

     ![액세스 관리로 일정 공유](assets/calendar-share-manage-permissions-350x241.png)

     >[!NOTE]
     >
     >[!DNL Workfront] 관리자와 일정 작성자는 이러한 엔터티에서 권한을 제거할 수 있습니다.

1. (선택 사항) 사용자의 역할에 따라 **[!UICONTROL 고급 옵션]**&#x200B;을 클릭한 다음 **[!UICONTROL 공유]**&#x200B;를 클릭하여 사용자가 다른 사용자와 일정&#x200B;을 공유할 수 있도록 할 수 있습니다.

   권한 수준에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

1. (선택 사항) 모든 [!DNL Workfront] 사용자가 캘린더를 사용할 수 있도록 하려면 톱니바퀴 아이콘을 클릭한 다음, 드롭다운 메뉴에서 **[!UICONTROL 시스템 전체에 표시]**&#x200B;를 클릭하여 모든 [!DNL Workfront] 사용자가 개체를 사용할 수 있도록 합니다.\
   모든 사용자는 사용자가 설정한 권한에 따라 개체를 볼 수 있습니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 공개 링크와 캘린더 공유

캘린더를 공개하고 [!DNL Workfront] 라이선스가 없는 사람과 링크를 공유할 수 있습니다.

1. 공유할 캘린더로 이동합니다.
1. **[!UICONTROL 일정 작업]**&#x200B;을 클릭한 다음 **[!UICONTROL 공유]**&#x200B;를 클릭합니다.

1. 톱니바퀴 아이콘을 클릭한 다음 **[!UICONTROL 외부 사용자에게 공개하기]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 링크 복사]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 비공개 링크와 캘린더 공유

[!DNL Workfront]명의 사용자와 개인 캘린더 링크를 공유할 수 있습니다. 사용자가 링크를 사용할 때 캘린더를 보려면 로그인해야 합니다.

1. 공유할 캘린더로 이동합니다.
1. **[!UICONTROL 일정 작업]**&#x200B;을 클릭한 다음 **[!UICONTROL 공유 가능한 링크 가져오기]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 링크 복사]**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >[!DNL Workfront]명의 사용자가 캘린더에 액세스할 수 있어야 링크로 캘린더에 액세스할 수 있습니다. 액세스 권한을 부여하려면 [사용자 [!DNL Workfront] 와 일정 공유](#share-a-calendar-with-workfront-users)를 참조하세요.\
   >사용자에게 액세스 권한이 없는 경우 브라우저에 링크를 붙여넣은 후 요청할 수 있습니다.
