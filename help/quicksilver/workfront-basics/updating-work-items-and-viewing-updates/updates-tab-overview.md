---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 업데이트 탭 개요
description: 업데이트 탭에는 지난 90일 이내에 수행한 최신 업데이트 중 최대 200개가 표시됩니다.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 799a2f3463ee98d57b13edfda8a0c93629439ea3
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 6%

---

# 업데이트 탭 개요

업데이트 탭에는 지난 90일 이내에 수행한 최신 업데이트 중 최대 200개가 표시됩니다. 다음 객체에 대한 업데이트에 응답할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>프로젝트</li> 
     <li>포트폴리오</li> 
     <li>프로그램</li> 
     <li>템플릿</li> 
     <li>템플릿 작업</li> 
     <li>작업</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>문제</li> 
     <li>반복</li> 
     <li>스토리</li> 
     <li>사용자</li> 
     <li>문서</li> 
     <li>타임시트</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 상위 등급 개체에도 표시되는 업데이트

다음 표에 표시된 것처럼 특정 개체의 업데이트에 대한 응답도 상위 등급 개체의 업데이트 탭에 표시됩니다.

예를 들어 작업에 업데이트를 추가하면 해당 작업의 업데이트 탭 및 작업이 포함된 프로젝트의 업데이트 탭에 업데이트가 나타납니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>원본 업데이트가 추가된 개체</strong> </th> 
   <th> <p><strong>원래 업데이트도 표시되는 등급이 높은 개체</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>문제</td> 
   <td>프로젝트</td> 
  </tr> 
  <tr> 
   <td>작업</td> 
   <td>프로젝트</td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td>프로그램, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>문서 </td> 
   <td>문서가 첨부된 객체, 프로젝트 </td> 
  </tr> 
  <tr> 
   <td>프로그램</td> 
   <td>포트폴리오</td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td>팀</td> 
  </tr> 
  <tr> 
   <td>타임시트</td> 
   <td>사용자, 팀</td> 
  </tr> 
  <tr> 
   <td>템플릿 작업</td> 
   <td>템플릿</td> 
  </tr> 
  <tr> 
   <td>스토리</td> 
   <td>반복, 팀</td> 
  </tr> 
  <tr> 
   <td>반복</td> 
   <td>팀</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>시스템 업데이트에 추가된 응답이 상위 개체에 롤업되지 않습니다. 하위 개체에 대한 직접 답장과 기존 업데이트에 추가된 응답만 상위 개체에 롤업됩니다.

Adobe Workfront의 개체 계층 구조에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 업데이트 탭의 제한 사항

### 사용자 및 팀의 제한 사항

팀에서 업데이트할 수 없습니다. 팀의 업데이트 탭은 다음 객체에 입력한 업데이트로 채워집니다.

* 사용자
* 타임시트
* 스토리
* 반복

사용자 및 팀의 업데이트 탭에서 지난 90일 동안 입력한 업데이트를 볼 수 있습니다.

사용자 또는 팀이 90일 제한 이상의 업데이트를 모두 보려면 노트에 대한 보고서를 작성할 수 있습니다. 보고서에는 사용자 또는 팀에 대한 모든 업데이트를 표시하는 시간 필터가 있지 않아야 합니다. 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 다른 사용자를 대신하여 주석을 입력할 때 제한 사항

Adobe Workfront 관리자 및 그룹 관리자는 다른 사용자로 로그인하여 Workfront에서 주석 입력과 같은 작업을 수행할 수 있습니다. (자세한 내용은 [다른 사용자로 로그인](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)) 다른 사용자를 대신하여 작성한 모든 주석은 주석에 표시됩니다.

그룹 관리자는 다른 사람을 대신하여 주석을 작성할 수 있지만 해당 설명을 삭제할 수는 없습니다. Adobe Workfront 관리자만 다른 사용자를 대신하여 작성한 주석을 삭제할 수 있습니다.

## 분개 입력 보고서를 사용하여 작업 항목에 대한 시스템 갱신 조회

분개 입력 보고서 시스템은 프로젝트, 작업 및 문제의 갱신 영역에서 갱신됩니다.

보고서를 통해 다음을 확인할 수 있습니다.

* 발생한 상태 변경 수
* 작업 또는 문제가 삭제된 경우
* 프로젝트 진행 중에 중요한 사용자 지정 필드의 값이 변경되는 방법
* 프로젝트 진행 중에 변경된 중요한 날짜
* 프로젝트 진행 과정에서 우선순위가 변경된 경우
* 프로젝트 소유자가 변경된 경우

자세한 내용은 [업데이트 영역에 대한 보고서](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
