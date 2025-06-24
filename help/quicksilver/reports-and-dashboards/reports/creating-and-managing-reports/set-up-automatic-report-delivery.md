---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 자동 보고서 배달 예약
description: 자동 보고서 배달 예약
author: Courtney
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 62f56486ccc590921b7dc8227d46cdede84df32d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# 자동 보고서 배달 예약

<!-- Audited: 4/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

정의된 일정에 따라 보고서를 사용자에게 자동으로 전달하도록 예약하거나 보고서를 수동으로 한 번 보낼 수 있습니다. Adobe Workfront에서 보고서를 보내면 사용자는 별도의 첨부 파일에서 Workfront 보고서가 포함된 이메일을 받게 됩니다.

보고서 배달에 영향을 줄 수 있는 크기 제한을 포함한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
      <td> 
      <p>새로운 기능: 표준</p>
      <p>또는</p>

<p>현재: 플랜</p>

</td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 보고서를 만들어야 합니다. 보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하세요.

## 보고서 배달 예약


보고서를 자동 게재하도록 예약하려면 다음을 수행합니다&#x200B;.

{{step1-to-reports}}

>[!NOTE]
>
>보고서 게재에 프롬프트가 포함되어 있지 않습니다. 보고서 게재에서 데이터를 제한하려면 전송할 보고서에 필터를 적용하는 것이 좋습니다.

1. **보고서** 페이지에서 보고서를 선택하십시오.
1. 화면 맨 위에서 표시되는 드롭다운에서 **보고서 작업**&#x200B;을 클릭한 다음 **보고서 보내기**&#x200B;를 클릭합니다. **보고서 보내기** 대화 상자가 표시됩니다.

   >[!TIP]
   >
   >지정된 시간에 수동으로 보고서를 보내려면 해당 보고서로 이동한 다음 **보고서 작업** > **보고서 보내기** > **지금 보내기**&#x200B;를 클릭합니다.

1. **반복 게재** 탭을 선택합니다.
1. (조건부) 기존 반복 보고서 배달을 수정하려면 대화 상자의 오른쪽에 있는 **반복 배달** 섹션에서 보고서 배달을 선택합니다.
1. 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>전송 대상</p> </td> 
      <td> <p>보고서를 보낼 사용자, 그룹, 팀 또는 역할의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.</p> <p>또는</p> <p>보고서에 액세스하려는 Workfront 시스템 외부 사용자의 이메일 주소를 입력합니다.</p> <p>이 프로세스를 반복하여 여러 사용자, 그룹, 팀 또는 역할에 보고서를 전송합니다.</p> <p>참고:  <p>보고서 게재 수신자를 추가할 때 다음 사항을 고려하십시오.</p> 
        <ul> 
         <li><p>조직에서 Workfront 알림을 특정 이메일 도메인으로 제한하는 경우 이메일 허용 목록에 추가하다에 나열된 이메일 주소로만 보고서를 보낼 수 있습니다.</p> <p>예를 들어, 사용자가 보고서 수신자로 설정되어 이전에 허가한 이메일 주소를 가지고 있고, 허용 목록에 추가하다가 해당 도메인에 더 이상 이메일을 배달하지 못하도록 업데이트하면 사용자는 더 이상 배달된 보고서를 받지 않습니다.</p><p>Workfront 허용 목록에 추가하다 허용 목록에 추가하다 관리자가 전자 메일을 업데이트하는 방법에 대한 자세한 내용은 &lbrace;전자 메일 구성</a> 섹션을 참조하십시오.<a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref"></p></li> 
         <li> <p>많은 사용자를 수신자로 추가하면 게재가 실패할 수 있습니다. 게재 오류가 발생하는 경우 더 작은 사용자 그룹과 함께 여러 보고서 게재를 예약할 수 있습니다.</p> </li> 
        </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>이메일 제목</p> </td> 
      <td> <p>이메일 알림의 제목을 입력합니다.</p> <p>기본적으로 이메일 제목은 다음과 같습니다.</p> <p><em>Workfront 보고서: [보고서 이름] [날짜]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>이메일 메시지</p> </td> 
      <td> <p>이메일에 포함할 메시지를 입력합니다.</p> <p>기본적으로 이메일 메시지는 다음과 같습니다.</p> <p><em>Workfront에서 [Date]에 생성한 [보고서 빈도] 보고서 [보고서 이름]을(를) 첨부했습니다.</em> </p> <p>참고: Excel 파일로만 제공되는 보고서의 경우 다음과 같은 메시지도 전자 메일에 추가됩니다. "MS Excel(XLS) 파일 형식의 경우 이러한 파일 형식이 지원하는 하이퍼링크 수에 제한(65,530)이 있습니다. 이러한 제한을 초과하는 경우 파일이 열리지 않으며 하이퍼링크 없이 다시 전송하는 것이 좋습니다. 하이퍼링크를 제거하고 보고서를 다시 보내려면 보고서 스케줄러로 돌아가십시오." "보고서 스케줄러로 돌아가기" 구문은 보고서에 대한 링크입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>다음의 액세스 권한으로 이 보고서 게재</p> </td> 
      <td> <p>보고서에 액세스할 수 있는 사용자의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다. 보고서를 받는 사용자에게는 여기에서 지정한 사용자와 동일한 수준의 보고서 액세스 권한이 부여됩니다.<br> 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">다른 사용자의 액세스 권한으로 보고서 실행 및 전달</a>을 참조하십시오.</p> <p>참고: 이 필드는 와일드카드를 지원하지 않습니다. 예를 들어 와일드카드 <em>$$User.ID</em>을(를) 사용하면 보고서를 받는 사용자의 액세스 권한으로 보고서를 실행하지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>형식</p> </td> 
      <td> <p>게재된 보고서에 사용할 형식을 선택합니다.</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>PDF을 선택하면 표시되는 추가 <strong>용지 크기</strong> 및 <strong>방향</strong> 옵션을 사용하여 출력 형식을 지정할 수 있습니다.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>링크 포함</p> </td> 
      <td> <p>이 옵션은 <strong>서식</strong> 드롭다운 메뉴에서 <strong>MS Excel</strong>을(를) 선택한 경우에만 사용할 수 있습니다. 이 옵션을 활성화하면 내보낸 Excel 문서에 모든 하이퍼링크가 포함됩니다.</p> <p>링크가 65,530개를 초과하는 문서는 열 수 없습니다. 내보낸 문서에 65,530개 이상의 링크가 포함된 경우 이 옵션을 선택 취소합니다.</p> <p>이 옵션은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>요약</p> </td> 
      <td> <p>게재 반복 시 요약을 표시합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>반복</p> </td> 
      <td> <p>보고서를 일별, 주별, 월별 또는 연별로 배달할지 여부를 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>모두 반복</p> </td> 
      <td> <p>게재를 반복할 빈도를 선택합니다. 이 옵션에 대해 선택하는 값은 <strong>반복</strong> 드롭다운 목록에서 선택한 옵션을 기반으로 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>시간</p> </td> 
      <td> <p>게재를 보낼 시간을 선택합니다.</p> <p>팁: 시스템 로드는 보고서 배달 시간에 영향을 줄 수 있으므로 예약된 시간과 실제 배달 시간 사이에 최대 24시간의 지연이 있을 수 있습니다. 특정 시간까지 보고서를 배달해야 하는 경우에는 필요한 시간 전에 배달을 예약하는 것이 좋습니다. 일반적으로 필요한 날짜보다 최소 하루 전에 게재를 예약하는 것이 좋습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>반복 일자</p> </td> 
      <td> <p>이 옵션은 <strong>반복</strong> 옵션이 <strong>주별</strong> 또는 <strong>월별</strong> 중 하나로 설정된 경우에 사용할 수 있습니다.</p> 
       <ul> 
        <li> <p><strong>반복</strong> 옵션이 <strong>주별</strong>(으)로 설정된 경우: 게재를 보낼 요일을 선택합니다.</p> </li> 
        <li> <p><strong>반복</strong> 옵션이 <strong>월별</strong>(으)로 설정된 경우: 배달이 해당 월의 날짜, 요일 또는 마지막 날에 전송되는지 여부를 선택합니다. 이러한 옵션은 <strong>시작 날짜</strong> 필드에서 선택한 날짜를 활용합니다.</p> </li> 
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
      <td>예약된 배달이 무기한 지속되도록 하려면 <strong>절대 안 함</strong>을(를) 선택하십시오.</td> 
     </tr> 
    </tbody> 
   </table>

