---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira 활동 로그 보기
description: 로서의 [!DNL Jira] 관리자는 두 항목 사이에 티켓을 동기화하거나 만드는 동안 발생하는 예외와 오류를 볼 수 있습니다 [!DNL Adobe Workfront] 및 [!DNL Jira] ( 활동 로그)를 참조하십시오.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 보기 [!UICONTROL [!DNL Jira] 활동 로그]

로서의 [!DNL Jira] 관리자는 두 항목 사이에 티켓을 동기화하거나 만드는 동안 발생하는 예외와 오류를 볼 수 있습니다 [!DNL Adobe Workfront] 및 [!DNL Jira] 에서 [!UICONTROL 활동 로그].

활동 로그에서 최대 500개의 항목을 볼 수 있으며 가장 최근 항목으로 시작하는 항목이 나열됩니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 플랜</a>*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 라이선스 개요</a>*</td> 
   <td> <p>[!UICONTROL 계획]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 액세스</td> 
   <td> <p>시스템 관리자 액세스</p> <p>중요 사항: 에서 별도의 시스템 관리자 계정을 만드는 것이 좋습니다. [!DNL Jira] 및 [!DNL Workfront] 사용자에게 첨부할 수 있는 기존 항목을 사용하는 대신 이 통합에 전념할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

항목 사이에 항목을 연결하려면 먼저 [!DNL Workfront] 및 [!DNL Jira]:

* 설치 [!DNL Workfront for Jira]

   설치 지침 [!DNL Workfront for Jira]를 참조하십시오. [설치 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 액세스 권한 [!UICONTROL [!DNL Jira] 활동 로그]:

1. 시스템 관리자로 Jira에 로그인합니다.
1. 클릭 **[!UICONTROL 설정]** 주 [!DNL Jira] 메뉴 아래의 제품에서 사용할 수 있습니다.
1. 클릭 **[!UICONTROL 추가 기능]**, 그런 다음 **[!UICONTROL 추가 기능 관리]**.

1. 를 확장합니다. **[!DNL Workfront]** 추가 기능.
1. 클릭 **[!UICONTROL 구성]**.
1. 에 로그인합니다. [!DNL Workfront] 시스템 관리자
1. 을(를) 선택합니다 **[!UICONTROL 활동 로그]** 탭.

   항목을 만들거나 두 응용 프로그램 간에 필드를 동기화하는 동안 발생한 예외 및 오류에 대한 정보를 봅니다.

   로그에는 다음 필드가 포함되어 있습니다.

   * 발생 날짜
   * Jira의 사용자 이름입니다
   * Jira 문제 번호
   * 발생한 오류에 대한 간략한 설명입니다.
