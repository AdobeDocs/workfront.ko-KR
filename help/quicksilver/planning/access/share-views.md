---
title: 보기 공유
description: 보기를 다른 사용자와 공유하여 Adobe Workfront Planning 사용 시 공동 작업을 보장할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 1ffd8a3dbb31154186dc37132c7e77c35de42ac3
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

<!--update the metadata and description when we turn this article live-->

# 보기 공유

{{planning-important-intro}}

보기를 다른 사용자와 공유하여 Adobe Workfront Planning에서 레코드 작업 시 공동 작업을 보장할 수 있습니다.

작업 영역에 권한을 부여해도 다른 사용자에게 레코드 유형 페이지의 보기에 대한 권한이 부여되지 않습니다. 다른 사용자와 공유하려면 레코드 유형 페이지에서 개별 보기에 대한 권한을 부여해야 합니다.

보기를 공유할 때 다른 사용자에게 보기의 모든 요소에 액세스할 수 있는 권한을 부여합니다. 예를 들어, 보기에 대한 관리 권한을 부여하면 그룹화, 필터, 정렬 또는 막대 모양을 수정할 수 있습니다.


다음 엔티티와 뷰를 공유할 수 있습니다.

* 내부적으로, Workfront 사용자 및 그룹 사용
* 공개적으로, Workfront 외부의 사용자 포함

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Workfront Planning의 조기 액세스 단계에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>새로운 기능: 표준</p>
   또는
   <p>현재: 플랜 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> Adobe Workfront Planning에 대한 액세스 제어가 없습니다.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>보기에 대한 권한 관리</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> <p>자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>를 참조하십시오. </p> 
</td>
  </tr>
 </tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 보기 공유 시 고려 사항

* 내부 Workfront 사용자에게 보기에 대한 보기 또는 관리 권한을 부여할 수 있습니다.

* 관리 권한이 있는 사용자는 보기 설정을 수정, 공유, 복제 또는 삭제할 수 있습니다.

* 공개 링크를 사용하여 조직 외부의 사용자와 보기를 공유할 수 있습니다.

* 보기를 공개적으로 공유할 때는 회사 외부의 모든 사용자가 제한된 시간 동안 만료 날짜로 표시된 링크에 액세스할 수 있습니다. 공유 테이블 보기를 보는 데 로그인이 필요하지 않습니다.

* 보기에 대한 액세스 권한이 있는 조직 외부의 사람은 다른 보기를 만들거나 공유 보기를 편집하거나 표에서 레코드 정보를 추가, 삭제 또는 편집할 수 없습니다.

## 내부적으로 보기에 대한 권한 공유

만든 보기 또는 관리 권한이 있는 보기를 Workfront의 사용자 또는 그룹과 공유할 수 있습니다.

>[!NOTE]
>
>시스템 관리자는 자신이 만들지 않은 보기를 보거나 공유할 수 없습니다. 공유된 보기에만 액세스하거나 공유할 수 있습니다.
>
>시스템 관리자는 보기에 대한 관리 권한만 가질 수 있습니다.

{{step1-to-planning}}

1. 보기를 공유할 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다.

   그러면 레코드 유형 페이지가 열립니다.

1. 보기 탭에서 공유할 보기를 마우스로 가리키고 보기 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **공유**&#x200B;를 클릭합니다.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   기본적으로 **내부 공유** 탭을 선택해야 합니다.

1. (선택 사항) **액세스 권한이 있는 사용자** 영역에서 다음 선택 사항 중에서 선택합니다.

   * **초대된 사람만 액세스할 수 있습니다**: 보기를 공유할 사용자 또는 그룹을 지정해야 합니다. 기본 옵션입니다.
   * **작업 영역의 모든 사용자가 볼 수 있습니다**: 작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자가 보기에 액세스할 수 있습니다.

