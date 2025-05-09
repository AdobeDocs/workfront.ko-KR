---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira 활동 로그 보기
description: ' [!DNL Jira] 관리자는  [!DNL Adobe Workfront] 에서 [!DNL Jira]  사이의 티켓을 동기화하거나 만드는 동안 발생하는 예외와 오류를 작업 로그에서 볼 수 있습니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# [!UICONTROL [!DNL Jira] 작업 로그 보기]

[!DNL Jira] 관리자는 [!UICONTROL 활동 로그]에서 [!DNL Adobe Workfront]에서 [!DNL Jira] 사이의 티켓을 동기화하거나 만드는 동안 발생하는 예외와 오류를 볼 수 있습니다.

활동 로그에서 최대 500개의 항목을 볼 수 있으며 가장 최근 항목으로 시작하여 나열됩니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront] 계획</a>*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 라이선스 개요</a>*</td> 
   <td> <p>[!UICONTROL 계획]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p>중요: 사용자에게 첨부할 수 있는 기존 계정을 사용하는 대신 [!DNL Jira] 및 [!DNL Workfront]에서 별도의 시스템 관리자 계정을 만들어 이 통합 전용을 사용하는 것이 좋습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다. [!DNL Workfront] 관리자에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>를 참조하십시오.</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 전제 조건

[!DNL Workfront]과(와) [!DNL Jira] 사이의 항목을 연결하려면 먼저

* [!DNL Workfront for Jira] 설치

  [!DNL Workfront for Jira] 설치에 대한 지침은 [설치 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)를 참조하십시오.

## [!UICONTROL [!DNL Jira] 작업 로그]에 액세스:

1. 시스템 관리자로 Jira에 로그인합니다.
1. 주 [!DNL Jira] 메뉴에서 **[!UICONTROL 설정]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 추가 기능]**&#x200B;을 클릭한 다음 **[!UICONTROL 추가 기능 관리]**&#x200B;를 클릭합니다.

1. **[!DNL Workfront]** 추가 기능을 확장합니다.
1. **[!UICONTROL 구성]**&#x200B;을 클릭합니다.
1. 시스템 관리자로 [!DNL Workfront]에 로그인합니다.
1. **[!UICONTROL 활동 로그]** 탭을 선택합니다.

   항목을 생성하거나 두 응용 프로그램 간의 필드를 동기화하는 동안 발생한 예외 및 오류에 대한 정보를 봅니다.

   로그에는 다음 필드가 포함되어 있습니다.

   * 발생 날짜
   * Jira의 사용자 이름
   * Jira 문제 번호
   * 발생한 오류에 대한 간단한 설명입니다.
