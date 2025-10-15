---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 캔버스 대시보드에서 보고서 필터 편집
description: 보고서 필터가 캔버스 대시보드에 적용된 후 편집할 수 있습니다.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 5205c342-7f63-438e-97c8-e74f7dfecfd0
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 9%

---

# 캔버스 대시보드에서 보고서 필터 편집

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 이 단계에서 기능 일부가 완전하지 않거나 의도한 대로 작동하지 않을 수 있습니다. Canvas Dashboards Beta 개요 문서의 [피드백 제공](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) 섹션에 있는 지침에 따라 경험에 대한 피드백을 제출하십시오.<br>
>&#x200B;>가능한 버그 또는 기술 문제에 대한 피드백이 있는 경우 Workfront 지원에 티켓을 제출하십시오. 자세한 내용은 [고객 지원 센터에 문의](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)<br>를 참조하세요.
>&#x200B;>다음 클라우드 공급자에서는 이 Beta를 사용할 수 없습니다.
>
>* Amazon Web Services에 대한 자체 키 가져오기
>* Azure
>* Google Cloud 플랫폼

보고서 필터를 캔버스 대시보드에 적용하면 프로젝트 진행 시 표시되는 데이터를 업데이트할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
  </td> 
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

보고서를 편집하려면 먼저 보고서에 필터를 추가해야 합니다.

## 보고서 필터 편집