1. **보기 액세스 권한 부여** 필드에서 사용자 또는 그룹의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 드롭다운 메뉴에서 다음 권한 수준 중 하나를 선택합니다.
   * 보기
   * 관리

     권한 수준 및 사용자가 각 수준에 대해 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront Planning의 권한 공유 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.

     시스템 관리자는 항상 공유 보기에 대한 관리 권한을 받습니다.

1. 보기에 대한 링크를 클립보드에 복사하려면 **링크 복사**&#x200B;를 클릭하십시오.
1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자는 활성 사용자여야 하며 레코드 유형 페이지에 액세스하여 선택한 보기에 표시할 수 있도록 Workfront에 로그인해야 합니다.
1. **저장**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >   나와 공유된 보기의 보기 아이콘 옆에 사용자 표시기 ![](assets/view-shared-with-others-people-icon.png)이(가) 있습니다. 사람 표시기가 없는 보기는 사용자가 만든 보기입니다.

## 공개적으로 보기에 권한 공유

만든 보기 또는 관리 권한이 있는 보기를 Workfront 라이선스가 없고 조직 외부에 있을 수 있는 사람과 공유할 수 있습니다.

Workfront Planning에서 보기를 공개적으로 공유하려면 다음을 수행합니다.

{{step1-to-planning}}

1. 보기를 공유할 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다.

   그러면 레코드 유형 페이지가 열립니다.

1. 보기 탭에서 공유할 보기를 마우스로 가리키고 보기 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **공유**&#x200B;를 클릭합니다.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. **공개 공유**&#x200B;를 클릭합니다.

   ![](assets/public-sharing-tab-for-views.png)

1. **공개 링크 만들기** 설정을 사용하도록 설정합니다.

   링크를 사용할 수 있습니다. 공개 링크입니다. 링크를 공유하면 조직 외부의 직원을 포함하여 모든 사용자가 레코드 유형 페이지에 액세스하고 페이지의 레코드와 필드를 볼 수 있습니다.

1. **링크 복사** 아이콘 ![](assets/copy-link-view.png)을(를) 클릭하여 클립보드에 링크를 복사합니다.

1. 수동으로 날짜를 입력하거나 **링크 만료 날짜** 필드의 달력을 사용하여 공개 링크에 대한 만료 날짜를 선택하십시오. 선택한 날짜 이후에는 레코드 페이지 보기에 액세스할 수 없습니다.

1. **저장**&#x200B;을 클릭합니다.

   보기 아이콘이 업데이트되어 보기가 공개적으로 공유됨을 나타냅니다.

   ![](assets/public-shared-view-icon-highlighted.png)

1. (선택 사항) 복사한 링크를 이메일, 채팅 메시지, 문서 또는 Workfront 댓글에 붙여넣어 다른 사용자와 공유할 수 있습니다.

## 보기에 대한 권한 제거

{{step1-to-planning}}

1. 공유를 중지할 보기를 가진 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다. 그러면 레코드 유형 페이지가 열립니다.
1. 공유를 제거할 보기의 탭 이름 위에 마우스를 올려 놓고 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **공유**&#x200B;를 클릭합니다.
1. 보기의 내부 공유를 제거하려면 다음 작업을 수행하십시오.

   1. **내부 공유** 탭을 선택했는지 확인하십시오.
   1. 제거할 사용자 또는 그룹을 찾은 다음 사용자 또는 그룹 이름 오른쪽에 있는 권한 드롭다운 메뉴를 확장한 다음 **제거**&#x200B;를 클릭합니다.

1. 보기의 공개 공유를 제거하려면 다음 작업을 수행하십시오.

   1. **공개 공유** 탭을 클릭합니다.
   1. **공개 링크 만들기** 옵션을 선택 취소합니다.

1. **저장**&#x200B;을 클릭합니다.

   사용자는 더 이상 보기에 액세스할 수 없습니다. 보기에 액세스하지 못하도록 제거된 사용자에게 더 이상 이 액세스 권한이 없다는 알림이 없습니다.