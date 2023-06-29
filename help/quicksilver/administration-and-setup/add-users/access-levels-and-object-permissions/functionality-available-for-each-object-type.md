---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 액세스,모델,단계,다이어그램,수준,권한
navigation-topic: access-levels
title: 다양한 액세스 수준에 대해 각 객체 유형에 사용할 수 있는 기능
description: 다음 표에는 다양한 액세스 레벨의 각 객체 유형에 사용할 수 있는 기능이 나열되어 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 11%

---

# 다양한 액세스 수준에 대해 각 객체 유형에 사용할 수 있는 기능

{{highlighted-preview}}

다음 표에는 다양한 액세스 레벨의 각 객체 유형에 사용할 수 있는 기능이 나열되어 있습니다.

또한 Workfront 관리자가 액세스 수준을 사용하여 비활성화하거나 활성화할 수 있는 작업도 표시됩니다.

## 프로젝트

플랜 라이선스가 있는 사용자만 프로젝트에 대한 전체 액세스 권한을 부여할 수 있습니다.

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; |   |   |   |   |
| 복사 | ✓&#42; |   |   |   |   |
| 삭제 | ✓&#42; |   |   |   |   |
| 공유 | ✓&#42; | ✓&#42; |   |   |   |
| 시스템 전체 공유 | ✓&#42; |   |   |   |   |
| 보기 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 사용자 정의 양식 추가 | ✓ |   |   |   |   |
| 사용자 정의 필드 업데이트 | ✓ | ✓ |   |   |   |
| 승인 프로세스 추가 | ✓ |   |   |   |   |
| 프로젝트 승인 | ✓ | ✓ | ✓ |   |   |
| 문서 추가 | ✓ | ✓ | ✓ |   |   |
| 문제 추가 | ✓ | ✓ |   |   |   |
|  작업 추가 | ✓ | ✓ |   |   |   |
| 업데이트/주석 제공 | ✓ | ✓ | ✓ |   |   |
| 상태 변경 | ✓ |   |   |   |   |
| 시간 기록 | ✓ | ✓ |   |   |   |
| 할당 편집 | ✓ | ✓ |   |   |   |
| 기준선 관리 | ✓ |   |   |   |   |
| 위험 관리 | ✓ |   |   |   |   |
| 재무 관리 | ✓ |   |   |   |   |
| 경비 추가/편집 | ✓ | ✓ |   |   |   |
| 템플릿 첨부 | ✓ |   |   |   |   |
| 템플릿으로 저장 | ✓ |   |   |   |   |
| 비즈니스 사례 추가/편집 | ✓ |   |   |   |   |
| 프로젝트 세부 정보 편집 | ✓ |   |   |   |   |
| 직원 편집 | ✓ |   |   |   |   |
| MS 프로젝트로 내보내기 | ✓ | ✓ | ✓ |   |   |
| 재무/타임라인 다시 계산 | ✓ |   |   |   |   |
| 대기열 속성 설정 | ✓ |   |   |   |   |



&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 작업

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; | ✓&#42; |   |   |   |
| 삭제 | ✓&#42; | ✓&#42; |   |   |   |
| 공유 | ✓&#42; | ✓&#42; |   |   |   |
| 시스템 전체 공유 | ✓&#42; |   |   |   |   |
| 보기 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 전임 작업 추가 | ✓ | ✓ |   |   |   |
|  문제 추가 | ✓ | ✓ |   |   |   |
| 작업 편집(상태 제외) | ✓ | ✓ |   |   |   |
| 작업 상태 변경 | ✓ | ✓ |   |   |   |
| 문서 추가 | ✓ | ✓ | ✓ |   |   |
| 작업 복사 | ✓ | ✓ |   |   |   |
| 작업 이동 | ✓ | ✓ |   |   |   |
| 시간 기록 | ✓ | ✓ |   |   |   |
| 할당 수락 | ✓ | ✓ |   |   |   |
| 할당하기 | ✓ | ✓ | 인라인 편집만 | 인라인 편집만 |   |
| 사용자 정의 양식 첨부 | ✓ | ✓ |   |   |   |
| 사용자 정의 필드 편집 | ✓ | ✓ |   |   |   |
| 승인 프로세스 만들기 | ✓ | ✓ |   |   |   |
| 작업 승인 | ✓ | ✓ | ✓ |   |   |
| 재무 편집 | ✓ |   |   |   |   |
| 경비 추가/편집 | ✓ | ✓ |   |   |   |
| 재무 보기 | ✓ | ✓ | ✓ |   |   |
| 업데이트/주석 | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 문제

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 편집 | ✓ | ✓ | ✓ | ✓ |   |
| 삭제 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 공유 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 시스템 전체 공유 | ✓&#42; |   |   |   |   |
| 보기 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 사용자 정의 양식 첨부 | ✓ | ✓ | ✓ | ✓ |   |
| 사용자 정의 필드 편집 | ✓ | ✓ | ✓ | ✓ |   |
| 문제 승인 | ✓ | ✓ | ✓ | ✓ |   |
| 승인 프로세스 추가 | ✓ | ✓ | ✓ | ✓ |   |
| 문서 추가 | ✓ | ✓ | ✓ | ✓ |   |
| 문제 복사 | ✓ | ✓ | ✓ | ✓ |   |
| 문제 이동 | ✓ | ✓ | ✓ | ✓ |   |
| 시간 기록 | ✓ | ✓ |   |   |   |
| 문제를 프로젝트로 전환 | ✓ | ✓ |   |   |   |
| 문제를 작업으로 전환 | ✓ |   |   |   |   |
| 할당 수락 | ✓ | ✓ |   |   |   |
| 할당하기 | ✓ | ✓ |   |   |   |
| 업데이트 및 주석 추가 | ✓ | ✓ | ✓ | ✓ |   |