1. 보고서 배달을 저장하려면 **저장**&#x200B;을 클릭하세요. 보고서는 **보고서 보내기** 대화 상자의 **반복 배달** 섹션에 표시되며 예약된 시간에 전송됩니다.

   보고서 배달에 영향을 줄 수 있는 크기 제한에 대한 자세한 내용은 [보고서 배달 제한](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) 및 [내보내기 제한](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export) 섹션을 참조하십시오.

>[!IMPORTANT]
>
>예약된 보고서는 배달을 위해 처리될 때 내부 시간 제한을 받습니다. 보고서를 보내는 데 제한 시간보다 오래 걸리는 경우 알림을 받게 되며 나머지 예약된 배달에 관계없이 보고서가 더 이상 배달되지 않습니다. 보고서를 계속 보내려면 먼저 필터 및 보기를 통해 보고서 크기를 줄인 다음 예약된 새 게재를 만듭니다.
>
>예약된 보고서 배달을 사용하여 BI 도구를 통해 Workfront 데이터를 분석하는 경우 Workfront Data Connect를 대신 사용하는 것이 좋습니다. 자세한 내용은 [Workfront Data Connect 개요](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md)를 참조하십시오.

## 예약된 보고서 게재 삭제

예약된 보고서 게재를 삭제하려면 다음을 수행합니다&#x200B;.

{{step1-to-reports}}

1. **보고서** 페이지에서 보고서를 선택하십시오.

1. 화면 맨 위에서 표시되는 드롭다운에서 **보고서 작업**&#x200B;을 클릭한 다음 **보고서 보내기**&#x200B;를 클릭합니다. **보고서 보내기** 대화 상자가 표시됩니다.

1. **반복 게재** 탭을 선택합니다.
1. 대화 상자 오른쪽의 **반복 게재** 섹션에서 삭제할 예약된 게재를 클릭합니다.
1. **반복 게재** 세부 정보 섹션에서 **삭제**&#x200B;를 클릭합니다.

1. 확인하려면 **삭제**&#x200B;를 클릭하세요.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


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
