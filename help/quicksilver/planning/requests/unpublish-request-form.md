---
title: Adobe Workfront Planning에서 요청 양식 게시 취소
description: 더 이상 필요하지 않거나 관련이 없는 요청 양식은 게시를 취소할 수 있습니다. 게시를 취소하면 양식에 액세스할 수 있는 모든 사용자의 권한이 제거됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 3%

---

# Adobe Workfront Planning에서 요청 양식 게시 취소


<!--take Preview and Production references at Production time-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

더 이상 필요하지 않거나 관련이 없는 요청 양식은 게시를 취소할 수 있습니다. 게시를 취소하면 양식에 액세스할 수 있는 모든 사용자의 권한이 제거됩니다.

요청 양식을 더 작은 그룹의 사용자가 사용할 수 있도록 유지하려면 요청 양식과 공유한 엔터티를 변경할 수도 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront 계획<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td>
   <td>
<p>다음 Workfront 플랜 중 하나:</p>
<ul><li>선택</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td>
   <td>
<p>임의 </p>  
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td>
   <td>
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <ul>
   <li><p>작업 영역 <span class="preview"> 및 레코드 종류</span>에 대한 권한을 관리합니다. </p></li>
    <li><p>시스템 관리자는 자신이 만들지 않은 작업 공간을 관리할 수 있습니다. </p></li>
    </ul>
   <p>Workfront Planning 객체의 권한 공유에 대한 자세한 내용은  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning의 공유 권한 개요</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>프로덕션 환경에서는 시스템 관리자를 포함한 모든 사용자를 Planning이 포함된 레이아웃 템플릿에 할당해야 합니다.</p>
<p><span class="preview">미리보기 환경에서 표준 사용자 및 시스템 관리자는 기본적으로 Planning을 활성화합니다.</span></p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 양식 공유 변경

에 대한 요청을 조직 외부의 사용자를 포함한 모든 사용자와 공개적으로 공유하는 경우, 양식이 연결된 작업 영역을 보거나 관리하는 특정 사용자에게 이 액세스를 제한하는 것이 좋습니다.

요청 양식 공유를 변경하려면:

{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.

1. 페이지 헤더의 레코드 종류 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **요청 양식 관리**&#x200B;를 클릭합니다.

   레코드 유형과 연관된 모든 요청 양식이 테이블 보기에 표시됩니다.
1. 요청 양식 이름 위로 마우스를 가져간 후 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **공유**&#x200B;를 클릭합니다.
1. 다음 중 하나를 선택하여 공유 선택 사항을 업데이트합니다.

   * 작업 영역에 대한 보기 이상의 액세스 권한이 있는 모든 사용자
   * 작업 영역에 대한 참여 이상의 액세스 권한이 있는 모든 사용자
   * 링크를 보유한 모든 사용자

   자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.
1. (선택 사항) 요청 양식 공유를 변경하고 새 링크가 있는 새 사용자 그룹에 공유하려면 **링크 복사**&#x200B;를 클릭합니다.

## 레코드 유형에 대한 요청 양식 게시 취소

요청 양식이 무관해져서 더 이상 아무도 액세스할 수 없게 되면 게시를 취소할 수 있습니다.

{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.

1. 페이지 헤더의 레코드 종류 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **요청 양식 관리**&#x200B;를 클릭합니다.

   레코드 유형과 연관된 모든 요청 양식이 테이블 보기에 표시됩니다.
1. 요청 양식 이름을 마우스로 가리킨 다음 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **게시 취소**&#x200B;를 클릭합니다

또는

요청 양식 이름을 클릭하여 연 다음 요청 양식의 오른쪽 상단 모서리에서 **게시 취소**&#x200B;를 클릭합니다.

![게시 취소 단추 강조 표시](assets/unpublish-button-highlighted.png)

양식 게시가 취소되었음을 알리는 확인 메시지가 화면 하단에 표시됩니다.

**게시 취소** 링크 또는 단추가 **게시**(으)로 변경됩니다.

1. (조건부) 양식을 연 후 게시를 취소한 경우 **저장**&#x200B;을 클릭합니다.

   사용자는 더 이상 Workfront의 요청 영역에 있는 링크 또는 요청 큐에서 요청 양식에 액세스할 수 없습니다.

   요청 양식을 사용하여 이전에 추가한 모든 레코드는 레코드 유형 페이지에 그대로 유지됩니다.

   이전에 추가한 모든 요청은 계획 탭의 Workfront 요청 영역에 남아 있습니다.
