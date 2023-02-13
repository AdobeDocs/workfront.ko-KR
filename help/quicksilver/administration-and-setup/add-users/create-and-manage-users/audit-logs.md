---
title: 감사 로그
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자는 감사 로그를 사용하여 지난 90일 동안 시스템에서 트리거된 사용자 변경 사항을 추적할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 4%

---

# 감사 로그

Adobe Workfront 관리자는 아래에 설명된 감사 로그를 사용하여 지난 90일 동안 시스템에서 트리거된 사용자 변경 사항을 추적할 수 있습니다.

이러한 감사 로그에 표시할 내용을 보고 필터링하는 방법에 대한 지침은 [감사 로그 보기 및 내보내기](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## 감사 로그에서 찾을 수 있는 정보

모든 감사 로그 항목에 다음 필드가 기록됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">날짜 및 시간</td> 
   <td>작업이 발생한 시기.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">로그 유형</td> 
   <td>액세스 수준 또는 사용자 지정 양식과 같은 감사 로그 유형입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 이름</td> 
   <td> <p>작업을 수행한 사용자의 이름입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개 액션</td> 
   <td> 변경, 만들기 및 삭제와 같은 사용자가 수행한 작업입니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">오브젝트</td> 
   <td> 작업의 결과로 영향을 받는 객체의 이름입니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">세부 정보</td> 
   <td>작업에 대한 추가 세부 사항입니다. 전체 메시지를 읽으려면 텍스트 위로 마우스를 가져갑니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP 주소</td> 
   <td> <p>작업 시 작업을 수행한 사용자의 IP 주소입니다.</p> <p>일부 시스템 작업에는 IP 주소를 사용할 수 없습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 감사 로그 유형 및 이를 트리거하는 작업

* [액세스 수준](#access-level)
* [회사](#company)
* [상황](#condition)
* [사용자 정의 필드](#custom-field)
* [사용자 정의 양식](#custom-forms)
* [사용자 정의 섹션](#custom-section)
* [환율](#exchange-rate)
* [그룹](#group)
* [작업 역할](#job-roles)
* [로그인 시도](#login-attempt)
* [우선 순위](#priority)
* [프로젝트 환경 설정](#project-preferences)
* [심각도](#severity)
* [상태](#status)
* [작업 및 문제 환경 설정](#tasks-issues-preferences)
* [사용자](#user)

### 액세스 수준 {#access-level}

사용자가 다음 작업 중 하나를 수행하면 시스템이 액세스 수준 로그 항목을 생성합니다.

* 액세스 수준 만들기
* 액세스 수준 삭제
* 액세스 수준 변경:

   * 라이센스 유형을 수정합니다.
   * 프로젝트, 작업, 문제, Portfolio, 프로그램, 보고서, 문서, 사용자 또는 템플릿에 대한 권한을 변경합니다

      >[!NOTE]
      >
      >시스템에서 재무 데이터 또는 다음 액세스 유형 내에 권한 변경 사항을 기록하지 않습니다. 보기 및 편집.
      >
      >예를 들어 사용자가 계획자 액세스 유형을 뷰에서 편집으로 변경하면 설정 미세 조정 드롭다운 메뉴에 포함된 정보가 표시되지 않습니다.

### 회사 {#company}

사용자가 다음 중 하나를 수행하면 시스템이 회사 감사 로그 항목을 생성합니다.

* 회사 만들기
* 회사 변경:

   * 이름 바꾸기
   * 구성원 추가 또는 제거
   * 그룹 필드에서 값을 추가, 편집 또는 삭제합니다
   * Job 역할에 대한 회사 청구 비율을 추가하거나 편집합니다
   * Job 역할에 대한 회사 청구 비율 제거
   * 조직의 기본 회사로 설정합니다.
   * 사용자 지정 양식을 첨부하거나 제거합니다

* 회사 삭제

상태에 대한 자세한 내용은 [상태 개요](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### 상황 {#condition}

사용자가 다음 작업 중 하나를 수행하면 시스템이 조건 감사 로그 항목을 생성합니다.

* 조건 만들기
* 조건 변경:

   * 이름을 변경합니다
   * 색상 변경
   * 기본값으로 설정합니다
   * 조건 설명을 변경하거나 제거합니다
   * 조건을 숨기거나 표시합니다

* 조건 삭제

작업 역할 구성에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### 사용자 정의 필드 {#custom-field}

사용자가 다음 작업 중 하나를 수행하면 시스템이 사용자 지정 필드 감사 로그 항목을 생성합니다.

* 사용자 지정 필드 만들기
* 사용자 지정 필드 변경:

   * 이름, 레이블, 지침 또는 형식을 변경합니다
   * 표시 유형 변경

      필드가 다음 유형 중 하나인 경우에만 사용할 수 있습니다. 단일 행, 단락, 드롭다운, 확인란, 라디오 단추

   * 필드 크기를 변경합니다.

      필드가 다음 유형 중 하나인 경우에만 사용할 수 있습니다. 한 줄, 단락, 서식이 있는 텍스트

   * 필드 선택 사항을 추가, 제거 또는 숨깁니다.
   * 필드 선택 레이블 또는 값을 편집합니다
   * 기본적으로 선택하거나 선택하지 않을 필드 선택을 구성합니다
   * 여러 선택 또는 단일 선택을 허용하도록 드롭다운 필드를 구성합니다
   * 날짜 필드를 구성하여 시간 표시 또는 표시 안 함
   * 하이퍼링크를 편집하거나 설명 텍스트 필드의 값을 변경합니다

* 사용자 지정 필드 삭제
* 사용자 지정 필드 공유

### 사용자 정의 양식 {#custom-forms}

사용자가 다음 작업 중 하나를 수행하면 시스템이 사용자 지정 Forms 감사 로그 항목을 생성합니다.

* 사용자 지정 양식 만들기
* 사용자 지정 양식 변경:

   * 이름 또는 설명을 변경합니다
   * 활성 상태임 또는 비활성화
   * 필드 또는 섹션 추가 또는 제거
   * 사용자 지정 섹션의 경우 추가 설정에서 설정을 변경합니다
   * 필드를 필수 또는 필수로 변경
   * 사용자 지정 필드에서 계산 변경
   * 지침 가리키기 텍스트에서 계산된 필드와 연결된 공식을 숨기거나 표시합니다
   * 이전 계산 업데이트 사용 또는 사용 안 함
   * 건너뛰기 로직 또는 표시 로직을 추가하거나 변경합니다.

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* 사용자 지정 양식 삭제
* 사용자 지정 양식 공유

### 사용자 정의 섹션 {#custom-section}

사용자가 사용자 지정 양식에서 다음 작업 중 하나를 수행하면 시스템이 사용자 지정 섹션 감사 로그 항목을 생성합니다.

* 사용자 지정 섹션 만들기
* 사용자 지정 섹션의 이름 또는 설명을 변경합니다
* 사용자 지정 섹션 삭제

사용자 지정 양식의 사용자 지정 섹션에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### 환율 {#exchange-rate}

사용자가 다음 작업 중 하나를 수행하면 시스템이 환율 감사 로그 항목을 생성합니다.

* 환율을 만듭니다
* 환율 변경:

   * 통화 추가
   * 통화 환율을 변경합니다
   * 시스템 전체에서 모든 프로젝트 및 보고서에 대한 기본(기본값) 통화로 통화를 설정합니다

* 환율 삭제

환율 구성에 대한 자세한 내용은 [환율 설정](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### 그룹 {#group}

사용자가 다음 작업 중 하나를 수행하면 시스템이 그룹 감사 로그 항목을 생성합니다.

* 그룹을 만듭니다
* 그룹 삭제
* 그룹 변경:

   * 사용자 추가 또는 제거
   * 하위 그룹 추가 또는 제거

### 작업 역할 {#job-roles}

사용자가 다음 작업 중 하나를 수행하면 시스템이 작업 역할 감사 로그 항목을 생성합니다.

* 작업 역할 만들기
* 작업 역할 변경:

   * 이름을 변경합니다
   * 설명을 추가, 변경 또는 제거합니다
   * 시간당 비용을 추가, 변경 또는 제거합니다(비용/시간).
   * 청구 비율을 추가, 변경 또는 제거합니다(청구/시간).

* 작업 역할 삭제

작업 역할 구성에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### 로그인 시도 {#login-attempt}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 로그인 시도 감사 로그 항목을 생성합니다.

* Workfront(브라우저 및 모바일 앱의)에서 로그인하거나 로그아웃하거나 로그인 시도에 실패했습니다
* 모든 Workfront 통합(예: Slack용 Workfront 및 Salesforce용 Workfront)에서 로그인, 로그아웃 또는 로그인 시도에 실패합니다
* Workfront API에 로그인하거나 로그아웃합니다

Workfront 관리자가 다른 이름으로 로그인 기능을 사용하는 경우 로그인 시도 로그가 기록되지 않습니다.

>[!NOTE]
>
>조직이 Adobe Admin Console에 온보딩된 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

### 우선 순위 {#priority}

사용자가 다음 작업 중 하나를 수행하면 시스템이 우선 순위 감사 로그 항목을 생성합니다.

* 우선 순위 만들기
* 우선 순위 변경:

   * 이름을 변경합니다
   * 색상 변경
   * 기본값으로 설정합니다
   * 우선 순위의 설명을 추가, 변경 또는 제거합니다
   * 우선 순위를 숨기거나 표시합니다

* 우선 순위 삭제

우선순위 구성에 대한 자세한 내용은 다음을 참조하십시오 [우선순위 만들기 및 사용자 지정](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### 프로젝트 환경 설정 {#project-preferences}

사용자가 다음 작업 중 하나를 수행하면 프로젝트 환경 설정 감사 로그 항목이 생성됩니다.

* 사용자 지정 분기 만들기
* 프로젝트 환경 설정 변경:

   * 잠금 또는 잠금 해제
   * 설정 중 하나를 변경합니다.
   * 활성화, 비활성화 또는 편집
   * 타임라인 계산을 편집합니다

* 사용자 지정 분기 삭제

프로젝트 환경 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### 심각도 {#severity}

사용자가 다음 작업 중 하나를 수행하면 시스템이 심각도 감사 로그 항목을 생성합니다.

* 문제 심각도 만들기
* 문제 심각도 변경:

   * 이름을 변경합니다
   * 색상 변경
   * 기본값으로 설정합니다
   * 심각도에 대한 설명을 변경하거나 제거합니다.
   * 심각도를 숨기거나 표시합니다.

* 문제 심각도 삭제

작업 역할 구성에 대한 자세한 내용은 [문제 심각도 만들기 또는 사용자 지정](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### 상태 {#status}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 상태 감사 로그 항목을 생성합니다.

* 시스템 또는 그룹 수준에서 상태를 만듭니다
* 시스템 또는 그룹 수준에서 상태를 변경합니다.

   * 이름 바꾸기
   * 기본 상태로 만듭니다
   * 잠금 또는 잠금 해제
   * 숨기거나 숨기지 않습니다
   * 색상 또는 설명을 변경합니다

* 시스템 또는 그룹 수준에서 상태를 삭제합니다.

상태에 대한 자세한 내용은 [상태 개요](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### 작업 및 문제 환경 설정 {#tasks-issues-preferences}

다음 방법 중 하나로 사용자가 작업 및 문제 환경 설정을 변경할 때 시스템에서 작업 및 문제 환경 설정 감사 로그 항목을 생성합니다.

* 기본 설정 잠금 또는 잠금 해제
* 기본 설정에 대한 설정 변경
* 작업, 문제 또는 요청에 대한 액세스 설정을 변경합니다

작업 및 문제 환경 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### 사용자 {#user}

사용자가 다음 작업 중 하나를 수행하면 시스템이 사용자 감사 로그 항목을 생성합니다.

* 사용자 만들기

   <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

   >[!NOTE]
   >
   >조직이 Adobe Admin Console에 온보딩된 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

* 사용자 삭제
* 사용자의 액세스 수준, 회사, 팀 또는 그룹 변경
* 사용자를 활성화합니다
* 사용자 비활성화
