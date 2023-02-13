---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 자동 보고서 배달 예약
description: 자동 보고서 배달 예약
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 3%

---

# 자동 보고서 배달 예약

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

정의된 일정에 따라 사용자에게 보고서를 자동으로 전달하도록 예약하거나 보고서를 수동으로 한 번에 전송할 수 있습니다. Adobe Workfront에서 보고서를 보내면 사용자는 별도의 첨부 파일로 Workfront 보고서가 포함된 이메일을 받게 됩니다.

보고서 배달에 영향을 줄 수 있는 크기 제한 등 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 보고서를 만들어야 합니다. 보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 보고서 배달 예약

자동 전달을 위해 보고서를 예약하거나 기존 보고서 배달을 편집하거나 삭제하려면 다음을 &#x200B; 수행하십시오.

1. 배달 일정을 예약하려는 보고서로 이동합니다.

   >[!NOTE]
   >
   >보고서 게재에 프롬프트가 포함되지 않습니다. 보고서 배달에서 데이터를 제한하려면 전송할 보고서에 필터를 적용하는 것이 좋습니다.

1. 클릭 **보고서 작업**, 그런 다음 **보고서 보내기**.

   다음 **보고서 보내기** 대화 상자가 표시됩니다.

   >[!TIP]
   >
   >지정된 시간에 수동으로 보고서를 전송하려면 보고서로 이동한 다음 **보고서 작업** > **보고서 보내기** > **지금 보내기**.

