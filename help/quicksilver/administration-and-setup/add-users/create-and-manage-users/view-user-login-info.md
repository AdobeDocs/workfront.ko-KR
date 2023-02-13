---
title: 사용자 로그인 정보 보기
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 사용자 목록 보기 또는 사용자 보고서에 이 정보를 포함할지 여부를 표시하여 사용자가 Workfront에 마지막으로 로그인한 빈도를 확인할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# 사용자 로그인 정보 보기

사용자 목록 보기 또는 사용자 보고서에 이 정보를 포함할지 여부를 표시하여 사용자가 Adobe Workfront에 마지막으로 로그인한 빈도를 확인할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

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
   <td> <p>플랜 </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템 관리자 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> </li> 
     <li> <p><b>사용자</b> 액세스 수준에서 설정 <b>편집</b> 액세스, 사용 <b>만들기</b> 둘 중 적어도 하나 <b>사용자 관리자</b> 옵션 사용 <b>설정 세부 조정</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>이 두 옵션 중 사용자가 <b>관리자(그룹 사용자)</b> 이 활성화되어 있으면 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> <p>에 대한 자세한 정보 <b>사용자</b> 액세스 수준에서 설정하는 방법은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront이 로그인 정보를 기록하는 방법

Workfront은 시스템에 로그인하는 사용자에 대해 다음 정보를 기록합니다.

* **로그인 수**: Workfront에서는 24시간마다 애플리케이션에 로그인하는 사용자를 계산합니다. 한 사용자가 서로 다른 브라우저, 컴퓨터 또는 모바일 장치를 사용하여 여러 번 로그인하는 경우 Workfront에서는 한 번에 발생한 모든 로그인을 한 로그인으로 계산합니다. 로그인 수에는 사용자를 만들 때부터 시작되는 정보가 포함됩니다.
* **마지막 로그인 날짜**: 사용자가 로그인한 마지막 날짜입니다. 브라우저, 모바일 장치 또는 기타 애플리케이션에서 모든 로그인의 날짜가 이 필드에 기록됩니다.

다음 방법 중 하나로 Workfront에 로그인하는 것은 Workfront에 로그인하는 것으로 계산됩니다.

* Workfront 웹 애플리케이션
* Workfront 모바일 앱(iOS 또는 Android 장치)
* 다른 타사 애플리케이션(Slack, Jira)과 Workfront 통합을 지원하는 모든 기능
* Workfront과 다른 타사 애플리케이션 간의 모든 사용자 지정 통합.
* Workfront API

   >[!NOTE]
   >
   >Workfront API를 통해 Workfront에 로그인하는 것은 아직 Adobe 비즈니스 플랫폼에 온보딩되지 않은 조직에서만 사용할 수 있습니다.

## 사용자 목록 또는 보고서에 사용 정보 표시

사용자 목록 보기 또는 사용자 보고서에 로그인 수 및 마지막 로그인 날짜 필드를 표시할 수 있습니다.\
보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

사용자 목록 보기에 사용 정보를 표시하려면 다음을 수행하십시오.

1. Workfront의 사용자 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 클릭 **열 추가** 화면 오른쪽 아래 모서리 근처에 있습니다.
1. 에서 **이 열에 표시** 필드, 입력 시작 **로그인 수**&#x200B;을 선택한 다음 아래 목록에 이 이름이 표시되면 선택합니다 **사용자**.

1. 클릭 **열 추가** 다시 한 번
1. 에서 **열에 표시** 필드, 입력 시작 **마지막 로그인 날짜**&#x200B;을 선택한 다음 아래 목록에 이 이름이 표시되면 선택합니다 **사용자**.

1. (선택 사항) **고급 옵션**&#x200B;를 선택한 다음 을 선택합니다 **필드 형식** 드롭다운 메뉴에서 열에 마지막 로그인 요일을 포함하십시오.

1. 클릭 **보기 저장**.\
   보기에는 사용자가 로그인한 횟수와 마지막으로 로그인한 시기에 대한 정보가 포함됩니다.
