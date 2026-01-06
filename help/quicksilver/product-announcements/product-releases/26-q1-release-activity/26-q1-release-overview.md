---
title: 2026년 1분기 릴리스 개요
description: 이 페이지에서는 2026년 1분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b9016bc9a5609424b6cd6cdec67ac4d696e7ab45
workflow-type: tm+mt
source-wordcount: '2880'
ht-degree: 4%

---

# 2026년 1분기 릴리스 개요

이 페이지에서는 2026년 1월로 예정된 2026년 1분기 릴리스에 포함된 기능에 대한 정보를 제공합니다.

이 페이지의 개선 사항은 미리보기 환경에서 사용할 수 있습니다. 이 페이지는 2026년 1분기 릴리스가 계획 프로덕션 릴리스에 가까워짐에 따라 추가 개선 사항으로 업데이트됩니다.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>월별 및 분기별 릴리스는 달리 지정하지 않는 한 해당 월의 두 번째 전체 주 목요일에 사용할 수 있습니다.
>
>| 월별 릴리스 | 분기별 릴리스 |
>|----|----|
>| <ul><li>25.11 (2025년 11월 13일)</li><li>25.12 (2025년 12월 11일)</li><li>26.1 (2026년 1월 14일)</li></ul> | <ul><li>26.1 (2026년 1월 15일)</li></ul> |
>
>각 분기의 최종 릴리스(이번 분기 26.1)의 경우 빠른 릴리스 일정을 사용 중인 사용자는 하루 전(2026년 1월 14일)에 릴리스를 받게 됩니다.
>
>빠른 릴리스 프로세스에 대한 자세한 내용은 [빠른 릴리스 프로세스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하십시오.

## Adobe Workfront 개선 사항

* [관리자 개선 사항](#administrator-enhancements)
* [문서 및 승인 개선 사항](#documents-and-approvals-enhancements)
* [홈 개선 사항](#home-enhancements)
* [통합 개선 사항](#integration-enhancements)
* [프로젝트 개선 사항](#project-enhancements)
* [보고 개선 사항](#reporting-enhancements)
* [요청 개선 사항](#requests-enhancements)
* [기타 개선 사항](#other-enhancements)

### 관리자 개선 사항

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">레이아웃 템플릿의 우선 순위 관리</a>
            <p>이제 레이아웃 템플릿에서 특정 사용자에 대한 우선 순위를 활성화하거나 비활성화할 수 있습니다. 이전에 조직에 대해 [우선 순위]를 비활성화한 경우, 이 변경 사항으로 레이아웃 템플릿에서 비활성화된 상태로 유지됩니다.</p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2025년 1월 14일 수요일</td>
        <td>2025년 1월 15일 목요일</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">계산된 사용자 지정 필드에 대한 다중 양식 충돌 확인</a>
            <p>사용자 정의 필드에서 표현식을 편집할 때 영향을 받을 수 있는 오브젝트를 표시하기 위해 충돌을 확인하는 옵션을 추가했습니다. 이 대화 상자는 공식 변경의 영향을 받을 수 있는 모든 객체를 객체 유형별로 그룹화하여 표시합니다. 각 객체의 세부 정보로 이동하고 필드를 검토하여 양식에서 필드를 제거할지 또는 표현식을 변경하지 않고 유지할지 여부를 결정할 수 있습니다.</p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2025년 1월 14일 수요일</td>
        <td>2025년 1월 15일 목요일</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">사용자 지정 개체에 저장된 시작 날짜 및 입력한 ID</a><p>[!BADGE 해제 일정]{type=Neutral}</p>
            <p>이제 시작 날짜 및 ID로 입력된 날짜가 사용자 정의 양식, 필드 및 섹션에 저장됩니다. 보고서에서 이러한 데이터 옵션을 필터, 보기 또는 그룹화로 사용할 수 있습니다. 설정의 사용자 정의 양식, 필드 또는 섹션 목록에 표시하려면 새 뷰 또는 기존 뷰에 입력 일자 및 입력자: 이름을 열로 추가합니다.</p>
        </td>
        <td>2025년 11월 13일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">레이아웃 템플릿을 편집할 때 단추 이름을 업데이트합니다</a>
            <p>사용자 정의 양식 디자이너와 같은 다른 설정 영역과 일관성을 유지하기 위해 레이아웃 템플릿을 편집할 때 표시되는 단추가 적용, 저장 및 닫기 및 취소로 변경되었습니다. 새 옵션인 적용을 사용하면 변경 사항을 레이아웃 템플릿에 저장하고 편집을 계속할 수 있습니다. 이전에는 저장 및 취소 옵션을 사용할 수 있었습니다. </p>
        </td>
        <td>2025년 10월 30일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> 사용자 지정 필드의 활성 플래그를 사용하여 필드 관리를 개선했습니다</a>
            <p>시스템에 사용자 정의 필드가 많을 경우 사용자 정의 양식 및 보고서에서 해당 필드를 관리하기가 어려울 수 있습니다. 이제 사용자 지정 필드를 새 <b>활성</b> 플래그로 비활성 상태로 표시할 수 있습니다. 이 플래그는 사용자 정의 양식의 필드로 작업하거나 필드 목록에서 필드를 추가 또는 편집할 때 사용할 수 있습니다. </p>
        </td>
        <td>2025년 10월 30일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>   
  </tbody>
</table>

### 문서 및 승인 개선 사항

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Express에서 리뷰를 보낼 때 Workfront 프로젝트 선택<p>[!BADGE 해제 일정]{type=Neutral}</p> </a>
            <p>증명을 보낼 Workfront 프로젝트를 선택할 수 있습니다. 이렇게 하면 모든 관련 에셋과 증명이 동일한 프로젝트 내에 체계적으로 정리될 수 있습니다.</p>
        </td>
        <td>2025년 12월 15일 화요일</td>
        <td>2025년 12월 15일 화요일</td>
        <td>2025년 12월 15일 화요일</td>
    </tr> 
     <tr>
        <td>
            Workfront 교정을 통해 Adobe Express에 대한 <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">조직 간 지원<p>[!BADGE 해제 일정]{type=Neutral}</p> </a>
            <p>Workfront Proofing과 함께 Adobe Express에 대한 교차 조직 지원을 소개합니다. 이 향상된 기능을 통해 여러 IMS 조직에서 작업하는 고객은 증명 워크플로를 원활하게 사용하고 관리할 수 있습니다.</p>
        </td>
        <td>2025년 11월 13일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
    </tr>   
     <tr>
        <td>
            이제 Frame.io 통합에서 <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager을 사용할 수 있습니다. <p>[!BADGE 해제 일정]{type=Neutral}</p> </a>
            <p>이제 Experience Manager Assets을 사용하여 검토 및 승인 주기​을 거친 디지털 에셋을 관리하고 저장할 수 있습니다. 이 통합을 통해 Adobe Experience Manager, Frame.io 및 Workfront의 기능을 활용하여 컨텐츠 관리 및 공동 작업 프로세스를 간소화할 수 있습니다. </p>
        </td>
        <td>2025년 10월 30일 금요일</td>
        <td>2025년 10월 30일 금요일</td>
        <td>2025년 10월 30일 금요일</td>
    </tr>   
  </tbody>
</table>



### 홈 개선 사항

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">홈에서 언급 위젯 업데이트</a>
            <p>홈의 언급 위젯에 대한 다음과 같은 사항이 개선되었습니다. <ul><li>이제 홈 의 언급 위젯에서도 대부분의 Workfront 오브젝트의 업데이트 영역에서 동일한 경험을 사용할 수 있습니다. </li><li>이제 언급 위젯에 지난 2주 동안 사용자가 작성하거나 태그 지정한 주석이 포함됩니다</li><ul></p>
        </td>
        <td>2025년 12월 17일 목요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>   
  </tbody>
</table>

### 통합 개선 사항

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Creative Cloud Express에서 리뷰를 보낼 때 Workfront 프로젝트 선택</a><p>[!BADGE 해제 일정]{type=Neutral}</p>
            <p>증명을 보낼 Workfront 프로젝트를 선택할 수 있습니다. 이렇게 하면 모든 관련 에셋과 증명이 동일한 프로젝트 내에 체계적으로 정리될 수 있습니다. </p>
        </td>
        <td>2025년 12월 15일 화요일</td>
        <td>2025년 12월 15일 화요일</td>
        <td>2025년 12월 15일 화요일</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Experience Manager Assets 기본 통합을 위한 Adobe Workfront의 자산 선택기 </a>을(를) 업데이트했습니다.
            <p>Experience Manager Assets용 Adobe Workfront 통합에서 에셋 선택기를 업그레이드했습니다. 이제 이 업그레이드를 사용하여 AEM 컬렉션을 선택하고 Workfront으로 직접 가져올 수 있습니다. </p>
        </td>
        <td>2025년 11월 20일 금요일</td>
        <td>2025년 12월 11일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>   
    <!-- <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">New version of Salesforce integration now available </a>
            <p>To stay up-to-date with recent changes to the Workfront API, we've created a new Salesforce integration. The new integration features the same functionality as the previous version, and was updated to avoid losing functionality deprecated in the API.</p><p>NOTE: The Workfront for Salesforce integration, including the new version, will not be available after **February 28, 2026**. </p>
        </td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
    </tr>   -->
  </tbody>
</table>

### 프로젝트 개선 사항

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">일반 사용자가 프로젝트에 시간을 기록할 수 있음</a>
            <p>이제 일반 사용자가 프로젝트에 직접 시간을 기록할 수 있습니다. 이전에는 표준 라이선스 사용자만 프로젝트에 시간을 기록할 수 있었습니다.</p>
        </td>
        <td>2025년 12월 11일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>   
  </tbody>
</table>

### 보고 개선 사항

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">캔버스 대시보드의 통화 업데이트</a>
            <p>통화 필드에 대해 다음과 같이 업데이트되었습니다.<ul><li>Workfront에 여러 통화가 정의된 경우 이제 생성 중에 대시보드에 대한 기본 통화를 선택할 수 있습니다. </li><li>보고서를 만들 때 통화 필드를 잠글 수 있습니다. 이렇게 하면 대시보드 수준의 통화 기본 설정이 이러한 값 표시에 영향을 주지 않습니다.</li><li>대시보드를 볼 때 사용자는 Workfront에서 정의된 통화 간에 전환할 수 있습니다. 이러한 변경 사항은 잠긴 통화 필드를 제외하고 전체 대시보드에 적용됩니다</li></ul></p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>
 <tr>
        <td>
            캔버스 대시보드의 빠른 검색 테이블 결과 <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">개</a>
            <p>표 보고서에 빠른 검색을 추가했습니다. 이 검색은 모든 페이지에서 작동하므로 현재 표시되지 않는 데이터도 찾을 수 있습니다.</p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">원형 차트에 대한 새 전체 표시 옵션</a>
            <p>파이 차트를 도넛 차트로 변환하는 새로운 합계 표시 옵션을 도입했습니다. 이 기능을 사용하면 차트에 있는 모든 세그먼트의 합계를 나타내는 중앙 값을 표시할 수 있습니다.</p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">캔버스 대시보드의 파이 차트에 대한 새 구성 옵션</a>
            <p>파이 차트에 대한 두 가지 새로운 구성 옵션이 도입되었습니다. <ul><li>세그먼트 레이블 숨기기: 이제 세그먼트 레이블이 너무 길고 차트 가독성에 영향을 주는 경우 원형 차트에서 숨기도록 선택할 수 있습니다.</li><li>차트 범례 숨기기 및 위치 변경: 이제 원형 차트 범례를 숨기도록 선택할 수 있습니다. 범례의 위치를 차트의 오른쪽(기본값), 왼쪽, 위쪽 또는 아래쪽으로 설정할 수도 있습니다. </li></ul></p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">캔버스 대시보드 그룹화 수 개선</a>
            <p>현재 페이지의 레코드 수와 모든 페이지의 그룹화에 대한 전체 레코드 수를 표시하도록 캔버스 대시보드의 그룹화 막대를 업데이트했습니다. </p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">캔버스 대시보드의 보고서에 새로운 참조 줄 기능</a>
            <p>이제 막대, 열 및 선 차트에서 참조 라인을 정의하여 시리즈 기반 보고서의 대상 또는 임계값을 설정할 수 있습니다. </p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">캔버스 대시보드의 차트 보고서에서 축 레이블 사용자 지정</a>
            <p>이제 차트 보고서에서 축 레이블을 사용자 지정할 수 있습니다. 이 새 기능을 사용하면 기본 개체 및 필드 경로 대신 표시할 대체 축 레이블을 입력할 수 있습니다. 또한 축 레이블을 완전히 숨기도록 선택할 수 있습니다.</p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">캔버스 대시보드에 보고서 복제</a><p>[!BADGE 해제 일정]{type=Neutral}</p>
            <p>이제 KPI, 테이블 또는 차트 보고서를 만든 후 캔버스 대시보드에서 복제할 수 있습니다. 복제되면 저장하기 전에 필요에 따라 보고서를 편집할 수 있습니다.</p>
        </td>
        <td>2025년 10월 23일 금요일</td>
        <td>2025년 10월 23일 금요일</td>
        <td>2025년 10월 23일 금요일</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">보고서 필터에서 필드 옵션 제거</a>
            <p>보고서에 필터를 적용할 때 이전에 사용할 수 있었던 다음 필드 옵션을 제거했습니다.
            <ul>
            <li>기타 그룹 ID</li>
            <li>기타 역할 ID</li>
            <li>기타 팀 ID</li>
            </ul>
            </p>
        </td>
        <td>2025년 11월 6일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>    
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">캔버스 대시보드의 로드 시간을 개선하는 새 보호 기능</a>
            <p>Canvas Dashboards에서 로드 시간 지연을 방지하고 전체 성능을 개선하기 위해 대시보드에 추가할 수 있는 대시보드 구성 요소의 수에 대한 제한을 적용했습니다.
            <ul>
            <li>대시보드당 보고서: 25 제한</li>
            <li>테이블 보기의 그룹화: 5개 제한</li>
            <li>보고서의 기본 개체로부터의 거리: 10 제한</li>
            <li>테이블 보기의 열: 25개 제한</li>
            <li>대시보드 수준 필터 프롬프트: 10개 제한</li>
            </ul></p>
        </td>
       <td>2025년 11월 6일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>   
  </tbody>
</table>

### 요청 개선 사항

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">만들어진 개체 링크를 요청 영역 및 내 요청 위젯에서 사용할 수 있습니다</a>
            <p>특정 요청으로 만든 개체로 더 쉽게 이동할 수 있도록 만들어진 개체 열에 링크를 추가했습니다. 이제 이 열의 링크를 클릭하여 생성된 객체의 페이지로 바로 이동할 수 있습니다./p&gt;
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr> 
    <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr> -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">요청 목록 및 내 요청 위젯에 사용자 정의 필드 추가</a>
            <p>필요한 정보를 더 쉽게 볼 수 있도록 사용자 정의 필드를 요청 목록 및 홈 의 내 요청 위젯에 열로 추가하는 기능을 추가했습니다. 이제 사용자 정의 양식의 필드를 열로 추가할 수 있으며 해당 필드에 정보가 있는 요청은 목록 또는 위젯에 해당 정보를 표시합니다.</p><p>이 기능은 새 요청 환경에서만 사용할 수 있습니다.</p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">현재 사용자 와일드카드를 요청 필터에서 사용할 수 있음</a>
            <p>사용자에게 적용되는 요청을 더 쉽게 필터링할 수 있도록 현재 사용자 와일드카드를 만들었습니다. 이제 필터링할 때 "나(로그인한 사용자)"를 선택할 수 있습니다. 그런 다음 필터는 요청 목록을 보고 있는 사용자에게 적용됩니다.   </p>
        </td>
        <td>2025년 12월 18일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">AI에서 제공하는 양식 채우기를 이제 요청에 사용할 수 있음</a>
            <p>요청을 더 쉽게 만들 수 있도록 AI에서 제공하는 양식 채우기를 만들었습니다. 이제 프롬프트에 붙여넣거나 요청 양식에 문서를 업로드할 수 있으며 AI가 관련 정보를 꺼내 양식을 채웁니다.  </p>
        </td>
        <td>2025년 12월 11일 금요일</td>
        <td>2025년 12월 11일 금요일</td>
        <td>2025년 12월 11일 금요일</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">요청 영역 및 내 요청 위젯에서 보기 공유</a>
            <p>필요한 정보를 더 쉽게 볼 수 있도록 새 보고 환경에 보기를 공유하는 기능을 추가했습니다. 이제 다른 사용자, 팀 또는 그룹과 보기를 공유할 수 있습니다. </p>
        </td>
        <td>2025년 12월 4일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">새 요청 경험에 요청 초안 저장</a>
            <p>요청을 더 쉽게 만들고 제출할 수 있도록 새 요청 환경에 초안을 저장하는 기능을 추가했습니다. 이제 요청을 작성하고 닫으면 요청이 초안 상태로 저장되고 초안을 작성하는 데 사용되는 요청 양식에서 찾을 수 있습니다. 그런 다음 편리한 시간에 초안을 다시 열고, 업데이트하고, 제출할 수 있습니다. </p>
        </td>
        <td>2025년 11월 20일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">새 요청 경험에서 제출된 요청 삭제</a>
            <p>요청을 더 쉽게 정리하고 복잡하지 않게 유지하기 위해 요청을 삭제하는 기능을 새 요청 환경에 추가했습니다. 이제 제출한 요청을 삭제할 수 있습니다. Workfront 관리자 및 Workfront Planning Workspace 관리자도 요청을 삭제할 수 있습니다.</p>
        </td>
        <td>2025년 11월 20일 금요일</td>
        <td>2026년 1월 14일 목요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">새 요청 환경에서 이전에 제출된 요청을 복사하여 새 요청을 만듭니다</a>
            <p>요청을 더 쉽게 제출할 수 있도록 요청을 새 요청 경험에 복사하는 기능을 추가했습니다. 이제 요청을 복사하고 필드를 편집한 후 새 요청으로 제출할 수 있습니다. </p>
        </td>
        <td>2025년 11월 20일 금요일</td>
        <td>2025년 12월 11일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
    </tr>    
  </tbody>
</table>

### 기타 개선 사항

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>기능</strong>
        </td>
        <td><strong>미리보기</strong></td>
        <td><strong>빠른 릴리스</strong></td>
        <td><strong>분기별</strong></td>
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">2026년 1분기 릴리스 일정 동안의 룩앤필 업데이트</a>
                        <p>2026년 1분기 릴리스 기간 내에 Adobe Workfront 애플리케이션의 다양한 영역의 모양과 느낌에 대한 작은 업데이트가 이루어지고 있습니다. </p>
                    </td>
                    <td><p>2026년 1분기 릴리스 일정 내내<br /></p>
                    <td colspan="2"><p>빠른 릴리스: 미리 보기로 릴리스한 후 최소 1주(달리 지정되지 않은 경우)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                다중 선택 필드에 대한 <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}"> 선택 제한</a>
              <p>확인란 및 다중 선택 드롭다운과 같이 여러 항목을 선택할 수 있는 필드는 이제 사용자가 양식을 채울 때 5000개까지 선택할 수 있습니다.</p>
             </td>
        <td>2025년 10월 30일 금요일</td>
        <td>2025년 11월 13일 금요일</td>
        <td>2026년 1월 15일 금요일</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">이제 더 많은 Workfront 조직에서 Adobe 통합 환경을 사용할 수 있습니다</a><p></p>
            <p>조직이 Adobe 통합 경험의 이점을 이용할 수 있도록 하기 위해 기존 Workfront 고객이 이를 사용할 수 있도록 계속 노력하고 있습니다.</p>
        </td>
        <td><p>2025년 12월 11일 금요일</p></td>
        <td><p>2026년 1월 15일 금요일</p></td>
        <td><p>2026년 1월 15일 금요일</p></td>
    <tr>
            </tbody>
        </table>


### Workfront에서 곧 제거될 기능

#### 25.11 릴리스에서 작업 역할의 재정의 통화 사용 중단

재무 모델 단순화의 일부로, 10월 30일 미리보기 및 25.11 릴리스를 사용하는 모든 고객을 위한 프로덕션에서 작업 역할의 통화 재정의를 더 이상 사용하지 않을 예정입니다. 이 변경 사항은 [설정] 영역의 작업 역할에서 통화 및 요금이 구성되는 방식에 영향을 줍니다.

* 작업 역할의 **통화 재정의** 필드를 더 이상 사용할 수 없습니다.
* 각 작업 역할에는 관련 비용 및 청구 요금이 포함된 단일 통화가 있습니다.
* 기존의 모든 대체 통화 및 해당 환율 값은 자동으로 이전되어 해당 작업 역할의 유일한 통화 및 환율이 됩니다.

## 인터페이스 현대화

사용자 경험을 개선하고 다른 Adobe 애플리케이션과 통합하기 위해 Adobe Workfront 전체에서 인터페이스를 업데이트할 예정입니다. 이러한 변경 사항은 표준 릴리스 일정 외에 릴리스됩니다. 이러한 변경 사항 목록은 [인터페이스 현대화](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)를 참조하십시오.

## 기타 영역에 대한 릴리스 노트

### Workfront Fusion 개선 사항

Workfront Fusion의 새로운 기능은 표준 릴리스 일정이 아닌 케이던스로 프로덕션에서 사용할 수 있습니다. 최신 기능에 대한 자세한 내용은 [Adobe Workfront Fusion 릴리스 활동](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)을 참조하십시오.

### Workfront Planning 개선 사항

Workfront Planning의 새로운 기능은 프로덕션에서 사용할 수 있습니다. 최신 기능에 대한 자세한 내용은 [Adobe Workfront Planning의 2026년 1분기 릴리스 활동](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md)을 참조하십시오.

릴리스에는 현재 다음에 대한 업데이트가 없습니다.

* 시나리오 플래너
* 교정쇄
* 목표

## 데스크톱 증명 뷰어 업데이트

### 버전 2.1.54

**모든 고객을 위한 프로덕션 릴리스: 2025년 12월 11일**

Desktop Proofing Viewer가 2.1.52에서 2.1.54로 업데이트되었습니다. 이 업데이트에는 내부 도구 업데이트가 포함되었으며 최종 사용자 기능에는 영향을 주지 않았습니다.

2.1.53 버전에는 내부 공구 설비 변경 사항도 포함되어 있습니다.

이 업데이트는 Mac 및 Windows 모두에 해당됩니다.

### 버전 2.1.52

**모든 고객을 위한 프로덕션 릴리스: 2025년 7월 31일**

Desktop Proofing Viewer가 버전 2.1.52로 업데이트되어 버그 수정 사항을 해결합니다.

2.1.51 업데이트에는 내부 도구 업데이트가 포함되었으며 최종 사용자 기능에는 영향을 주지 않았습니다.

이 업데이트는 Mac 및 Windows 모두에 해당됩니다.

## 공지

### API 버전 21

Workfront API 버전 21은 2025년 10월 23일에 릴리스되었습니다. API 버전 21의 경우 일부 리소스 및 끝점을 수정했습니다. 일부 변경 사항은 새로운 기능을 지원하며, 다른 변경 사항을 통해 API를 통해 사용 가능한 정보를 보다 쉽게 사용할 수 있습니다.

>[!IMPORTANT]
>
>이 API 버전 변경은 기존 API 호출에 영향을 줄 수 있는 획기적인 변경 기능을 제공합니다. 이는 API 버전 21이 이벤트 구독 버전 2를 사용한다는 사실에 기인합니다.
>
> 다중 선택 필드의 경우, 이벤트 구독 버전 2는 항상 배열로 전송합니다. 두 개 이상의 값을 선택한 경우 버전 1에서 배열을 전송했습니다. 값을 하나만 선택한 경우 문자열을 보냈습니다.

새로운 기능 및 업데이트 내용은 [API 버전 21의 새로운 기능](/help/quicksilver/wf-api/api/new-api-version-21.md)을 참조하세요.

API 버전에 대한 자세한 내용은 [API 버전 관리 및 지원 일정](/help/quicksilver/wf-api/api/api-version-support-schedule.md)을 참조하십시오.

### Microsoft Teams용 Workfront의 새 버전

[Microsoft이 새 팀 클라이언트로 전환](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)됨에 따라 클래식 팀 클라이언트는 2025년 7월 1일 이후에 더 이상 사용할 수 없습니다. Workfront과 같은 Microsoft Teams 및 통합 앱을 계속 사용하려면 이 날짜 이전에 고객이 New Teams 클라이언트로 전환해야 합니다.

이제 업데이트된 Workfront 통합을 사용할 수 있으며 새 팀 경험과 완전히 호환됩니다. 대부분의 경우 사용자가 전환되면 Workfront이 자동으로 표시됩니다. 그렇지 않은 경우 Microsoft Teams App Store에서 수동으로 통합을 설치할 수 있습니다. 새 Teams 클라이언트에서 Workfront 통합을 설치하거나 확인하려면 [Microsoft Teams용 설치 [!DNL Adobe Workfront] 를 참조하십시오](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Microsoft Outlook용 Workfront

[Microsoft에서 기존 Exchange 온라인 토큰에 대한 지원을 사용하지 않도록 설정하는 중입니다](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens). 이 토큰은 현재 인증을 위해 Workfront Outlook 추가 기능에서 사용됩니다. Microsoft의 이러한 변경 사항은 이미 고객에게 영향을 주기 시작했으며 2025년 10월까지 단계적으로 계속 적용될 예정입니다.

* **Microsoft에서 이 토큰을 완전히 비활성화하면 Microsoft Outlook용 Workfront 통합이 더 이상 작동하지 않습니다.**

이 변경의 일부로 Microsoft은 토큰이 다시 활성화되는 방식을 변경하기로 결정했습니다. **2025년 6월 30일** 이후에는 관리자가 더 이상 토큰을 직접 다시 활성화할 수 없습니다. Microsoft 지원에서만 예외를 허용할 수 있습니다. **2025년 10월 1일부터 모든 테넌트에 대해 레거시 토큰이 꺼집니다. 예외가 부여되지 않습니다.**

### 기타 Workfront 통합 전환

보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 **2026년 2월 28일** 이후에는 다음 통합을 사용할 수 없습니다.

* G Suite용 Workfront
* Jira용 Workfront
* Salesforce용 Workfront

조직의 Google Workspace 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.


### Workfront 유지 관리 업데이트

2025년 1분기 릴리스 동안 이루어진 유지 관리 업데이트에 대한 자세한 내용은 [Workfront 유지 관리 업데이트](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ko)를 참조하십시오.

### 교육 업데이트

각 Adobe Workfront 제품 릴리스의 학습 프로그램, 학습 경로, 비디오 및 안내서에 대한 최신 업데이트를 살펴보십시오. 자세한 내용은 [Workfront 자습서 페이지](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ko)의 &quot;새로운 기능&quot; 섹션을 참조하십시오.
