---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ' [!DNL Adobe Workfront] 사용자 지정 새로 고침 샌드박스 환경'
description: 사용자 지정 새로 고침 샌드박스는 프로덕션 환경의 데이터를 사용하여 테스트하고 작업할 수 있는 환경입니다. 또한 교육을 실행하고 설정 기능을 결정하는 데에도 이상적입니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 5b5f9083ed4b60fa6642100cfb9b0da46799dffa
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 사용자 지정 새로 고침 샌드박스 환경

사용자 지정 새로 고침 샌드박스는 프로덕션 환경의 데이터를 사용하여 테스트하고 작업할 수 있는 환경입니다. 또한 교육을 실행하고 설정 기능을 결정하는 데에도 이상적입니다.

>[!NOTE]
>
>이는 [!DNL Workfront] 프로덕션 환경을 복제하는 테스트 환경이기도 한 미리 보기 샌드박스와는 다릅니다.
>
>* 프로덕션 환경에서는 미리보기 샌드박스에 새로운 기능을 사용할 수 있습니다.
>* 새로운 기능은 프로덕션에서 제공되기 전에 사용자 지정 새로 고침 샌드박스에 도입되지 않습니다.
>
>  또한 Preview 샌드박스에 필요하지 않은 Custom Refresh 샌드박스를 얻는 추가 비용이 있습니다.
>
>  미리 보기 샌드박스에 대한 자세한 내용은 [미리 보기 샌드박스 환경 [!DNL Adobe Workfront] 을 참조하십시오.](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 패키지</td> 
   <td> <p>Prime 또는 Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Workfront 라이선스</td> 
   <td> <p>표준</p><p>플랜</p>  </td> 
  </tr> 
  </tr>
   <tr>
   <td>액세스 수준 구성
   </td>
   <td><p>Workfront 관리자여야 합니다.</p>
   </td>
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 새로 고침 샌드박스 새로 고침

사용자 정의 새로 고침 샌드박스에는 실제 프로덕션 데이터가 포함되어 있으며 이를 예약하기 전까지 새로 고쳐지지 않습니다. 언제든지 편리하게 일주일에 한 번처럼 자주 새로 고침을 예약할 수 있습니다.

>[!NOTE]
>
>* 현재 날짜의 새로 고침을 예약할 수 없습니다. 예를 들어 오늘이 6월 1일인 경우 새로 고침을 예약할 수 있는 가장 빠른 날은 6월 2일입니다.
>* 예약된 새로 고침은 사용자의 클러스터(미국의 경우 야간 미국 클러스터 새로 고침)를 기반으로 야간 중에 발생합니다. 특정 시간은 큐에 있는 다른 고객과 새로 고친 데이터의 양 때문에 예측할 수 없습니다. 큐에 많은 대형 고객이 있는 경우, 해당 날짜 후반이나 다음 날까지 새로 고침이 실행되지 않을 수 있습니다.
>* 사용자 정의 새로 고침 샌드박스는 항상 프로덕션 환경과 동일한 제품 기능을 갖습니다. 그러나 사용자 지정 새로 고침 샌드박스를 새로 고칠 때 로그인 화면 배경색에 대해서만 브랜딩이 유지됩니다. 로그인 화면과 탐색 막대 로고가 [!DNL Workfront] 기본값으로 재설정되며 새로 고침 전에 수정한 브랜딩 이미지는 표시되지 않습니다.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 프로덕션 환경에서 사용자 정의 새로 고침 샌드박스에 액세스 {#access-the-custom-refresh-sandbox-from-your-production-environment}

[!DNL Workfront] 관리자는 프로덕션 환경에서 사용자 지정 새로 고침 샌드박스에 액세스할 수 있습니다.

>[!NOTE]
>
>계정이 클러스터 4(EMEA 클러스터)에 있는 경우 프로덕션 환경에서 사용자 정의 새로 고침 샌드박스에 액세스할 수 없습니다. Cluster 4에 계정이 있을 때 사용자 정의 새로 고침 샌드박스에 액세스하는 방법에 대한 자세한 내용은 [Cluster 4의 계정에 대한 사용자 정의 새로 고침 샌드박스 액세스(EMEA 계정)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Cluster 4의 계정에 대한 사용자 정의 새로 고침 샌드박스 액세스(EMEA 계정)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)를 참조하십시오.

사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. **[!UICONTROL 의 오른쪽 상단에 있는]**&#x200B;주 메뉴![&#x200B; 아이콘 &#x200B;](assets/main-menu-icon.png)주 메뉴 아이콘[!DNL Adobe Workfront]을 클릭한 다음 **[!UICONTROL 설정]** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.

1. **[!UICONTROL 시스템]** >**[!UICONTROL 환경 설정]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 테스트 환경]** 섹션에서 **[!UICONTROL 샌드박스 1]** 또는 **[!UICONTROL 샌드박스 2]**&#x200B;을(를) 클릭합니다.

   지원 패키지는 하나 또는 두 개의 사용자 정의 새로 고침 샌드박스에 액세스할 수 있는지 여부를 지정합니다.

1. 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.

   사용자 정의 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않는 한, 사용자 정의 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.

   사용자 정의 새로 고침 샌드박스는 화면 상단의 배너에 버전과 마지막 새로 고침 날짜를 표시합니다. 프로덕션의 모든 정보를 사용할 수 있으며 새로 고침이 완료된 후 작업할 준비가 되었습니다.

## URL을 사용하여 사용자 정의 새로 고침 샌드박스에 액세스 {#access-the-custom-refresh-sandbox-using-a-url}

모든 사용자는 URL을 사용하여 사용자 정의 새로 고침 샌드박스에 액세스할 수 있습니다.

* [클러스터 1, 2, 3 및 5의 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [클러스터 4(EMEA 계정)의 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### 클러스터 1, 2, 3 및 5의 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

지원 패키지에 따라 하나 또는 두 개의 사용자 정의 새로 고침 샌드박스에 액세스할 수 있어야 합니다.

URL을 사용하여 사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. 사용자 정의 새로 고침 샌드박스가 하나만 있는 경우 이 URL로 이동합니다.

   `https://companyname.sb01.workfront.com`(이전 URL:`https://cr1.attasksandbox.com/`.)

   또는 위의 URL 외에 두 개의 사용자 정의 새로 고침 샌드박스가 있는 경우 다음 URL로 이동하여 두 번째 사용자 정의 새로 고침 샌드박스에 액세스할 수도 있습니다.

   `https://companyname.sb02.workfront.com`(이전 URL:`https://cr2.attasksandbox.com/`)

1. 로그인 화면에서 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.
1. 사용자 정의 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않는 한, 사용자 정의 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.

### 클러스터 4(EMEA 계정)의 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스 {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

[!DNL Workfront] 계정이 클러스터 4(EMEA 클러스터)에 있는 경우 URL만 사용하여 사용자 지정 새로 고침 샌드박스에 액세스할 수 있습니다. 계정이 속한 클러스터를 확인하려면 고객 지원 팀에 문의하십시오.

지원 패키지에 따라 하나 또는 두 개의 사용자 정의 새로 고침 샌드박스에 액세스할 수 있어야 합니다.

URL을 사용하여 사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. 사용자 정의 새로 고침 샌드박스가 하나만 있는 경우 이 URL로 이동합니다.

   `https://companyname.sb01.workfront.com`(이전 URL:`https://cr3.attasksandbox.com`)

   또는

   사용자 지정 새로 고침 샌드박스가 두 개 있는 경우 다음 URL 중 하나로 이동합니다.

   `https://companyname.sb01.workfront.com`(이전 URL:`https://cr3.attasksandbox.com`)

   `https://companyname.sb02.workfront.com`(이전 URL:`https://cr4.attasksandbox.com`)

1. 로그인 화면에서 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.

   사용자 정의 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않는 한, 사용자 정의 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.

## 사용자 지정 새로 고침 샌드박스 새로 고침 예약

>[!IMPORTANT]
>
>새로 고침 기간은 새로 고치는 데이터의 크기에 따라 다릅니다. 새로 고침 프로세스 중에 사용자 정의 새로 고침 샌드박스 환경이 API 호출 및 통합 등 어떤 식으로든 사용되고 있지 않으면 샌드박스 새로 고침이 성공적으로 완료되지 않을 수 있습니다. [!DNL Workfront]은(는) 시작하기 전에 사용자 지정 새로 고침 샌드박스 환경을 비활성화하지만 샌드박스 새로 고침이 성공했는지 확인하려면 모든 활성 세션을 종료해야 합니다.

사용자 지정 새로 고침 샌드박스의 새로 고침을 예약한 후 페이지 상단의 [!UICONTROL 취소]를 클릭하여 취소할 수 있습니다. 나중에 다시 예약할 수도 있습니다.

>[!NOTE]
>
>자동 샌드박스 새로 고침을 예약할 수 없습니다.

고객 새로 고침 샌드박스의 새로 고침을 예약하려면:

1. 사용자 지정 새로 고침 샌드박스에 로그인합니다.
1. 화면 상단의 배너에서 **[!UICONTROL 일정]**&#x200B;을 클릭하고 달력에서 날짜를 선택합니다.
1. 새로 고침을 수행할 날짜를 선택한 다음 **[!UICONTROL 새로 고침 예약]**&#x200B;을 클릭하세요.

## 사용자 지정 새로 고침 샌드박스에서 프로덕션으로 전환

1. 사용자 지정 새로 고침 샌드박스에 로그인합니다.

   사용자 지정 새로 고침 샌드박스에 액세스하는 방법에 대한 자세한 내용은 [프로덕션 환경에서 사용자 지정 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-from-your-production-environment) 또는 [URL을 사용하여 사용자 지정 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-using-a-url)를 참조하십시오.

1. 화면 상단의 배너에서 **[!UICONTROL 프로덕션으로 이동]**&#x200B;을 클릭합니다.

   데이터 전송은 단방향이고 프로덕션에서 사용자 지정 새로 고침 샌드박스로 전송되며 그 반대는 아니므로 샌드박스에서 수행된 작업이 [!UICONTROL production] 환경에 표시되지 않습니다.

## 사용자 정의 새로 고침 샌드박스에서 이메일 수신

[!DNL Workfront]은(는) 사용자 지정 새로 고침 샌드박스 환경에서 모든 전자 메일 통신을 사용하지 않도록 설정합니다. 사용자 지정 새로 고침 샌드박스 환경에서 이메일 알림을 수신하려면 사용자 설정에서 이 기능을 활성화해야 합니다. 사용자 지정 새로 고침 샌드박스 환경에서 전자 메일 알림을 사용하는 방법에 대한 자세한 내용은 [미리 보기 샌드박스 환경에서 전자 메일 배달 사용](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)을 참조하십시오.

>[!NOTE]
>
>모바일 앱의 보고서 배달 및 푸시 알림은 사용자 지정 새로 고침 샌드박스 환경에 대해 항상 비활성화됩니다. [사용자 지정 새로 고침 샌드박스] 환경에 액세스할 때 사용자와 [!DNL Workfront] 관리자 모두 모바일 앱에 대해 보고서 배달이나 푸시 알림을 활성화할 수 없습니다.\
>프로덕션 환경의 보고서 게재에 대한 자세한 내용은 [보고서 게재 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하십시오. 프로덕션 환경의 모바일 앱에서 푸시 알림에 대한 자세한 내용은 의 섹션을 참조하십시오.

## 사용자 지정 새로 고침 샌드박스에서 Single Sign-On 구성

단일 사인온 솔루션에서 작동하도록 사용자 지정 새로 고침 샌드박스를 구성하려면 프로덕션 환경과 별도로 구성하여 이 작업을 수행할 수 있습니다. 사용자 정의 새로 고침 샌드박스의 SSO 구성은 프로덕션 환경의 SSO 구성과 독립적입니다.\
사용자 정의 새로 고침 샌드박스를 새로 고칠 때 SSO 정보는 프로덕션 환경에서 복사되어 사용자 정의 새로 고침 샌드박스 구성을 덮어쓰지 않습니다.

사용자 지정 새로 고침 샌드박스에서 SSO(Single Sign-On)를 구성하는 단계는 프로덕션 환경에서 구성하는 단계와 유사합니다.\
SSO를 사용하여 [!DNL Workfront]을(를) 구성하는 방법에 대한 자세한 내용은 [Adobe Workfront의 Single Sign-On 개요](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)를 참조하십시오.

>[!NOTE]
>
>조직의 [!DNL Workfront] 인스턴스가 Adobe IMS에서 활성화된 경우에는 사용할 수 없습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

## 프로젝트 타임라인 자동 재계산

타임라인을 다시 계산하면 관리자는 프로젝트 외부의 힘이 프로젝트의 타임라인에 미치는 영향을 확인할 수 있습니다. 프로젝트의 타임라인은 프로젝트의 계획된 일자와 예상 일자를 나타냅니다.

Workfront 관리자는 Workfront이 프로젝트 타임라인을 자동으로 다시 계산하는 시기를 구성할 수 있습니다. Workfront은 매일 밤, 프로젝트 범위가 변경될 때 또는 둘 다 프로젝트 타임라인을 다시 계산할 수 있습니다.

자세한 내용은 [프로젝트에 대한 타임라인 다시 계산 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)을 참조하십시오.

사용자 정의 샌드박스 새로 고침 환경의 경우 야간 다시 계산이 비활성화되고 프로젝트 타임라인이 자동으로 다시 계산되지 않습니다. 사용자 지정 새로 고침 샌드박스 환경에 대한 프로젝트 타임라인을 수동으로 다시 계산해야 합니다. 자세한 내용은 [프로젝트 타임라인 다시 계산](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md)을 참조하십시오.


## 의도한 사용 및 가용성

* [!DNL Workfront] 사용자 지정 새로 고침 샌드박스 환경은 성능 또는 로드 테스트용이 아닙니다. 대신 이러한 환경을 사용하여 조직의 기존 워크플로우로 기능 기능을 검증할 수 있습니다.

* 문서와 관련된 워크플로우는 로드 테스트가 아닌 프로세스에 중점을 두어야 합니다. 샌드박스 환경에서는 큰 파일이 지원되지 않습니다.

* [!DNL Workfront] 사용자 지정 새로 고침 샌드박스 환경은 항상 사용할 수 있도록 되어 있습니다. 정규 업무 시간 동안 Workfront 사용자 정의 새로 고침 샌드박스 환경의 중단은 프로덕션 문제가 해결된 후 즉시 최우선 순위가 됩니다(존재하는 경우). 주말(토요일 및 일요일)에 발생한 Workfront 사용자 정의 새로 고침 샌드박스 환경의 중단은 월요일 업무 시간 동안 환경이 실행되도록 처리됩니다.

* 사용자 정의 새로 고침 샌드박스 환경에서는 증명을 사용할 수 없습니다.

* 다음 알림은 사용자 정의 새로 고침 샌드박스 환경에서 사용할 수 없습니다.

   * 미리 알림
   * 자동 지연 또는 조기 미리 알림
