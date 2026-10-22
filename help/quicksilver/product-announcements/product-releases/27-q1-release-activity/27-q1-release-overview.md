---
title: 2027년 1분기 릴리스 개요
description: 이 페이지에서는 2027년 1분기 릴리스에 포함된 기능에 대한 정보를 제공합니다. 이러한 개선 사항은 분기 내내 프로덕션 환경에서 사용할 수 있도록 계획되어 있습니다.
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4af92ba2774dc7fea7f91df14d8c3cdc8e865025
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 5%
---

# 2027년 1분기 릴리스 개요

이 페이지에서는 2027년 1월로 예정된 2027년 1분기 릴리스에 포함된 기능에 대한 정보를 제공합니다.

이 페이지의 개선 사항은 미리보기 환경에서 사용할 수 있습니다. 이 페이지는 2027년 1분기 릴리스가 계획 프로덕션 릴리스에 가까워짐에 따라 추가 개선 사항으로 업데이트됩니다.

>[!IMPORTANT]
>
>
>월별 및 분기별 릴리스는 달리 지정하지 않는 한 해당 월의 두 번째 전체 주 목요일에 사용할 수 있습니다.
>
>| 월별 릴리스 | 분기별 릴리스 |
>|----|----|
>| <ul><li>2026.11(2026년 11월 12일)</li><li>2026.12 (2026년 12월 17일)</li><li>2027.01 (2027년 1월 21일)</li></ul> | <ul><li>2027.01 (2027년 1월 21일)</li></ul> |
>
>빠른 릴리스 프로세스에 대한 자세한 내용은 [빠른 릴리스 프로세스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하십시오.

## Adobe Workfront 개선 사항

* [AI 개선 사항](#ai-enhancements)
* [프로젝트 개선 사항](#project-enhancements)

### AI 개선 사항

<table>
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
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-ai.md">Workfront MCP 서버 도구 세트</a></p>
                <p>이제 Workfront MCP 카탈로그를 특정 도구 세트로 제한하고 제품 권한별로 가용성을 필터링할 수 있으므로 AI 클라이언트는 필요한 기능만 액세스할 수 있습니다.</p>
            </td>
            <td><p>2026년 10월 21일</p></td>
            <td><p>2026년 11월 12일</p></td>
            <td><p>2027년 1월 21일</p></td>
        </tr>
    </tbody>
</table>

### 프로젝트 개선 사항

<table>
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
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">업데이트 상단에 스레드 고정</a></p>
                <p>이제 주요 정보가 팀에 계속 표시되도록 프로젝트, 작업, 문제 또는 요청의 업데이트 영역 상단에 가장 중요한 스레드를 고정할 수 있습니다.</p>
            </td>
            <td><p>2026년 10월 15일</p></td>
            <td><p>2026년 11월 12일</p></td>
            <td><p>2027년 1월 21일</p></td>
        </tr>
    </tbody>
</table>

## 기타 영역에 대한 릴리스 노트

* [Adobe Workfront Fusion 릴리스 활동](https://experienceleague.adobe.com/ko/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).
* [Adobe Workfront Planning 릴리스 활동](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

릴리스에는 현재 다음에 대한 업데이트가 없습니다.

* 시나리오 플래너
* 교정쇄
* 목표

## 공지

### 작업 역할 목록 보기의 레거시 청구 및 비용 요금 필드 사용 중단

시간이 지남에 따라, Dell은 비율 정보를 보다 완벽하고 확장 가능한 방식으로 유지 관리할 수 있는 향상된 비율 관리 기능과 전담 작업 역할 경험을 도입했습니다. 따라서 등급 관리는 목록 기반 관리 워크플로보다는 이러한 전용 경험으로 이동하고 있습니다.

2027년 1월 릴리스에서는 필터/보기/그룹화 구성(직접 참조 및 텍스트 모드 계산 열 모두)을 포함하여 레거시 필드 **시간당 청구** 및 **시간당 비용**&#x200B;을 Workfront API 또는 작업 역할 목록 보기에서 더 이상 사용할 수 없습니다.

보고서에서 대체물로 권장되는 텍스트 모드 코드를 사용할 수 있습니다(필요에 따라 `costRates` 또는 `billingRates` 사용).

    &quot;
    displayname=Test
    listdelimiter=&lt;br>
    listmethod=nested(costRates).lists
    type=iterate
    valueexpression=CONCAT({startDate},&quot; - &quot;,{endDate},&quot;: &quot;,{value})
    valueformat=HTML
    &quot;

작업 역할 비율을 관리하고 검토하려면 전용 비율 관리 환경을 사용하십시오.

* [작업 역할] > [비율] 페이지에서 직접 작업 역할 비율에 액세스하고 관리합니다.
* 비율 보고서를 사용하여 작업 역할 간의 비율 정보를 검토, 분석 및 보고합니다.

변경을 준비하는 데 필요한 작업은 없습니다. 그러나 현재 작업 역할 목록 보기에 **시간당 청구** 및 **시간당 비용** 필드를 표시하는 관리자는 위에서 설명한 권장 요금 관리 경험을 사용하도록 워크플로우를 업데이트해야 합니다.

작업 역할 비율에 대한 자세한 내용은 [작업 역할 만들기 및 관리](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

-->

### 교육 업데이트

각 Adobe Workfront 제품 릴리스의 학습 프로그램, 학습 경로, 비디오 및 안내서에 대한 최신 업데이트를 살펴보십시오. 자세한 내용은 [Workfront 자습서 페이지](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)의 &quot;새로운 기능&quot; 섹션을 참조하십시오.