1. 을(를) 선택합니다 **반복 게재** 탭.
1. (조건부) 기존 반복 보고서 전달을 수정하려면 **반복 게재** 섹션을 참조하십시오.
1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>다음으로 전송:</p> </td> 
      <td> <p>보고서를 보낼 사용자, 그룹, 팀 또는 역할의 이름을 입력하고 드롭다운 목록에 표시되면 이름을 클릭합니다.</p> <p>또는</p> <p>보고서에 액세스할 Workfront 시스템 외부의 개인 이메일 주소를 지정합니다.</p> <p>이 프로세스를 반복하여 여러 사용자, 그룹, 팀 또는 역할에 보고서를 보냅니다.</p> <p>참고:  <p>보고서 배달 수신자를 추가할 때 다음 사항을 고려하십시오.</p> 
        <ul> 
         <li>조직에서 Workfront 알림을 특정 이메일 도메인으로 제한하는 경우 이메일에 나열된 이메일 주소에만 보고서를 보낼 수 허용 목록에 추가하다 있습니다.<p>Workfront 관리자가 이메일을 업데이트하는 방법허용 목록에 추가하다에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">이메일 허용 목록에 추가하다 구성</a>.</p></li> 
         <li> <p>수신자로 많은 사용자를 추가하면 게재가 실패할 수 있습니다. 게재 오류가 발생하는 경우 사용자 그룹이 작은 여러 보고서 배달을 예약할 수 있습니다.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>이메일 제목</p> </td> 
      <td> <p>이메일 알림의 제목을 지정합니다.</p> <p>기본적으로 이메일 제목은 다음과 같습니다.</p> <p><em>Workfront 보고서: [보고서 이름] [날짜]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>이메일 메시지</p> </td> 
      <td> <p>이메일에 포함할 메시지를 지정합니다.</p> <p>기본적으로 이메일 메시지는 다음과 같습니다.</p> <p><em>[Date]에 Workfront이 생성한 [Report Frequency] 보고서 [Name of the report]가 첨부됩니다.</em> </p> <p>참고: Excel 파일로 전달된 보고서의 경우 다음 메시지도 이메일에 추가됩니다. "MS Excel(XLS) 파일 형식의 경우 지원되는 하이퍼링크 수에 제한(65,530)이 있습니다. 이러한 제한을 초과하는 경우 파일이 열리지 않으므로 하이퍼링크 없이 다시 보내는 것이 좋습니다. 하이퍼링크를 제거하고 보고서를 다시 보내려면 보고서 스케줄러로 돌아가십시오." "보고서 스케줄러로 돌아가기" 구문은 보고서에 대한 다시 링크입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>다음의 액세스 권한으로 이 보고서 게재</p> </td> 
      <td> <p>보고서에 액세스할 수 있는 사용자의 이름을 입력하고 드롭다운 목록에 이 이름이 표시되면 이름을 클릭합니다. 보고서를 받는 사용자에게 여기에서 지정한 사용자와 동일한 수준의 보고서 액세스 권한이 부여됩니다.<br> 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">다른 사용자의 액세스 권한이 있는 보고서를 실행하고 전달합니다</a>.</p> <p>참고: 이 필드는 와일드카드를 지원하지 않습니다. 예를 들어, 와일드카드 $$User.ID를 사용하면 보고서를 받는 사용자의 액세스 권한이 있는 보고서가 실행되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>포맷</p> </td> 
      <td> <p>배달된 보고서에 사용할 형식을 선택합니다.</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>이 옵션을 선택하면 추가 <strong>용지 크기</strong> 및 <strong>방향</strong> 표시되는 옵션입니다.</p> </li> 
        <li> <p>MS Excel(.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>링크 포함</p> </td> 
      <td> <p>이 옵션은 <strong>MS Excel</strong> 에서 선택됨 <strong>형식</strong> 드롭다운 메뉴 이 옵션을 활성화하면 내보낸 Excel 문서에 하이퍼링크가 포함됩니다.</p> <p>65,530개 이상의 링크가 포함된 문서는 열 수 없습니다. 내보낸 문서에 65,530개 이상의 링크가 포함된 경우 이 옵션을 선택 취소합니다.</p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>요약</p> </td> 
      <td> <p>게재가 반복되는 경우에 대한 요약을 표시합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>반복</p> </td> 
      <td> <p>보고서를 일별, 주별, 월별 또는 연간 중 어떤 것으로 전달해야 하는지를 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>모두 반복</p> </td> 
      <td> <p>게재를 반복할 빈도를 선택합니다. 이 옵션에 대해 선택하는 값은 <strong>반복</strong> 드롭다운 목록.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>시간</p> </td> 
      <td> <p>게재를 보낼 시간을 선택합니다.</p> <p>팁: 시스템 로드는 보고서 배달 시간에 영향을 줄 수 있으므로 예약된 시간과 실제 배달 시간 사이에 지연이 있을 수 있습니다. 특정 시간까지 보고서를 배달해야 하는 경우 필요한 시간 전에 게재를 예약하는 것이 좋습니다. 예를 들어 필요한 날짜 전날에 게재를 예약하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>반복 일자</p> </td> 
      <td> <p>이 옵션은 <strong>반복</strong> 옵션이 다음 중 하나로 설정되어 있습니다. <strong>주별</strong> 또는 <strong>월별</strong>:</p> 
       <ul> 
        <li> <p>이 <strong>반복</strong> 옵션이 <strong>주별</strong>: 게재를 보낼 요일을 선택합니다.</p> </li> 
        <li> <p>이 <strong>반복</strong> 옵션이 <strong>월별</strong>: 게재가 해당 월의 일, 요일 또는 월의 마지막 날에 전송되는지 여부를 선택합니다(이러한 옵션은 <strong>시작 시간</strong> 필드)만 로드하는 것입니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>다음에 시작:</p> </td> 
      <td>예약된 게재를 시작할 날짜를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>종료 일자</p> </td> 
      <td>예약된 배달이 종료될 날짜를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>안 함</p> </td> 
      <td>선택 <strong>절대 안 함</strong> 예약된 게재를 무기한 유지하려면</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **저장** 보고서 배달을 저장하려면 을 클릭합니다.

   보고서는 **반복 게재** 섹션(에서) **보고서 보내기** 대화 상자)를 클릭하여 예약된 시간에 전송됩니다.

   보고서 배달에 영향을 줄 수 있는 크기 제한에 대한 자세한 내용은 섹션을 참조하십시오 [보고서 배달 제한](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) 및 [내보내기 제한](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. (선택 사항) 예약된 게재를 삭제하려면

   1. 에서 **반복 게재** 패널에서 예약된 게재를 클릭한 다음 **삭제**.
   1. 클릭 **삭제** 확인합니다.

## 비디오 둘러보기

다음 비디오를 보고 보고서 배달을 예약하는 방법을 알아보십시오. 이 비디오는 Workfront Classic에 녹화되었습니다. 하지만 컨텐츠는 새로운 Workfront 경험에도 적용됩니다.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
