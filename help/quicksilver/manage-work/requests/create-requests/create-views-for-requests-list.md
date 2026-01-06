---
product-area: requests
navigation-topic: create-requests
title: 요청 영역에서 보기 만들기 및 관리
description: 새 요청 경험을 사용하는 경우 요청 영역에 대한 보기를 만들고 저장할 수 있습니다.
author: Becky
feature: Work Management
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 2%

---

# 요청 영역에서 보기 만들기 및 관리

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

새 요청 경험을 사용하는 경우 요청 영역에 대한 보기를 만들고 저장할 수 있습니다. 이러한 보기에는 필터 및 열 배열이 포함됩니다.

Workfront의 요청 영역과 홈의 내 요청 위젯에서 보기를 만들고 관리할 수 있습니다. 보기 설정은 요청 영역과 위젯 간에 유지됩니다.

>[!IMPORTANT]
>
>이 기능은 새 요청 환경에서만 사용할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p>  <p>레이아웃 템플릿에 보기를 추가하려면 Workfront 관리자여야 합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 제품</td> 
   <td> <ul><li>Adobe Workfront</li><li>Planning 요청 또는 요청 양식을 보려면 Adobe Workfront Planning이 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 영역에 보기 만들기

Workfront의 요청 영역이나 홈의 내 요청 위젯에서 보기를 만들 수 있습니다.

1. 요청 목록에 액세스하려면:

   {{step1-to-requests}}

1. 홈에서 내 요청 위젯에 액세스하려면 다음을 수행하십시오.

   {{step1-to-home}}

   1. 내 요청 위젯을 찾습니다.

      내 요청 위젯에 대한 자세한 내용은 [내 요청 위젯 사용](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)을 참조하십시오.

1. 요청 목록 또는 내 요청 위젯에서 **보기** 드롭다운 ![보기 드롭다운](assets/view-icon-requests.png)을 클릭하고 **새 보기**&#x200B;를 선택합니다.

   ![새 보기](assets/create-new-view.png)

1. 새 보기의 이름을 입력하고 **만들기**&#x200B;를 클릭합니다.
1. [요청 영역의 보기 편집](#edit-a-view-in-the-requests-area)을 계속합니다.

## 요청 영역에서 보기 편집

방금 만든 보기를 포함하여 기존 보기를 편집할 수 있습니다.

1. 요청 목록에 액세스하려면:

   {{step1-to-requests}}

1. 홈에서 내 요청 위젯에 액세스하려면 다음을 수행하십시오.

   {{step1-to-home}}

   1. 내 요청 위젯을 찾습니다.

      내 요청 위젯에 대한 자세한 내용은 [내 요청 위젯 사용](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)을 참조하십시오.

1. 요청 목록 또는 내 요청 위젯에서 편집할 보기를 찾습니다.

1. (선택 사항) 보기의 이름을 바꾸려면 **보기** 드롭다운 ![보기 드롭다운](assets/view-icon-requests.png)을 클릭하고 보기 옆에 있는 세 점 메뉴를 클릭하고 **이름 바꾸기**&#x200B;를 선택한 다음 보기의 새 이름을 입력합니다.
1. **보기** 드롭다운 ![보기 드롭다운](assets/view-icon-requests.png)을(를) 클릭하고 편집할 보기를 선택합니다.
1. <span class="preview">사용자 지정 필드를 열로 추가하려면 화면 오른쪽 근처에 있는 **열 추가** 아이콘 ![열 추가](assets/add-column.png)를 클릭하고 보기에 열로 추가하려는 사용자 지정 양식 필드 옆에 있는 더하기 아이콘을 클릭합니다.</span>

   <span class="preview">목록의 개체에 첨부된 양식의 사용자 지정 필드를 열로 추가할 수 있습니다.</span>

   >[!TIP]
   >
   >현재 프로덕션 환경에 열을 추가할 수 없습니다.
1. (선택 사항) **열**&#x200B;을 클릭하고 요청 목록에서 열을 숨기거나 표시하거나 다시 정렬합니다.

   ![열 상자](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >현재 프로덕션 환경에 열을 더 이상 추가할 수 없습니다.

1. (선택 사항) **필터**&#x200B;를 클릭하고 Planning 탭에서 보려는 요청에 대한 조건을 추가하기 시작합니다.

   ![계획 요청 탭에서 필터 편집](assets/filters-editing-box-in-requests-planning-tab.png)

   다음 필드를 기준으로 필터링할 수 있습니다.

   * **Workspace**: 요청 양식과 연결된 작업 영역입니다.
   * **레코드 종류**: 요청 양식과 연결된 레코드 종류.
   * **시작 날짜**: 요청이 제출된 날짜입니다.
   * **요청 양식**: 요청을 제출하는 데 사용되는 요청 양식의 이름입니다.
   * **상태**: 요청의 상태입니다.
   * **입력한 사람**: 요청을 추가한 사용자의 이름입니다. Workfront 외부의 사용자가 요청을 추가한 경우 **입력한 사람** 필드에 `N/A`이(가) 표시됩니다.

   <span class="preview">미리 보기 환경에서 보기에 추가된 모든 사용자 지정 필드를 기준으로 필터링할 수도 있습니다.</span>

   **And** 또는 **Or** 중 하나로 여러 필터를 연결할 수 있습니다.
필터 조건을 추가하면 요청 목록이 자동으로 필터링됩니다.



>[!IMPORTANT]
>
> * 보기에 대한 변경 사항은 자동으로 저장됩니다.
> * 보기에 대한 변경 사항은 보기를 사용하는 모든 사람에게 표시됩니다.

## 레이아웃 템플릿에 보기를 추가합니다.

Workfront 관리자는 레이아웃 템플릿에 새 보기를 추가할 수 있습니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

## 보기 공유

만든 보기를 다른 사용자, 팀 또는 그룹과 공유할 수 있습니다.

1. 요청 목록에 액세스하려면:

   {{step1-to-requests}}

1. 홈에서 내 요청 위젯에 액세스하려면 다음을 수행하십시오.

   {{step1-to-home}}

   1. 내 요청 위젯을 찾습니다.

      내 요청 위젯에 대한 자세한 내용은 [내 요청 위젯 사용](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)을 참조하십시오.

1. 요청 목록 또는 내 요청 위젯에서 공유할 보기를 찾습니다.
1. 공유할 보기 위로 마우스를 가져간 다음 세 점 메뉴가 나타나면 클릭합니다.
1. **공유**&#x200B;를 선택합니다.
1. 열리는 대화 상자에서 보기를 공유할 사용자, 팀 또는 그룹의 이름을 입력한 다음 표시될 때 목록에서 선택합니다.
1. **저장**&#x200B;을 클릭합니다.

