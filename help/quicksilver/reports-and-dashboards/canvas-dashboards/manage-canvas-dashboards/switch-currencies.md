---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 캔버스 대시보드의 통화 필드 사용
description: 캔버스 대시보드의 통화 필드를 사용할 수 있습니다.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---


# 캔버스 대시보드의 통화 필드 사용

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 이 단계에서 기능 일부가 완전하지 않거나 의도한 대로 작동하지 않을 수 있습니다. Canvas Dashboards Beta 개요 문서의 [피드백 제공](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) 섹션에 있는 지침에 따라 경험에 대한 피드백을 제출하십시오.<br>
>가능한 버그 또는 기술 문제에 대한 피드백이 있는 경우 Workfront 지원에 티켓을 제출하십시오. 자세한 내용은 [고객 지원 센터에 문의](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)<br>를 참조하세요.
>다음 클라우드 공급자에서는 이 Beta를 사용할 수 없습니다.
>
>* Amazon Web Services에 대한 자체 키 가져오기
>* Azure
>* Google Cloud 플랫폼

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>임의 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td> 
<p>표준</p> 
<p>플랜</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td><p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p>
   <p>재무 데이터에 대한 액세스 보기</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td><p>대시보드에 대한 권한 관리</p>
  </td> 
  </tr> 
</tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 전제 조건

1. 이 문서에 설명된 기능을 사용하려면 Workfront 인스턴스에 여러 통화 유형이 설정되어 있어야 합니다. 자세한 내용은 [환율 설정](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)을 참조하세요.

   >[!IMPORTANT]
   >
   >이 문서에 설명된 기능은 기본 통화 필드에만 적용됩니다. 사용자 정의 통화 필드에 대한 지원이 곧 제공됩니다.


## 캔버스 대시보드에 대한 기본 통화 설정

캔버스 대시보드를 만들 때 대시보드에 대한 기본 통화를 설정할 수 있습니다. 보고서 수준에서 통화 필드가 잠겨 있지 않은 경우 이 통화는 대시보드의 보고서에 모든 기본 통화 필드를 표시하는 데 사용됩니다.

1. 왼쪽 패널에서 **캔버스 대시보드**&#x200B;를 클릭합니다.

1. 오른쪽 상단 모서리에서 **새 대시보드**&#x200B;를 클릭합니다.

1. **대시보드 만들기** 상자에서

1. 다음을 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>이름</strong></td>
      <td><p>대시보드 이름을 입력합니다. 호환성 문제를 방지하려면 UTF-8 문자만 사용하는 것이 좋습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>설명 (선택 사항)</strong></td>
      <td>대시보드에 대한 설명을 입력합니다.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>통화</strong></td>
      <td>대시보드에 대한 기본 통화 유형을 선택합니다. <br>
      <br>대시보드를 필터링할 때 사용자가 다른 통화 유형을 전환할 수 있습니다.</td>
     </tr>
    </tbody>
   </table>


## 캔버스 대시보드에서 통화 간 전환

대시보드 수준에서 다른 통화 유형 간에 전환할 수 있습니다. 통화 필드가 포함된 보고서는 선택한 통화 유형을 반영하도록 업데이트됩니다.

통화 필드는 보고서 수준에서 잠길 수 있습니다. 통화 필드가 잠겨 있으면 대시보드의 통화 유형을 변경할 때 해당 보고서의 통화 유형이 변경되지 않습니다.

대시보드에 대한 통화 유형을 변경하려면

1. 대시보드 세부 정보 페이지의 오른쪽 위 모서리에 있는 통화 드롭다운 메뉴를 클릭합니다.
1. 목록에서 원하는 통화 유형을 선택합니다.

   ![통화 드롭다운 변경](assets/filter-by-currency.png)


## 제한 사항

다음 표에서는 [설정]의 [환율] 영역에 통화가 정의된 경우의 제한 사항에 대해 설명합니다.

<table> 
<tr>
<td></td>
<td>사용자는 다음을 수행할 수 있습니다.</td>
<td>사용자가 할 수 없음</td>
</tr>
<tr> 
<td>단일 통화가 정의됨</td>
<td>
<ul>
<li>캔버스 차트, KPI 및 테이블 보고서에서 기본 통화 필드 사용</li>
<li>캔버스 차트, KPI 및 차트 보고서에서 사용자 지정 통화 필드를 사용합니다.</li>
</ul>
</td>
<td>
<ul>
<li>대시보드에 기본 통화 할당(생성 시 또는 대시보드 편집 시)</li>
<li>대시보드 수준 통화 토글을 확인하고 사용하십시오.</li>
<li>캔버스 차트, KPI 또는 테이블 보고서에서 보기에 대한 특정 통화 잠금</li>
<li>캔버스 차트, KPI 및 테이블 보고서에서 Planning 통화 필드를 사용합니다.</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>여러 통화가 정의되었습니다.</td>
<td>
<ul>
  <li>캔버스 차트, KPI 및 테이블 보고서에서 기본 통화 필드 사용</li>
  <li>대시보드에 대한 기본 통화 설정(생성 시 또는 대시보드 편집 시)</li>
  <li>대시보드 수준 통화 토글을 확인하고 사용하십시오.</li>
  <li>대시보드 통화 전환 기본 설정을 무시하려면 캔버스 차트, KPI 또는 테이블 보고서에서 보기에 대한 특정 통화를 잠급니다.</li>
</ul>
</td>
<td><ul>
  <li>캔버스 차트, KPI 및 테이블 보고서에서 사용자 지정 데이터 통화 필드를 사용합니다.</li>
  <li>캔버스 차트, KPI 및 테이블 보고서에서 Planning 통화 필드를 사용합니다.</li>
</ul>
</td>
</tr></table>