&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 포트폴리오

플랜 라이선스가 있는 사용자만 포트폴리오에 대한 전체 액세스 권한을 가질 수 있습니다.

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; |   |   |   |   |
| 삭제 | ✓&#42; |   |   |   |   |
| 공유 | ✓&#42; |   |   |   |   |
| 시스템 전체 공유 | ✓&#42; |   |   |   |   |
| 보기 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 세부 정보 편집 | ✓ |   |   |   |   |
| 사용자 정의 양식 첨부 | ✓ |   |   |   |   |
| 사용자 정의 필드 편집 | ✓ |   |   |   |   |
| 프로젝트 추가 및 제거 | ✓ |   |   |   |   |
| 프로젝트 승인 | ✓ |   |   |   |   |
| Portfolio 최적화 | ✓ |   |   |   |   |
| 문서 추가 | ✓ | ✓ | ✓ |   |   |
| 업데이트 및 주석 추가 | ✓ | ✓ | ✓ |   |   |



&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 프로그램

플랜 라이선스가 있는 사용자만 프로그램에 대한 전체 액세스 권한을 가질 수 있습니다.

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; |   |   |   |   |
| 삭제 | ✓&#42; |   |   |   |   |
| 공유 | ✓&#42; |   |   |   |   |
| 시스템 전체 공유 | ✓&#42; |   |   |   |   |
| 보기 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 세부 정보 편집 | ✓ |   |   |   |   |
| 사용자 정의 양식 첨부 | ✓ |   |   |   |   |
| 사용자 정의 필드 편집 | ✓ |   |   |   |   |
| 프로젝트 추가 및 제거 | ✓ |   |   |   |   |
| 프로젝트 승인 | ✓ |   |   |   |   |
| 포트폴리오 최적화 | ✓ |   |   |   |   |
| 문서 추가 | ✓ | ✓ | ✓ |   |   |
| 추가 업데이트 및 주석 추가 | ✓ | ✓ | ✓ |   |   |



&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 보고서, 대시보드 및 캘린더

플랜 라이선스가 있는 사용자는 보고서에 대한 전체 액세스 권한을 가질 수 있습니다. 다른 모든 액세스 수준에는 보고서에 대한 보기 액세스 권한이 있습니다.

| 개 액션 | 플래너 | 보조 | 검토자 | 요청 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; |   |   |   |   |
| 삭제 | ✓&#42; |   |   |   |   |
| 기본 제공 보고서 보기 | ✓&#42; |   |   |   |   |
| 공유 | ✓&#42; | ✓ | ✓ |   |   |
| 캘린더 및 보고서 공개 | ✓&#42; |   |   |   |   |
| 시스템 전체 공유 | ✓&#42; |   |   |   |   |
| 보기 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 편집 | ✓ |   |   |   |   |
| 복사 | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>요청자는 공유된 보고서만 볼 수 있습니다.

