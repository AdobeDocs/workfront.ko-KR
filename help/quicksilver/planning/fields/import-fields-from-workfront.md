---
title: Adobe Workfront에서 필드 가져오기
description: Adobe Workfront Planning에서 각 레코드 유형에 대한 사용자 정의 필드를 만들 수 있습니다. 그런 다음 필드를 Workfront Planning 레코드와 연결할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 7%

---

<!--add to TOC-->

# Adobe Workfront에서 필드 가져오기

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


{{planning-important-intro}}

기존 Workfront 필드의 복사본을 가져올 수 있습니다. Workfront에서 필드를 가져오면 Workfront Planning 레코드 유형에 대한 각 필드의 사본이 만들어집니다.


## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항 보기..

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
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
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
   <td><p> 표준 </p>
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
   <td>   <p>작업 영역 <span class="preview"> 및 레코드 종류</span> </a>에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자에게는 작성하지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한이 있습니다.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Workfront에서 필드 가져오기에 대한 고려 사항

* 기본 또는 사용자 지정 Workfront 필드를 Workfront Planning의 레코드 유형으로 가져올 수 있습니다.
* Workfront 필드를 가져오면 동일한 필드의 복사본이 만들어지고 Workfront Planning에서 필드 이름이 유지됩니다. 이러한 필드는 Workfront Planning에 복사되면 원래 Workfront 필드와 독립적이며 정보를 공유하지 않습니다.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* 다음 Workfront 개체에서 기본 또는 사용자 지정 필드를 추가할 수 있습니다.
   * 포트폴리오
   * 프로그램
   * 프로젝트
   * 작업
   * 문제
   * 문서
   * 회사
   * 그룹
   * 사용자
   * 작업 역할
   * 할당
   * 시간
   * 청구 기록
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * 경비
   * 반복
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* Workfront 필드를 Workfront Planning에서 가져온 후 필드 유형이 유지되지 않을 수 있습니다.

  아래 표는 Workfront 필드 유형과 해당 Workfront Planning 필드 유형을 보여 줍니다.

  | Workfront 필드 유형 | Workfront Planning 필드 유형 |
  |------------------------------------------|-------------------------------|
  | 텍스트 서식 있는 한 줄 텍스트 | 한 줄 텍스트 |
  | 숫자 형식의 한 줄 텍스트 | 숫자 |
  | 통화 형식의 한 줄 텍스트 | 통화 |
  | 단락 | 단락 |
  | 서식 포함 텍스트 | 단락 |
  | 단일 선택 드롭다운 | 단일 선택 |
  | 다중 선택 드롭다운 | 다중 선택 |
  | 사용자 자동 완성 필터는 지원되지 않습니다. | 사용자 |
  | 계산됨* | 공식 |
  | 일자 | 일자 |
  | 확인란 그룹 | 다중 선택 |
  | 라디오 단추 | 다중 선택 |

  *계산된 필드는 나중에 사용할 수 있습니다.
다른 모든 Workfront 필드 유형은 Workfront Planning에서 지원되지 않습니다.


## Workfront에서 필드 가져오기

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. 필드를 만들 레코드 유형의 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.

1. 기록 유형의 카드를 클릭합니다.

   레코드 유형과 연관된 모든 기존 레코드는 테이블 뷰의 행에 표시됩니다.

   >[!TIP]
   >
   >    일부 필드가 숨겨져 있을 수 있습니다. **필드**&#x200B;를 클릭하고 테이블 보기에서 열로 보려는 필드에 대해 토글을 활성화합니다.

1. 테이블 보기의 오른쪽 위 모서리에 있는 **+** 아이콘을 클릭합니다

   또는

   열 머리글 위로 마우스를 가져간 후 필드 이름 뒤에 있는 아래쪽 화살표를 클릭한 다음 **왼쪽 삽입** 또는 **오른쪽 삽입**&#x200B;을 클릭하여 새 필드를 추가합니다.
1. **새 필드** 탭의 오른쪽 아래 모서리에 있는 **기존 필드 추가**&#x200B;를 클릭합니다. <!--check UI - did they change this??-->

   ![Workfront 모달에서 기존 필드 추가](assets/add-existing-fields-from-workfront-modal.png)

1. 검색 영역에서 기존 Workfront 필드의 이름을 입력한 다음 목록에 표시될 때 **+**&#x200B;을(를) 클릭합니다.
1. (선택 사항) 다른 필드를 입력한 다음 목록에 표시될 때 **+**&#x200B;을(를) 클릭합니다.
1. (선택 사항) **필터** 아이콘 ![필드 가져오기의 필터 아이콘](assets/filters-in-import-fields-icon.png)을 클릭한 다음, 다음 필드 중 하나 또는 둘 다를 업데이트합니다.

   * 오브젝트 유형: 가져올 필드의 Workfront 오브젝트 유형을 선택합니다.
   * 사용자 정의 양식: Workfront에서 하나 또는 여러 사용자 정의 양식을 선택합니다. 먼저 오브젝트 유형을 선택하지 않고 사용자 정의 양식을 선택할 수 있습니다.
1. **+**&#x200B;을 클릭한 다음 **필드 추가**를 클릭합니다.
필드는 표 보기 및 레코드의 세부 사항 페이지에 추가됩니다.

   >[!IMPORTANT]
   >
   >    모든 레코드 유형에는 500개의 필드로 제한됩니다. 가져온 필드와 함께 기존 필드가 이 제한에 기여합니다.

   추가된 필드는 Workfront 필드의 사본이며 더 이상 Workfront의 원래 필드에 연결되지 않습니다.
