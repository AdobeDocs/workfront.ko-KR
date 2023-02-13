---
user-type: administrator
product-area: system-administration
keywords: kicstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: 킥스타트를 통해 Adobe Workfront에서 데이터 내보내기
description: Adobe Workfront 관리자는 Kick-Starts 데이터 내보내기 를 사용하여 Workfront에서 데이터를 내보낼 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# 킥스타트를 통해 Adobe Workfront에서 데이터 내보내기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Adobe Workfront 관리자는 Kick-Starts 데이터 내보내기 를 사용하여 Workfront에서 데이터를 내보낼 수 있습니다. 내보낸 후에 다른 응용 프로그램에서 사용할 수 있습니다.

Kick-Starts를 통해 데이터를 내보내면 각 개체와 어떤 필드가 연결되는지, 이러한 필드가 어떻게 코딩되는지, 그리고 데이터베이스에서 이러한 필드의 값이 어떻게 형식화되어 있는지 이해하는 데에도 유용합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## kick-starts를 사용하여 데이터를 내보낼 때의 장점과 단점

Workfront 내에서 데이터를 내보내는 방법에는 두 가지가 있습니다.

* 보고서 또는 목록에서 데이터 내보내기

   보고서 또는 목록에서 데이터 내보내기에 대한 자세한 내용은 [데이터 내보내기](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* kick-starts를 통해 데이터 내보내기

다음 표는 각 메서드의 장점과 단점을 보여줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>내보낸 데이터에 개체 및 필드 값이 포함됨</p> </th> 
   <th> <p>여러 객체 유형에 대한 데이터를 동시에 내보내는 기능</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>목록 보기에서 데이터 내보내기</strong> </p> <p>목록에서 데이터 내보내기에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">데이터 내보내기</a></p> </td> 
   <td> <p>예</p> <p>Workfront 기본 필드와 개체와 연결된 사용자 지정 필드를 모두 내보냅니다.</p> </td> 
   <td> <p>아니요</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>킥스타트를 통해 데이터 내보내기</strong> </p> </td> 
   <td> <p>예(제한됨)</p> <p>개체와 연결된 대부분의 Workfront 기본 필드는 내보내지지만 일부는 내보내지지 않습니다. 예를 들어 프로젝트 킥시작 내보내기를 통해 일정, 프로젝트 소유자 또는 프로젝트 스폰서 필드를 내보낼 수 없습니다.</p> <p>사용자 지정 양식이 첨부된 프로젝트에서 양식의 필드에 입력한 데이터는 내보내지지 않습니다.</p> <p>그러나 사용자 지정 양식을 내보낼 수 있습니다. 결과 파일에는 텍스트 상자 및 라디오 단추와 같이 양식에 구성된 필드가 나열됩니다.</p> </td> 
   <td> <p>예</p> <p>Kick-Starts를 사용하여 Workfront 데이터를 내보내면 하나의 내보내기에서 여러 개체 유형과 관련된 데이터를 내보낼 수 있습니다. 예를 들어 작업, 문제 및 프로젝트를 단일 내보내기에 포함할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 내보내기 제한

킥스타트를 통해 데이터를 내보낼 때에는 다음 제한 사항이 있습니다(데이터는 Excel 파일 형식으로 내보내짐).

* **50,000개 행:** 파일에서 허용되는 행 수입니다.
* **65,530개의 하이퍼링크:** 이는 65,530개 이상의 하이퍼링크가 포함된 문서에 대해 Excel에서 적용하는 제한입니다. 이러한 문서를 내보낸 후에는 열 수 없습니다. Excel 문서에는 200개의 데이터 행만 있을 수 있지만 문서 내에 65,530개가 넘는 링크가 있는 경우 문서가 열리지 않습니다.

## kick-starts를 통해 데이터 내보내기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **시스템** > **킥스타트,** 을 클릭한 다음 **데이터를 내보냅니다.**

1. 내보낼 객체를 선택합니다.
1. 클릭 **추가 옵션** 전체 객체 목록을 확인합니다.

   여기에 나열된 모든 개체를 사용하여 데이터를 Workfront으로 가져올 수도 있습니다.

   유일한 예외는 **액세스 수준** 개체. 내보내기에 포함된 액세스 레벨 데이터 시트는 참조용으로만 제공됩니다. 이를 통해 ID별로 새 사용자 계정에 액세스 수준을 지정할 수 있습니다.

   킥시작을 통해 Workfront으로 데이터를 가져오는 방법에 대한 자세한 내용은 [킥시작 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). 다음은 킥스타트를 통해 내보낼 수 있는 모든 개체 목록입니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>오브젝트</p> </th> 
      <th> <p>Excel 파일의 내보낸 시트</p> </th> 
      <th> <p>내보내기 형식</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">액세스 수준</td> 
      <td scope="col" valign="top">액세스 수준<br>기본 설정</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">할당</td> 
      <td scope="col" valign="top">배정<br>기본 설정</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">회사</td> 
      <td scope="col" valign="top"> 회사<br>기본 설정 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">이메일 템플릿</td> 
      <td scope="col" valign="top"> 이메일 템플릿<br>기본 설정 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">경비</td> 
      <td valign="top"> 비용<br>기본 설정 </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">외부 페이지</td> 
      <td valign="top"> 외부 페이지<br>기본 설정 </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">필터</td> 
      <td valign="top"> 필터<br>기본 설정 </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">그룹</td> 
      <td valign="top"> 그룹<br>기본 설정  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">그룹화</td> 
      <td valign="top"> 그룹화<br>기본 설정 </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">시간</td> 
      <td valign="top"> 시간<br>기본 설정 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">문제</td> 
      <td valign="top"> 문제<br>기본 설정 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">작업 역할</td> 
      <td valign="top"> 작업 역할<br>기본 설정 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">마일스톤 경로</td> 
      <td valign="top"> 이정표<br>이정표 경로<br>기본 설정 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">참고</td> 
      <td valign="top"> 참고<br>기본 설정 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">포트폴리오</td> 
      <td valign="top"> Portfolio<br>기본 설정  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">프로젝트</td> 
      <td valign="top"> 큐<br>프로젝트<br>라우팅 규칙<br>큐 항목<br>기본 설정 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">리소스 견적</td> 
      <td valign="top"> 리소스 예상<br>기본 설정 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">리소스 풀</td> 
      <td valign="top"> 리소스 풀<br>기본 설정 </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">위험</td> 
      <td valign="top"> 위험<br>기본 설정  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">위험 유형</td> 
      <td valign="top"> 위험 유형<br>기본 설정  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">스코어카드</td> 
      <td valign="top">스코어카드 질문<br>스코어카드 옵션<br>스코어카드<br>기본 설정 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">작업</td> 
      <td valign="top"> 작업<br>기본 설정 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">템플릿</td> 
      <td valign="top"> 큐<br>템플릿<br>라우팅 규칙<br>큐 항목<br>기본 설정 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">템플릿 할당</td> 
      <td valign="top"> 템플릿 지정<br>기본 설정 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">템플릿 작업</td> 
      <td valign="top"> 템플릿 작업<br>기본 설정 </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">타임시트</td> 
      <td valign="top"> 작업표 프로필<br>작업표<br>기본 설정 </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> 보기 </td> 
      <td valign="top"> 보기<br>기본 설정  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **다운로드.**

   내보낸 킥시작 파일은 Excel 파일 또는 로 컴퓨터에 다운로드됩니다. 여러 Excel 및 속성 파일이 포함된 zip 파일입니다. 각 Excel 파일은 시트 컬렉션입니다. 각 시트는 선택한 객체와 연관된 필드를 나타냅니다. 다음 항목이 있습니다 **속성** 모든 내보내기와 연관된 시트입니다.

   다음 **대시보드** 및 **보고서** 옵션을 사용하면 다운로드에 포함할 특정 대시보드 및 보고서를 선택할 수 있습니다. 시스템 전체에서 공유되는 대시보드만 내보낼 수 있습니다.

   매트릭스 보고서는 내보낼 수 없습니다. 매트릭스 보고서에 대한 자세한 내용은 [매트릭스 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   단일 내보내기에서 최대 100개의 대시보드 및 100개의 보고서를 선택할 수 있습니다.

   ![](assets/kickstart-export-350x381.png)

   여러 개체를 한 번에 내보낼 수 있습니다.

   기본적으로 다음 객체가 **포함할 내용** 레이블(누르기 전) **추가 옵션**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>오브젝트</strong> </p> </th> 
      <th> <p><strong>Excel 파일의 내보낸 시트</strong> </p> </th> 
      <th> <p> <strong>내보내기 형식</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>대시보드</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>매개 변수<br>매개 변수 옵션<br>매개 변수 그룹<br>카테고리 매개 변수<br>카테고리<br>보고서<br>포털 탭 섹션<br>대시보드<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>보고서</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">매개 변수<br>매개 변수 옵션<br>매개 변수 그룹<br>카테고리 매개 변수<br>카테고리<br>보고서<br>기본 설정</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>승인</p> </td> 
      <td scope="col" valign="top"> <p>단계 승인자<br>승인 단계<br>승인<br>승인 프로세스<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>사용자 정의 데이터</p> </td> 
      <td scope="col" valign="top"> <p>매개 변수<br>매개 변수 옵션<br>매개 변수 그룹<br>카테고리 매개 변수<br>카테고리<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>경비 유형</p> </td> 
      <td valign="top"> <p>비용 유형<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>시간 유형</p> </td> 
      <td valign="top"> <p>시간 유형<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>팀</p> </td> 
      <td valign="top"> 팀 구성원<br>팀<br>기본 설정 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>사용자</p> </td> 
      <td valign="top"> <p>사용자<br>기본 설정</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Excel 파일의 내보낸 시트</strong> </p> </th> 
      <th> <p> <strong>내보내기 형식</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>대시보드</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>매개 변수<br>매개 변수 옵션<br>매개 변수 그룹<br>카테고리 매개 변수<br>카테고리<br>보고서<br>포털 탭 섹션<br>대시보드<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>보고서</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">매개 변수<br>매개 변수 옵션<br>매개 변수 그룹<br>카테고리 매개 변수<br>카테고리<br>보고서<br>기본 설정</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>승인</p> </td> 
      <td scope="col" valign="top"> <p>단계 승인자<br>승인 단계<br>승인<br>승인 프로세스<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>사용자 정의 데이터</p> </td> 
      <td scope="col" valign="top"> <p>매개 변수<br>매개 변수 옵션<br>매개 변수 그룹<br>카테고리 매개 변수<br>카테고리<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>경비 유형</p> </td> 
      <td valign="top"> <p>비용 유형<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>시간 유형</p> </td> 
      <td valign="top"> <p>시간 유형<br>기본 설정</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>팀</p> </td> 
      <td valign="top"> 팀 구성원<br>팀<br>기본 설정 </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>사용자</p> </td> 
      <td valign="top"> <p>사용자<br>기본 설정</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (권장) 내보낸 데이터를 분석하여 표시되는 것으로 예상되는 모든 정보를 내보냈는지 확인합니다.

   대규모 내보내기의 경우 Workfront은 백그라운드에서 작동하여 Excel 파일을 만들고 지연에 대한 경고 메시지를 제공합니다. 다운로드가 완료되면 킥시작 파일이 이메일로 전송됩니다.

   ![](assets/large-kick-start-file-warning-350x65.png)
