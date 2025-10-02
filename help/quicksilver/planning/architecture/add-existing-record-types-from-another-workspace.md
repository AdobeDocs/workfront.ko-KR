---
title: 다른 Workspace에서 기존 레코드 유형 추가
description: 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 다른 작업 영역에서 생성된 기존 레코드 유형을 추가할 수 있습니다.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 다른 작업 영역에서 기존 레코드 유형 추가

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

작업 영역 관리자는 다른 작업 영역에 있는 레코드 유형을 Adobe Workfront Planning에서 관리하는 작업 영역에 추가할 수 있습니다.

이 문서에서는 기존 레코드 유형에서 레코드 유형을 추가하는 방법과 더 이상 필요하지 않은 경우 삭제하는 방법에 대해 설명합니다.

기존 레코드 유형으로 관리하는 작업 영역에 레코드 유형을 추가하려면 먼저 작업 영역 관리자가 레코드 유형을 중앙 집중식으로 지정해야 합니다.

고급 설정을 정의할 때 레코드 유형을 만들거나 편집할 때 중앙 집중식으로 지정할 수 있습니다.

자세한 내용은 [레코드 형식에 대한 작업 영역 간 기능 구성](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)을 참조하십시오.

중앙 집중식 레코드 형식에서 작업 영역에 레코드를 추가하기 전에 문서 [작업 영역 간 레코드 형식 개요](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)를 참조하십시오.


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
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul><li><p>모든 Workfront 패키지</p></li>
<p>And</p>
<li><p>연결 가능한 레코드 유형을 만들기 위한 모든 Planning 패키지</p></li>
<li><p>중앙 집중식 레코드 유형을 만드는 Planning Plus 패키지</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
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

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++   

## 기존 레코드 유형에서 레코드 유형 만들기

1. 문서 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)에 설명된 대로 레코드 종류 만들기를 시작한 다음 **기존 항목 추가**&#x200B;를 클릭합니다. <!--check this - the option might have been renamed in the UI-->

   ![다른 작업 영역에서 추가할 수 있는 옵션과 함께 레코드 종류를 추가하는 모달](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. **계속**&#x200B;을 클릭합니다.
1. **레코드 종류 선택** 상자에서 기존 작업 영역에서 추가할 레코드 종류의 카드를 클릭한 다음 **추가**&#x200B;를 클릭합니다.

   선택한 작업 영역에 레코드 유형이 추가됩니다.

   >[!TIP]
   >
   >다른 작업 영역에 추가하도록 구성된 레코드 유형이 없는 경우 다른 작업 영역에서 해당 레코드 유형을 추가하는 옵션이 표시되지 않습니다.

   다음과 같은 상황이 발생합니다.

   * 기존 중앙 집중식 레코드 유형에서도 다음 정보가 추가됩니다.

      * 모든 원본 필드
      * 모든 레코드 연결
   * 해당 작업 영역에 대해 적어도 보기 권한이 있는 경우에만 동일한 중앙 집중식 레코드 유형을 사용하는 다른 작업 영역에서 추가된 레코드를 볼 수 있습니다.
   * **중앙 집중식 레코드 종류** 아이콘 ![중앙 집중식 레코드 종류 아이콘](assets/global-icon.png)이(가) 새 레코드 종류의 카드에 추가되었습니다.
   * 읽기 전용 **Workspace** 필드가 새 레코드 형식 테이블 보기에 추가되었습니다. 필드에는 각 레코드가 생성된 작업 공간이 표시됩니다.

     >[!NOTE]
     >
     >새 레코드 종류의 모양, 고급 설정 또는 원본 필드는 편집할 수 없습니다. 원본 작업공간에서만 레코드 종류 및 원본 필드와 설정을 편집할 수 있습니다.

1. (선택 사항) 을 클릭한 다음, 새로 추가된 레코드 유형을 작업 공간 내의 임의의 섹션으로 끌어다 놓습니다.

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

## 보조 작업 영역에서 중앙 집중식 레코드 유형 삭제

더 이상 필요하지 않은 경우 다른 작업 영역에서 추가한 레코드 유형을 삭제할 수 있습니다. 삭제하면 보조 작업 영역에서만 삭제되고 해당 작업 영역에서 추가된 레코드도 삭제됩니다. 원래 레코드 유형은 원래 작업 영역 및 원래 작업 영역이 추가된 다른 작업 영역에 남아 있습니다.

보조 작업 영역에서 중앙 집중식 레코드 유형을 삭제하려면 다음을 수행합니다.

1. 보조 작업 공간의 중앙 집중식 레코드 유형으로 이동합니다.

1. (선택 사항) 레코드 종류의 카드에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png) 또는 해당 페이지의 레코드 종류 이름 오른쪽에 있는 **삭제**&#x200B;를 클릭합니다.
1. (조건부) 제공된 필드에 **delete**&#x200B;을(를) 입력한 다음 **영구적으로 삭제**&#x200B;을(를) 클릭합니다.

   다음과 같은 상황이 발생합니다.

   * 중앙 집중식 레코드 유형에서 생성된 레코드 유형은 선택한 작업 영역에서 제거됩니다.
   * 원래 레코드 유형 및 해당 필드는 원래 작업 영역에 유지됩니다.
   * 레코드 유형은 추가된 다른 모든 작업 영역에 남아 있습니다.
   * 현재 작업 영역에서 레코드 유형에 추가된 레코드가 삭제됩니다. 중앙 집중식 레코드 유형이 추가된 추가 작업 영역에서 추가된 다른 모든 레코드는 보존됩니다.