## 필터, 보기 및 그룹화

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>개 액션</p> </th> 
   <th> <p>플래너</p> </th> 
   <th> <p>보조</p> </th> 
   <th> <p>검토자</p> </th> 
   <th> <p>요청자</p> </th> 
   <th>외부 사용자<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>만들기</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>삭제</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>공유</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>시스템 전체 공유</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>보기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>편집</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 문서

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 삭제(문서 및 폴더) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 공유 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 공개 공유(외부) | ✓&#42; |   |   |   |   |
| 시스템 전체 공유 | ✓&#42; | ✓&#42; |   |   |   |
| 보기 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 세부 정보 편집 | ✓ | ✓ | ✓ | ✓ |   |
| 다운로드 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 체크아웃 | ✓ | ✓ | ✓ | ✓ |   |
| 승인자 추가 | ✓ | ✓ | ✓ | ✓ |   |
| 문서 승인 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 사용자 정의 양식 첨부 | ✓ | ✓ | ✓ | ✓ |   |
| 사용자 정의 필드 편집 | ✓ | ✓ | ✓ | ✓ |   |
| (오브젝트)로 이동 | ✓ | ✓ | ✓ | ✓ |   |
| (통합) (으)로 보내기 | ✓ | ✓ | ✓ | ✓ |   |
| 업데이트 및 주석 추가 | ✓ | ✓ | ✓ | ✓ |   |
| 새 버전 업로드 | ✓ | ✓ | ✓ | ✓ |   |
| 버전 삭제 | ✓ | ✓ | ✓ | ✓ |   |
| 미리보기 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 증명 | ✓ | ✓ | ✓ | ✓ |   |
| 증명 생성 | ✓ | ✓ |   |   |   |
| 증명 제거 | ✓ | ✓ | ✓ | ✓ |   |
| 추가/제거&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 이름 바꾸기&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 링크(통합 사용) | ✓ | ✓ | ✓ | ✓ |   |
| 연결 해제(통합 사용) | ✓ | ✓ | ✓ | ✓ |   |

{style="table-layout:auto"}

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;문서 폴더에만 사용할 수 있고 문서에는 사용할 수 없음

## 사용자

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>개 액션</p> </th> 
   <th> <p>플래너</p> </th> 
   <th>보조</th> 
   <th> <p>검토자</p> </th> 
   <th> <p>요청자</p> </th> 
   <th> <p>외부 사용자**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>만들기</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>삭제</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>모든 사용자의 암호 편집, 삭제, 비활성화, 다음으로 로그인 또는 재설정</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>관리하는 그룹의 모든 사용자에 대한 암호를 편집, 삭제, 비활성화, 다음으로 로그인 또는 재설정합니다</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>사용자 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>연락처 정보 보기</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;외부 사용자는 다른 사용자만 검색할 수 있습니다.

## 팀

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>개 액션</p> </th> 
   <th> <p>플래너</p> </th> 
   <th>보조</th> 
   <th> <p>검토자</p> </th> 
   <th> <p>요청자</p> </th> 
   <th> <p>외부 사용자*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>만들기</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>삭제</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>속한 팀 편집</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>자신이 관리하는 그룹에서 팀 편집</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>모든 팀 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>해당 그룹과 관련된 팀 보기</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 템플릿

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 만들기 | ✓&#42; |   |   |   |   |
| 삭제 | ✓&#42; |   |   |   |   |
| 공유 | ✓&#42; |   |   |   |   |
| 시스템 전체 공유 | ✓&#42; |   |   |   |   |
| 보기 | ✓&#42; |   |   |   |   |
| 복사 | ✓ |   |   |   |   |
| 템플릿 세부 정보 편집 | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 재무 데이터

플랜 라이선스가 있는 사용자만 재무 데이터에 대한 전체 액세스 권한을 가질 수 있습니다.

요청 및 외부 사용자 라이선스 유형은 이러한 개체 및 영역에 대한 액세스 권한이 없으므로 여기에 포함되지 않습니다.

| 개 액션 | 플래너 | 보조 | 검토자 |
|---|---|---|---|
| 역할 청구 및 비용 요금 편집 | ✓&#42; |   |   |
| 사용자 청구 및 비용 요금 편집 | ✓&#42; |   |   |
| 역할 청구 및 비용 요금 보기 | ✓&#42; |   |   |
| 사용자 청구 및 비용 요금 보기 | ✓&#42; |   |   |
| 청구 기록 관리 | ✓ |   |   |
| 경비 관리 | ✓ | ✓ |   |
| 재무 데이터 보기 | ✓&#42; | ✓&#42; | ✓&#42; |
| <span class="preview">등급 카드 관리</span> | ✓ |   |   |
| 자원 계획 도구에서 원가별 정보 조회 | ✓ |   |   |
| 자원 계획 도구의 예산 자원&#42;&#42; | ✓ |   |   |
| 자원 계획 도구에서 자원 할당 조회&#42; | ✓ | ✓ | ✓ |
| 프로젝트에 대한 위험 만들기 | ✓ |   |   |
| 프로젝트에 대한 위험 보기 | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;리소스 관리에 대한 추가 액세스 권한이 필요합니다.

