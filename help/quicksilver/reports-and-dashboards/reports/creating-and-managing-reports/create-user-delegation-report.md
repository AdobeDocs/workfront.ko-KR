---
product-area: reporting
keywords: 사용자,위임,보고서,위임,승인
navigation-topic: create-and-manage-reports
title: 사용자 위임 보고서 만들기
description: 사용자 위임 보고서 만들기
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# 사용자 위임 보고서 만들기

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

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>승인이 위임된 항목 및 위임에 관련된 사용자에 대한 권한을 봅니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 사용자 위임 보고서 만들기

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **보고서**&#x200B;를 클릭합니다.

1. **새 보고서**&#x200B;를 클릭한 다음 **사용자 위임**&#x200B;을 선택합니다.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   이 보고서에는 기본적으로 다음 필드가 표시됩니다.

   | 필드 | 설명 |
   |---|---|
   | **사용자로부터** | 이 사용자는 작업, 문제 및 프로젝트 승인을 다른 사용자에게 위임하는 사용자입니다. |
   | **사용자에게** | 작업, 문제 및 프로젝트 승인이 위임된 사용자입니다. |
   | **시작** | 위임을 수행한 사용자의 종료 시간이 시작됩니다. |
   | **종료** | 위임을 수행한 사용자의 종료 시간입니다. |

   {style="table-layout:auto"}

1. (선택 사항) Report Builder에서 다음을 수정합니다.

   * 열
   * 그룹화
   * 필터
   * 차트

   이러한 기능에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

1. 보고서 작성이 끝나면 **저장 + 닫기**&#x200B;를 클릭합니다.

1. **보고서 이름** 필드에 새 이름을 입력한 다음 **보고서 저장**&#x200B;을 클릭합니다.

   보고서가 표시됩니다.
