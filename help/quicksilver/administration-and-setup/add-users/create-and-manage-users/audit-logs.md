---
title: 감사 로그
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 관리자는 감사 로그를 사용하여 지난 90일 동안 시스템에서 트리거된 사용자 변경 사항을 추적할 수 있습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 5a2df341a54d305807a1c9f175baf60b9007ffa2
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 3%

---

# 감사 로그

<!--Audited: 01/2024-->

Adobe Workfront 관리자는 아래에 설명된 감사 로그를 사용하여 지난 90일 동안 시스템에서 트리거된 사용자 변경 사항을 추적할 수 있습니다.

이 감사 로그에서 보고 필터링할 내용을 보려면 [감사 로그 보기 및 내보내기](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)를 참조하십시오.

## 감사 로그에서 찾을 수 있는 정보

다음 필드는 모든 감사 로그 항목에 기록됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">일자 및 시간</td> 
   <td>작업이 발생한 시간.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">로그 유형</td> 
   <td>액세스 수준 또는 사용자 정의 양식과 같은 감사 로그 유형입니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 이름</td> 
   <td> <p>작업을 수행한 사용자의 이름입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액션</td> 
   <td> 변경, 만들기 및 삭제와 같이 사용자가 수행한 작업입니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">오브젝트</td> 
   <td> 작업 결과로 영향을 받는 개체의 이름입니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">세부 사항</td> 
   <td>작업에 대한 추가 세부 정보. 전체 메시지를 읽으려면 마우스를 텍스트 위로 가져갑니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP 주소</td> 
   <td> <p>작업 시 작업을 수행한 사용자의 IP 주소입니다.</p> <p>일부 시스템 작업에는 IP 주소를 사용할 수 없습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 감사 로그 유형 및 이를 트리거하는 작업

