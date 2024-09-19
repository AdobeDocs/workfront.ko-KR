---
product-area: home
navigation-topic: use-the-home-area
title: 내 작업 위젯을 사용하여 작업 관리
description: 내 작업 위젯은 할당된 모든 작업, 문제 및 요청을 한 곳에 표시합니다. 여기에서 작업을 필터링 및 구성하고 시간을 기록하며 업데이트하고 작업 항목을 완료로 표시할 수 있습니다.
author: Courtney
feature: Get Started with Workfront
source-git-commit: c96169186af3bc83b823ec8870173911cf546091
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 5%

---


# 내 작업 위젯을 사용하여 작업 관리

내 작업 위젯은 할당된 모든 작업, 문제 및 요청을 한 곳에 표시합니다. 여기에서 작업을 필터링 및 구성하고 시간을 기록하며 업데이트하고 작업 항목을 완료로 표시할 수 있습니다.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td> <p>현재: Contribute</p>
   <p>또는</p> 
   <p>새로 만들기:[!UICONTROL Light] 이상<p> 
  </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>프로젝트, 작업, 문제 및 문서에 대한 [!UICONTROL 보기] 이상 액세스 권한</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 대한 Contribute 권한 이상</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 필터를 사용하여 작업 찾기

내 작업 필터를 미세 조정하여 작업 목록의 특정 항목에 집중할 수 있습니다.

![](assets/filter-my-work-widget.png)

### 필터 세부 정보

<table>
  <tbody>
    <tr>
      <td>작업 중</td>
      <td>현재 작업 중인 항목을 표시합니다.</td>
    </tr>
    <tr>
      <td>시작 준비 완료</td>
      <td>항목이 있는 항목 표시 
      <ul>
      <li>완료되지 않은 전임 작업 또는 작업 제한 없음</li>
      <li>계획된 시작 일자가 과거 또는 최대 2주 미래입니다.</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>준비 안 됨</td>
      <td>다음과 같은 항목이 있는 항목 표시
       <ul>
      <li>항목이 작업되지 않도록 하는 불완전한 전임 작업 또는 작업 제한</li>
      또는
      <li>2주 이상 후의 계획된 시작 일자</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>요청됨</td>
      <td>작업을 시작하지 않은 문제를 표시합니다.</td>
    </tr>
    <tr>
      <td>내가 위임함</td>
      <td>다른 사용자에게 위임한 항목을 표시합니다.</td>
    </tr>
    <tr>
      <td>내게 위임함</td>
      <td>사용자가 귀하에게 위임한 항목을 표시합니다.</td>
    </tr>
    <tr>
      <td>완료됨</td>
      <td>지난 2주 이내에 완료된 작업을 표시합니다. 이 필터 옵션에는 승인이 포함되지 않습니다.</td>
    </tr>
  </tbody>
</table>

>[!TIP]
>
>보다 구체적인 필터링 옵션을 원하는 경우 내 작업 또는 내 문제 위젯을 사용할 수 있습니다. 내 작업 및 내 문제 필터에 대한 자세한 내용은 [새 홈 위젯 필터 개요](/help/quicksilver/workfront-basics/using-home/new-home/widget-filter-overview-new-home.md)를 참조하세요.

## 작업 구성

내 작업 위젯의 정렬 및 그룹 기능을 사용하여 자신에게 적합한 방식으로 작업을 구성할 수 있습니다.

### 정렬

작업 목록 정렬 기준:

* 기한
기한이 지난 항목은 날짜 옆에 경고 아이콘을 표시합니다. Workfront은 계획된 완료 일자를 사용하여 작업 및 문제의 기한이 지났는지 확인합니다.
* 이름
* 완료율
* 상태

>[!TIP]
>
>내 작업 위젯의 맨 위에 모든 기한 경과 항목을 표시하는 목록을 만들려면 기한을 기준으로 정렬하고 그룹을 적용하지 마십시오.


![](assets/sort-my-work-widget.png)

### 그룹

작업 목록을 다음 기준으로 그룹화할 수 있습니다

* 프로젝트
* 상태
* 기한
계획된 완료 일자에 의해 납기 일자가 결정됩니다.

>[!NOTE]
>
>그룹화를 적용하면 [정렬] 메뉴에서 선택한 항목에 따라 그룹화 내의 순서가 결정됩니다.


![](assets/group-my-work-widget.png)

## 요약에서 작업 항목 정보 업데이트

요약 패널을 열어 작업 또는 문제의 정보를 신속하게 업데이트할 수 있습니다. 요약에서 다음을 수행할 수 있습니다.

* 완료율 업데이트
* 업데이트 추가
* 문서 영역으로 이동하여 문서 업로드
* 작업 항목 세부 정보 보기 및 사용자 정의 필드 업데이트
Workfront 관리자는 레이아웃 템플릿의 요약에 표시되는 필드를 사용자 정의할 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 홈 및 요약 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)을 참조하십시오.
* 작업 항목 상태 변경
* 하위 작업 보기
* 로그 시간
* 첨부된 승인 진행 보기

요약을 열려면 작업 항목 위로 마우스를 가져간 다음 **요약** 아이콘 ![](assets/open-summary-new-home.png)을(를) 클릭합니다.

요약 패널 사용 방법에 대한 자세한 내용은 [요약 개요](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)를 참조하십시오.

## 빠른 작업을 사용하여 작업 항목 업데이트

빠른 작업 메뉴를 사용하여 다음 작업을 수행할 수 있습니다.

* 로그 시간
* 업데이트 추가
* 사용자 정의 양식 업데이트
* 파일 업로드

빠른 작업 메뉴를 찾으려면 작업 항목 위로 마우스를 가져갑니다. 빠른 작업 목록은 **처리 중** 또는 **완료** 단추 근처에 표시됩니다.

![](assets/quick-actions-new-home.png)


## 승인 및 팀 요청 보기

승인 및 팀 요청이 내 작업 위젯에 표시되지 않습니다. 승인 및 팀 요청으로 정기적으로 작업하는 경우 새 홈 페이지에 다음 위젯을 추가하는 것이 좋습니다.

* 승인 대기 중
* 모든 승인
* 팀 요청

새 홈 페이지에 위젯을 추가하는 방법에 대한 자세한 내용은 [새 홈에서 위젯 추가, 편집 또는 제거](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md)를 참조하십시오.




