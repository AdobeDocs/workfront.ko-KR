---
product-area: reporting
keywords: 사용자,위임,보고서,위임,승인
navigation-topic: create-and-manage-reports
title: 사용자 위임 보고서 만들기
description: 사용자 위임 보고서 만들기
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 2%

---

# 사용자 위임 보고서 만들기

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

Adobe Workfront에서 사용자는 프로젝트, 작업 및 문제 승인을 다른 사용자에게 위임하여 사용자가 부재 중일 때 승인이 관리되도록 할 수 있습니다. 플랜 라이선스가 있는 사용자는 사용자 위임 보고서를 만들어 다음을 볼 수 있습니다.

* 작업, 문제 및 프로젝트 승인을 다른 사용자에게 위임한 사용자
* 작업, 문제 및 프로젝트 승인이 할당된 사용자

* 위임이 시작되고 종료되는 날짜

승인 위임에 대한 자세한 내용은 [승인 요청 위임](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)을 참조하세요.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
      <p>표준</p>
      <p>플랜</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
 <td> <p>승인이 위임된 항목 및 위임에 관련된 사용자에 대한 권한을 봅니다</p></td>  
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 위임 보고서 만들기

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **보고서**&#x200B;를 클릭합니다.

1. **새 보고서**&#x200B;를 클릭한 다음 **사용자 위임**&#x200B;을 선택합니다.

   ![새 보고서 사용자 위임](assets/classic-new-report-user-delegation-350x644.png)

   이 보고서에는 기본적으로 다음 필드가 표시됩니다.

   | 필드 | 설명 |
   |---|---|
   | **사용자로부터** | 이 사용자는 작업, 문제 및 프로젝트 승인을 다른 사용자에게 위임하는 사용자입니다. |
   | **사용자에게** | 작업, 문제 및 프로젝트 승인이 위임된 사용자입니다. |
   | **시작 날짜** | 위임을 수행한 사용자의 종료 시간이 시작됩니다. |
   | **종료 날짜** | 위임을 수행한 사용자의 종료 시간입니다. |

   {style="table-layout:auto"}

1. (선택 사항) Report Builder에서 다음을 수정합니다.

   * 열(조회)
   * 그룹화
   * 필터
   * 차트

   이러한 기능에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

1. 보고서 작성이 끝나면 **저장 + 닫기**&#x200B;를 클릭합니다.

   보고서가 표시됩니다.
