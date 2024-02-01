---
title: 레코드 유형 편집
description: 레코드 유형을 저장한 후 편집할 수 있습니다. 레코드 유형은 Adobe 마에스트로의 객체 유형입니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the objec types of Adobe Maestro.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# 레코드 유형 편집

{{maestro-important-intro}}

레코드 유형은 Adobe 마에스트로의 객체 유형입니다. 사용자 또는 다른 사용자가 만든 레코드 유형의 모양을 편집할 수 있습니다. Maestro 레코드 유형 생성에 대한 자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <p> Adobe Workfront</p> <p>Maestro 레코드 유형을 Experience Manager Assets과 연결하려면 Adobe Experience Manager Assets 라이선스가 있어야 하며, 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Maestro에 대한 액세스 수준 제어 없음</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 레코드 유형 편집

{{step1-to-maestro}}

기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드 유형을 만들 작업 영역을 선택합니다.
1. 기록 유형의 카드 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png) 기록 유형 카드의 오른쪽 상단 모서리에서 을(를) 클릭합니다. **모양 업데이트**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. 레코드 유형 갱신 상자에서 다음 정보를 갱신합니다.

   * **레코드 이름**: 필요한 경우 레코드 유형 이름을 편집합니다. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **모양**: 레코드 종류와 관련된 아이콘의 색 및 모양을 편집합니다. 다음을 수행합니다.
      * 레코드 유형을 식별할 색상을 선택합니다. 레코드 유형 아이콘의 색상입니다. 기본적으로 회색이 선택되어 있습니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

     ![](assets/update-record-type-box.png)

1. 레코드 유형 업데이트 상자 외부를 클릭하여 변경 내용을 저장합니다.
1. (선택 사항) 작업 영역 영역에서 레코드 유형 카드를 클릭하여 레코드 유형의 페이지를 엽니다.
1. 다음을 클릭합니다. **자세히** 레코드 종류 이름의 오른쪽에 있는 메뉴를 클릭한 다음 **이름 바꾸기** 레코드 유형의 이름을 변경하려면

   또는

   헤더에서 레코드 유형의 이름을 변경합니다.  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   레코드 유형 페이지의 헤더에서 레코드 유형의 이름을 바꿀 수도 있습니다.
1. (선택 사항) 레코드 유형 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 편집할 다른 레코드 유형을 선택합니다.
