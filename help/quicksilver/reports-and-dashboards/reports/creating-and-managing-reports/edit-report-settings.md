---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 보고서 설정 편집
description: 보고서의 설정을 편집하여 다른 사용자에게 표시되는 방법이나 사용자가 보고서를 실행하기 전에 어떤 정보를 묻는 메시지를 표시할 수 있는지 정의할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 6%

---

# 보고서 설정 편집

보고서의 설정을 편집하여 다른 사용자에게 표시되는 방법이나 사용자가 보고서를 실행하기 전에 어떤 정보를 묻는 메시지를 표시할 수 있는지 정의할 수 있습니다.

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
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 방법 단계

1. 로 이동하여 보고서 만들기 시작 **메인 메뉴** > **보고서**&#x200B;를 클릭한 다음 보고서의 개체를 선택합니다.

   또는

   기존 보고서를 연 다음 **보고서 작업** > **편집**.

1. 클릭 **보고서 설정** report builder의 오른쪽 상단 모서리에서
1. 다음 보고서 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">보고서 제목</td> 
      <td>보고서 제목을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>보고서의 목적 및 용도를 설명하는 문을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">다음의 액세스 권한으로 이 보고서 실행:</td> 
      <td>다른 사용자를 위해 이 보고서를 표시할 때 사용할 액세스 권한을 가진 사용자를 선택합니다. 다른 사용자의 액세스 권한으로 보고서를 실행하는 방법에 대한 자세한 내용은 문서를 참조하십시오 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">다른 사용자의 액세스 권한으로 보고서 실행 및 전달</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서가 로드되면</td> 
      <td>보고서가 로드될 때 모든 사용자에 대해 표시되는 기본 탭을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서가 대시보드에 로드되면 ... 항목을 표시합니다.</td> 
      <td>보고서가 대시보드에 로드될 때 모든 사용자에 대해 표시되는 항목 수를 지정합니다. 기본값은 15개 항목이며 최대 항목 수는 200개입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">세부 정보 탭에서 리소스 그리드 보기 표시</td> 
      <td> <p>(사용자 보고서만 해당) 이 옵션을 선택하면 보고서의 세부 정보 탭에 리소스 그리드가 표시됩니다.</p> <p>참고: 사용자 보고서에 리소스 그리드 보기를 적용하면 보고서에는 현재 상태에 있는 프로젝트만 표시됩니다. 다른 상태에서 프로젝트를 보려면 전역 탐색 막대의 사람 영역에서 사용자 활용성 탭을 사용하여 리소스 그리드 보기를 적용할 수 있습니다. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">세부 정보 탭에서 특별 보기 표시</td> 
      <td>(프로젝트 보고서만 해당) 사용자가 세부 정보 탭에서 이 정보에 액세스할 때 표시되는 보기 유형을 지정합니다. 예를 들어 마일스톤 또는 간트 보기를 선택할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본으로 간트 보기에서 이 보고서 표시</td> 
      <td>(프로젝트 보고서 및 작업 보고서만 해당) 사용자가 이 보고서의 세부 정보 탭을 볼 때 간트 보기를 자동으로 활성화하려면 이 옵션을 선택합니다.<br>프로젝트 보고서 및 작업 보고서에서 간트 차트를 보는 방법에 대한 자세한 내용은 문서의 "프로젝트 목록 간트 차트에서 작업 정보 보기" 섹션을 참조하십시오 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">간트 차트에서 정보 보기 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서에서 보기 변경 가능</td> 
      <td>사용자가 보고서를 실행할 때 보기를 변경할 수 있도록 하려면 이 옵션을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서에서 그룹 변경 가능</td> 
      <td>보고서를 실행할 때 사용자가 그룹을 변경할 수 있도록 하려면 이 옵션을 선택하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">보고서에서 필터를 변경할 수 있도록 허용</td> 
      <td>사용자가 보고서를 실행할 때 필터를 변경할 수 있도록 하려면 이 옵션을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **보고서 프롬프트** 를 클릭하여 보고서에 대한 프롬프트를 설정합니다.\
   보고서에 프롬프트를 추가하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 클릭&#x200B;**완료,** 그런 다음 을 클릭합니다. **저장 + 닫기**.

## 추가 정보

다음도 참조하십시오.

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [보고서 시작](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Adobe Workfront 기본 제공 보고서 사용](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