>[!NOTE]
>
>보고서 필터를 작성하고 편집하는 데 사용할 수 있는 구성 도구가 많이 있습니다. 이러한 도구에 대한 자세한 내용은 이 문서에서 다음 섹션을 참조하십시오. [보고서 필터를 편집할 때 고려 사항](#considerations-when-editing-a-report-filter).


{{step1-to-dashboards}}

1. 왼쪽 패널에서 **캔버스 대시보드**&#x200B;를 클릭합니다.

1. **캔버스 대시보드** 페이지에서 편집할 필터가 포함된 보고서의 오른쪽 위 모서리에 있는 **자세히** ![자세히 아이콘](assets/more-icon.png) 아이콘을 클릭한 다음 **편집**&#x200B;을 선택합니다.

   ![보고서 편집](assets/edit-report-box.png)

1. **구성** 대화 상자의 왼쪽에서 **필터** 패널을 선택합니다.

1. **필터 편집**&#x200B;을 클릭합니다.

1. 편집할 필드 또는 수정자를 선택한 다음 필요에 따라 현재 선택 사항을 조정합니다.

   ![조건 추가](assets/add-condition.png)

1. (선택 사항) 다른 필터링 기준 집합을 추가하려면 **필터 그룹 추가**&#x200B;를 클릭합니다. 세트 사이의 기본 연산자는 AND입니다. 연산자를 클릭하여 OR로 변경합니다.

1. **저장**&#x200B;을 클릭합니다.

## 보고서 필터 편집 시 고려 사항

### 날짜 기반 와일드카드 필터 변수

날짜 기반 와일드카드 옵션은 모든 날짜 필터 속성과 함께 사용할 수 있습니다. 보고서에 날짜 기반 와일드카드를 추가하는 방법에 대한 자세한 내용은 문서 [날짜 기반 와일드카드를 사용하여 보고서 일반화](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)를 참조하십시오.

>[!NOTE]
>
>시간 부분을 포함하지 않거나 날짜 와일드카드 $$TODAY 또는 $$NOW를 사용하는 날짜 및 시간 계산을 만드는 경우, 시스템은 현지 시간대가 아닌 UTC(협정 세계시) 시간대에 따라 날짜를 사용합니다. 이로 인해 예상치 못한 날짜 결과가 발생할 수 있습니다.

다음 날짜 기반 와일드카드 중에서 선택할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>내일, 다음 주 또는 다음 달에 필터를 다시 빌드하지 않도록 이 와일드카드를 사용하여 날짜 구분 필터를 빌드하는 것이 좋습니다.</p> <p>예를 들어 오늘 전에 마감된 모든 작업을 표시하려는 경우 작업 필터에서 다음 규칙을 사용할 수 있습니다. <em>계획된 시작 일자가 $$TODAY보다 작음</em>.</p> <p>$$TODAY는 현재 날짜의 자정과 항상 같습니다.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>$$TODAY 와일드카드와 유사하지만 현재 날짜 및 시간을 포함합니다. $$NOW는 현재 날짜 및 시간과 같습니다.</p> <p>예를 들어 현재 시간까지 제공된 모든 시간 항목을 표시하려면 시간 필터에서 <em>계획된 시작 일자가 $$NOW</em>보다 작은 규칙을 사용하여 표시할 수 있습니다.</p> <p>참고: 이 와일드카드는 리소스 플래너에서 지원되지 않습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

다양한 기간 및 다양한 시점(미래 또는 과거)을 나타내기 위해 위의 와일드카드를 다음과 결합할 수 있습니다.

| 속성 |   |
|---|---|
| **q** | 달력 분기 |
| **시간** | 시간 |
| **d** | 일 |
| **너비** | 주 |
| **분** | 개월 |
| **y** | 년 |

{style="table-layout:auto"}

| **한정자** | |
|---|---|
| **b** | 기간의 시작(지정된 속성이 없음)은 기본적으로 주의 시작(일요일)으로 설정됩니다. |
| **e** | 기간의 종료(지정된 속성이 없으면 기본값: 주의 종료: 토요일) |

{style="table-layout:auto"}

| **연산자** | |
|---|---|
| **+** | 와일드카드 값에 값 추가 |
| **-** | 와일드카드 값에서 값 빼기 |

{style="table-layout:auto"}

예를 들어 와일드카드 `$$TODAYb+2w`은(는) &quot;이번 주 초부터 2주&quot;를 참조합니다. 와일드카드 *`$$NOW+2h`은(는) &quot;지금부터 2시간 후&quot;를 참조합니다.

### 로그인한 사용자 와일드카드 필터 변수

* 사용자 `name` 특성을 필터링하면 **내(로그인한 사용자)** 옵션이 표시됩니다.

  ![사용자 이름 특성](assets/user-name-attribute.png)

* `name` 그룹 특성을 필터링하면 필터 조건에 사용할 **내 홈 그룹(로그인한 사용자 그룹)** 및 **내 다른 그룹(로그인한 사용자 그룹)** 옵션이 표시됩니다.

  ![그룹 이름 특성](assets/group-name-attribute.png)

* `name` 팀 특성을 필터링하면 필터 조건에서 선택할 **내 기본 팀(로그인한 사용자 팀)** 및 **내 다른 팀(로그인한 사용자 팀)** 옵션이 표시됩니다.

  ![팀 이름 특성](assets/team-name-attribute.png)


### 자식 개체 참조

추가 열, 필터 옵션 및 그룹화 속성에 대해 사용할 수 있는 관계는 일반적으로 Workfront 개체 계층 구조의 상위 개체로 제한되거나 보고서의 기본 엔티티 개체를 한 번만 선택합니다. 여기에는 다음과 같은 몇 가지 예외가 있습니다.

* 프로젝트 > 작업
* 문서 승인 > 문서 승인 단계
* 문서 승인 단계 > 문서 승인 단계 참가자

위에 나열된 상위-하위 관계를 활용하는 경우 상위 객체에 연결된 각 하위 레코드에 대한 행이 테이블에 표시됩니다.

### 필드 유형별 필드 연산자

+++ 를 확장하여 필드 유형별 필드 연산자 목록을 봅니다. 

<table>
    <tr>
        <td><b>필드 유형</b></td>
        <td><b>예</b></td>
       <td><b>연산자</b></td>
        <td><b>와일드카드</b></td>
    </tr>
    <tr>
        <td>개체/참조 이름</td>
        <td>모든 네이티브 이름 특성 또는 사용자 지정 조회</td>
              <td><ul>
        <li>Equal</li>
        <li>같지 않음</li>
        <li>다음 포함</li>
          <li>다음을 포함하지 않음</li>
            <li>Null임</li>
              <li>Null이 아님</li>
        </ul></td>
        <td>사용자: 이름
        <ul>
        <li>나(로그인한 사용자)</li>
        </ul>
        그룹: 이름
        <ul>
          <li>내 홈 그룹(로그인한 사용자 그룹)</li>
            <li>내 다른 그룹(로그인한 사용자 그룹)</li>
          </ul>
          팀: 이름
                  <ul>
          <li>내 기본 팀(로그인한 사용자 팀)</li>
            <li>내 다른 팀(로그인한 사용자 팀)</li>
          </ul>
        </td>
    </tr>
    <tr>
        <td>문자열/텍스트 입력 </td>
                <td>프로젝트: 설명</td>
                      <td><ul>
             <li>Equal</li>
        <li>같지 않음</li>
        <li>다음 포함</li>
          <li>다음을 포함하지 않음</li>
            <li>Null임</li>
              <li>Null이 아님</li>
        </ul></td>
        <td></td>
    </tr>
    <tr>
        <td>정수 / 더블</td>
             <td>프로젝트: 계획된 시간
        <br>작업: 완료율</td>
              <td><ul>
        <li>Equal</li>
        <li>같지 않음</li>
        <li>보다 큼</li>
          <li>크거나 같음</li>
          <li>보다 작음</li>
          <li>작거나 같음</li>
            <li>Null임</li>
              <li>Null이 아님</li>
        </ul></td>
        <td></td>
    </tr>
       <tr>
        <td> 날짜 / 날짜 시간 </td>
                    <td>프로젝트: 계획된 시작 일자
        <br>시간: 시작 날짜</td>
              <td><ul>
        <li>Equal</li>
        <li>같지 않음</li>
        </ul></td>
        <td><b>상대적 날짜 설정</b> 옵션을 전환하여 상대적 날짜 와일드카드를 적용하여 보고서를 보다 동적이고 일반적인 날짜 기간에 따라 자동으로 조정할 수 있습니다. 
         <ul><li>$$오늘</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>부울 </td>
                  <td>프로젝트: 문서 있음
        <br>작업: 중요
        <br> 사용자: 활성 상태입니다.</td>
        <td><ul>
        <li>Equal</li>
        <li>같지 않음</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++