## 리소스 관리

플랜 라이선스가 있는 사용자만 다음에 대한 전체 액세스 권한을 가질 수 있습니다. [개체 또는 영역 선택]. 다른 라이선스 유형은 Workfront에서 리소스 관리에 대한 액세스가 제한되거나 없을 수 있습니다.

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 플래너에서 우선 순위 및 예산 시간 편집 | ✓&#42; |   |   |   |   |
| 리소스 풀 만들기, 편집, 삭제&#42;&#42; | ✓&#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| 리소스 플래너에서 프로젝트 우선 순위 보기 | ✓&#42; |   |   |   |   |
| 자원 계획 도구에서 자원 할당 조회 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 리소스 풀 보기 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 리소스 계획 도구의 예산 리소스&#42;&#42; | ✓ |   |   |   |   |
| 프로젝트, 템플릿 및 사용자에 리소스 풀 첨부 | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Workfront 관리자는 액세스 수준을 사용하여 이 기능을 비활성화하거나 활성화할 수 있습니다. 자세한 내용은 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;재무 데이터에 대한 추가 액세스 및 프로젝트 재무 권한이 필요합니다. 재무 데이터에 대한 액세스 권한이 없는 플래너 사용자에게 리소스 관리 액세스 권한을 부여하는 경우 사용자는 리소스 플래너에서 시간별 할당을 계속 볼 수 있지만 비용 보기로 전환하거나 비즈니스 사례를 볼 수는 없습니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 및 [개체에 대한 재무 권한 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;[고급 설정]에서 [할당]을 활성화하여 개체에 기여할 수 있는 권한이 필요합니다. 자세한 내용은 섹션을 참조하십시오 [상속된 권한 및 개체의 계층 구조 이해](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) 이 문서에서 [오브젝트에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 시나리오 플래너 영역

| 개 액션 | 플래너 | 보조 | 검토자 | 요청자 | 외부 사용자 |
|---|---|---|---|---|---|
| 기존 계획 및 이니셔티브 생성/편집 | ✓ | ✓ | ✓ |   |   |
| 계획 및 이니셔티브에 대한 작업 역할 정보 추가 또는 편집&#42; | ✓ | ✓ | ✓ |   |   |
| 계획 및 이니셔티브의 비용 정보 추가 또는 편집&#42; | ✓ | ✓ | ✓ |   |   |
| 계획 및 이니셔티브 삭제 | ✓ | ✓ | ✓ |   |   |
| 메인 메뉴에서 시나리오 보기 ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |   |
| 사용자가 만든 계획 및 이니셔티브 보기&#42; | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

>[!NOTE]
>
>플랜에 대한 링크가 다른 사용자와 공유되는 경우에만 다른 사용자가 만든 플랜을 볼 수 있습니다.

&#42; 사용자가 계획이나 이니셔티브에서 재무 데이터를 보려면 재무 데이터에 액세스해야 합니다. 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Workfront 목표 영역

| 액션 | 보기 | 편집 |
|---|---|---|
| 만들기 |   | ✓ |
| 모든 목표 편집/삭제 |   | ✓ |
| 메인 메뉴에서 목표 보기 | ✓ | ✓ |
| 공유 링크에서 목표 영역 보기 | ✓ | ✓ |
| 시스템의 모든 목표 보기 | ✓ | ✓ |
| 모든 목표 활성화/비활성화/종료 |   | ✓ |
| 활동 만들기/편집/삭제 |   | ✓ |
| 결과 만들기/편집/삭제 |   | ✓ |
| 정렬된 목표 추가 |   | ✓ |
| 결과 또는 활동에 대한 진행 업데이트 |   | ✓ |
| 목표, 결과 또는 활동 소유 | ✓ | ✓ |
| 목표에 대한 댓글 | ✓ | ✓ |
| 목표 복사 |   | ✓ |
| 왼쪽 패널에서 목표 목록 섹션 보기 | ✓ | ✓ |
| 왼쪽 패널에서 그래프 섹션 보기 | ✓ | ✓ |
| 왼쪽 패널에서 목표 정렬 섹션 보기 | ✓ | ✓ |