* [액세스 수준](#access-level)
* [비즈니스 규칙](#business-rules)
* [회사](#company)
* [조건](#condition)
* [사용자 지정 필드](#custom-field)
* [사용자 정의 양식](#custom-forms)
* [사용자 지정 섹션](#custom-section)
* [환율](#exchange-rate)
* [그룹](#group)
* [작업 역할](#job-roles)
* [로그인 시도](#login-attempt)
* [우선 순위](#priority)
* [프로젝트 환경 설정](#project-preference)
* [심각도](#severity)
* [상태](#status)
* [작업 및 문제 환경 설정](#tasks-issues-preferences)
* [사용자](#user)

### 액세스 수준 {#access-level}

사용자가 다음 작업 중 하나를 수행하면 시스템이 액세스 수준 로그 항목을 생성합니다.

* 액세스 수준 만들기
* 액세스 수준 삭제
* 액세스 수준 변경:

   * 라이선스 유형 수정
   * 프로젝트, 작업, 문제, 포트폴리오, 프로그램, 보고서, 문서, 사용자 또는 템플릿에 대한 권한을 변경합니다.

     >[!NOTE]
     >
     >시스템은 재무 데이터 또는 보기 및 편집 액세스 유형에 대한 권한 변경 사항을 기록하지 않습니다.
     >
     >예를 들어 사용자가 계획자 액세스 유형을 보기에서 편집으로 변경하면 설정 세부 조정 드롭다운 메뉴에 포함된 정보가 시스템에 표시되지 않습니다.

### 비즈니스 규칙

비즈니스 규칙은 Ultimate Workfront 플랜을 구입한 고객에게만 제공됩니다. 자세한 내용은 [비즈니스 규칙 만들기 및 편집](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md)을 참조하세요.

사용자가 다음 중 하나를 수행하면 시스템에서 비즈니스 규칙 감사 로그 항목을 생성합니다.

* 비즈니스 규칙 만들기
* 비즈니스 규칙 편집:

   * 이름 바꾸기
   * 표현식 추가 또는 제거
   * 트리거 변경

* 비즈니스 규칙 삭제

### 회사 {#company}

사용자가 다음 중 하나를 수행하면 시스템이 회사 감사 로그 항목을 생성합니다.

* 회사 만들기
* 회사 변경:

   * 이름 바꾸기
   * 멤버 추가 또는 제거
   * 그룹 필드의 값을 추가, 편집 또는 삭제합니다.
   * 작업 역할에 대한 회사 청구 요금 추가 또는 편집
   * 작업 역할에 대한 회사 청구 요금 제거
   * 조직의 기본 회사로 설정합니다.
   * 사용자 정의 양식을 첨부하거나 제거합니다.

* 회사 삭제

상태에 대한 자세한 내용은 [상태 개요](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)를 참조하십시오.

### 조건 {#condition}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 조건 감사 로그 항목을 생성합니다.

* 조건 만들기
* 조건을 변경합니다.

   * 이름 변경
   * 색상 변경
   * 기본값으로 설정합니다.
   * 조건의 설명을 변경하거나 제거합니다.
   * 조건을 숨기거나 표시합니다.

* 조건 삭제

작업 역할 구성에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)을 참조하세요.

### 사용자 정의 필드 {#custom-field}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 사용자 정의 필드 감사 로그 항목을 생성합니다.

* 사용자 정의 필드 만들기
* 사용자 정의 필드를 변경합니다.

   * 이름, 레이블, 지침 또는 형식 변경
   * 표시 유형 변경

     이 기능은 필드가 한 줄, 단락, 드롭다운, 확인란, 라디오 버튼 유형 중 하나인 경우에만 사용할 수 있습니다

   * 필드 크기 변경

     이 기능은 필드가 한 줄, 단락, 서식이 있는 텍스트 유형 중 하나인 경우에만 사용할 수 있습니다

   * 필드 선택 사항을 추가, 제거 또는 숨깁니다.
   * 필드 선택 레이블 또는 값 편집
   * 기본적으로 선택하거나 선택하지 않도록 필드 선택을 구성합니다.
   * 다중 선택 또는 단일 선택을 허용하도록 드롭다운 필드를 구성합니다.
   * 날짜를 표시하거나 표시하지 않도록 날짜 필드를 구성합니다.
   * 하이퍼링크를 편집하거나 설명 텍스트 필드의 값을 변경합니다.

* 사용자 정의 필드 삭제
* 사용자 정의 필드 공유

### 사용자 정의 양식 {#custom-form}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 사용자 지정 Forms 감사 로그 항목을 생성합니다.

* 사용자 정의 양식 만들기
* 사용자 정의 양식을 변경합니다.

   * 이름 또는 설명을 변경합니다.
   * 활성화됨 또는 비활성화됨
   * 필드 또는 섹션 추가 또는 제거
   * 사용자 정의 섹션의 경우 추가 설정에서 설정을 변경합니다
   * 필드를 필수 또는 필수로 변경합니다.
   * 사용자 정의 필드에서 계산 변경
   * 지침 가리키기 텍스트에서 계산된 필드와 연결된 수식을 숨기거나 표시합니다
   * 이전 계산 업데이트 를 활성화하거나 비활성화합니다.
   * 건너뛰기 논리 또는 표시 논리 추가 또는 변경

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* 사용자 정의 양식 삭제
* 사용자 정의 양식 공유

### 사용자 정의 섹션 {#custom-section}

사용자가 사용자 정의 양식에서 다음 작업 중 하나를 수행하면 시스템이 사용자 정의 섹션 감사 로그 항목을 생성합니다.

* 사용자 정의 섹션 만들기
* 사용자 정의 섹션의 이름 또는 설명을 변경합니다.
* 사용자 정의 섹션을 삭제합니다.

사용자 정의 양식의 사용자 정의 섹션에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

### 환율 {#exchange-rate}

사용자가 다음 작업 중 하나를 수행하면 시스템이 환율 감사 로그 항목을 생성합니다.

* 환율 생성
* 환율을 변경합니다.

   * 통화 추가
   * 통화의 환율을 변경합니다.
   * 통화를 시스템 전체의 모든 프로젝트 및 보고서에 대한 기본(기본) 통화로 설정합니다.

* 환율을 삭제합니다.

환율 구성에 대한 자세한 내용은 [환율 설정](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)을 참조하십시오.

### 그룹 {#group}

사용자가 다음 작업 중 하나를 수행하면 시스템이 그룹 감사 로그 항목을 생성합니다.

* 그룹 만들기
* 그룹 삭제
* 그룹을 변경합니다.

   * 사용자 추가 또는 제거
   * 하위 그룹 추가 또는 제거

### 작업 역할 {#job-roles}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 작업 역할 감사 로그 항목을 생성합니다.

* 작업 역할 만들기
* 작업 역할을 변경합니다.

   * 이름 변경
   * 설명을 추가, 변경 또는 제거합니다.
   * 시간당 비용(비용/시간) 추가, 변경 또는 제거
   * 청구 요금(청구/시간)을 추가, 변경 또는 제거합니다.

* 작업 역할 삭제

작업 역할 구성에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

<!--DELETE THIS SECTION MARCH 2026-->

<!--
### Login Attempt {#login-attempt}

The system generates a Login Attempt audit log entry when a user does one of the following actions:

* Logs in, logs out, or fails a login attempt in Workfront (in a browser and in the mobile app)
* Logs in, logs out, or fails a login attempt in any Workfront integration (such as Workfront for Slack)
* Logs in or logs out of the Workfront API

Login Attempt Logs do not record when a Workfront administrator uses the Log In As feature.

>[!NOTE]
>
>This is not available if your organization has been onboarded to the Adobe Admin Console. See your network or IT administrator if you need more information.

-->

### 우선순위 {#priority}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 우선 순위 감사 로그 항목을 생성합니다.

* 우선 순위를 만듭니다.
* 우선 순위를 변경합니다.

   * 이름 변경
   * 색상 변경
   * 기본값으로 설정합니다.
   * 우선 순위 설명을 추가, 변경 또는 제거합니다.
   * 우선 순위를 숨기거나 표시합니다.

* 우선 순위를 삭제합니다.

우선 순위 구성에 대한 자세한 내용은 [우선 순위 만들기 및 사용자 지정](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md)을 참조하십시오.

### 프로젝트 환경 설정 {#project-preference}

사용자가 다음 작업 중 하나를 수행하면 시스템이 프로젝트 환경 설정 감사 로그 항목을 생성합니다.

* 사용자 정의 영역 만들기
* 프로젝트 환경 설정을 변경합니다.

   * 잠금 또는 잠금 해제
   * 설정 중 하나를 변경합니다.
   * 활성화, 비활성화 또는 편집
   * 타임라인 계산을 편집합니다.

* 사용자 정의 영역 삭제

프로젝트 환경 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

### 심각도 {#severity}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 심각도 감사 로그 항목을 생성합니다.

* 문제 심각도 만들기
* 문제 심각도를 변경합니다.

   * 이름 변경
   * 색상 변경
   * 기본값으로 설정합니다.
   * 심각도 설명을 변경하거나 제거합니다.
   * 심각도를 숨기거나 표시합니다.

* 문제 심각도 삭제

작업 역할 구성에 대한 자세한 내용은 [문제 심각도 만들기 또는 사용자 지정](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md)을 참조하십시오.

### 상태 {#status}

사용자가 다음 작업 중 하나를 수행하면 시스템에서 상태 감사 로그 항목을 생성합니다.

* 시스템 또는 그룹 수준에서 상태를 만듭니다.
* 시스템 또는 그룹 수준의 상태를 변경합니다.

   * 이름 바꾸기
   * 기본 상태로 설정
   * 잠금 또는 잠금 해제
   * 숨기거나 해제합니다.
   * 색상 또는 설명을 변경합니다.

* 시스템 또는 그룹 수준에서 상태를 삭제합니다.

상태에 대한 자세한 내용은 [상태 개요](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)를 참조하십시오.

### 작업 및 문제 환경 설정 {#tasks-issues-preferences}

사용자가 다음 방법 중 하나로 작업 및 문제 환경 설정을 변경하면 시스템에서 작업 및 문제 환경 설정 감사 로그 항목을 생성합니다.

* 환경 설정 잠금 또는 잠금 해제
* 환경 설정 변경
* 작업, 문제 또는 요청에 대한 액세스 설정 변경

작업 및 문제 환경 설정에 대한 자세한 내용은 [시스템 전체의 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

### 사용자 {#user}

<!--DELETE THIS SECTION MARCH 2026-->
<!--
The system generates a User audit log entry when a user does one of the following actions:

* Creates a user

  >[!NOTE]
  >
  >This is not available if your organization has been onboarded to the Adobe Admin Console. See your network or IT administrator if you need more information.

* Deletes a user
* Changes a user's access level, company, team, or group
* Activates a user
* Deactivates a user-->
