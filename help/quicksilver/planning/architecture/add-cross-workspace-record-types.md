---
title: 기존 레코드 유형 추가
description: 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 다른 작업 영역에서 기존 레코드 유형을 가져올 수 있습니다.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 기존 레코드 유형 추가

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

작업 영역 관리자는 기존 레코드 유형을 다른 작업 영역으로 가져오거나 추가할 수 있습니다.

작업 영역 관리자가 레코드 유형을 다른 작업 영역으로 가져오려면 먼저 레코드 유형을 중앙 집중식으로 지정해야 합니다.

기록 유형을 만들거나 편집할 때 교차 작업 공간 설정을 정의할 때 중앙 집중식으로 지정할 수 있습니다.

자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지*</p></td> 
   <td> 
<ul><li><p>모든 Workfront 패키지</p></li>
And
<li><p>Planning Plus 패키지</p></li></ul>
또는:
<ul><li><p>모든 워크플로우 패키지</p> </li>
And
<li><p>Prime 또는 Ultimate 패키지 계획</p></li></ul>
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++   

## 중앙 집중식 레코드 유형 개요

다른 작업 영역에서 기존 레코드 유형을 추가할 때 고려 사항

* 다른 작업 영역에 추가하도록 구성된 레코드 유형이 없는 경우 레코드 유형을 만들 때 다른 작업 영역에서 해당 레코드 유형을 가져오는 옵션이 표시되지 않습니다. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* 다른 작업 영역에서 레코드 유형을 추가하면 기존 레코드 유형에서 다음 정보도 추가됩니다.

   * 필드
   * 레코드 연결

* 다른 작업 영역에서 추가된 레코드는 해당 작업 영역에 대한 권한이 있는 경우에만 볼 수 있습니다.

* 필드를 포함한 레코드 유형은 원래 작업 공간에서만 편집할 수 있습니다. 추가된 작업공간에서는 편집할 수 없습니다.
* 모든 작업 영역에서 추가된 레코드는 권한이 없는 작업 영역에서 생성된 경우에도 모든 작업 영역에서 액세스하는 모든 사용자에게 표시됩니다.

## 기존 레코드 유형에서 레코드 유형 만들기

1. 문서 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)에 설명된 대로 레코드 종류 만들기를 시작한 다음 **기존 항목 추가**&#x200B;를 클릭합니다. <!--check this - the option might have been renamed in the UI-->

   ![다른 작업 영역에서 가져올 수 있는 옵션과 함께 레코드 종류를 추가하는 모달](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. **계속**&#x200B;을 클릭합니다.
1. **레코드 종류 선택** 상자에서 기존 작업 영역에서 추가할 레코드 종류의 카드를 클릭한 다음 **추가**&#x200B;를 클릭합니다.

   선택한 작업 영역에 레코드 유형이 추가되고 다음과 같은 상황이 발생합니다.

   * **작업 영역 간 레코드 종류** 아이콘 ![작업 영역 간 연결 아이콘](assets/global-icon.png)이 가져온 레코드 종류의 카드에 추가됩니다.
   * 가져온 레코드 형식에 읽기 전용 **Workspace** 필드가 추가되었습니다. 필드에는 각 레코드가 생성된 작업 공간이 표시됩니다.

     >[!NOTE]
     >
     >* 가져온 레코드 종류 또는 해당 필드는 편집할 수 없습니다. 원래 작업 영역에서 레코드 유형 및 해당 필드를 편집할 수 있습니다.

1. (선택 사항) 가져온 레코드 종류의 카드에서 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭하거나 페이지의 레코드 종류 이름 오른쪽에 있는 **삭제**&#x200B;를 클릭합니다.
1. (조건부) 제공된 필드에 **delete**&#x200B;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다.

   이렇게 하면 선택한 작업 영역에서 가져온 레코드 유형이 제거됩니다. 원래 레코드 유형 및 해당 필드는 원래 작업 영역에 유지됩니다.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



