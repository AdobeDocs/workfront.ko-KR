---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 다음 [!DNL Adobe Workfront] 사용자 정의 샌드박스 환경 새로 고침
description: 사용자 지정 새로 고침 샌드박스는 프로덕션 환경의 데이터를 사용하여 테스트하고 작업할 수 있는 환경입니다. 또한 교육을 실행하고 설정 기능을 결정하는 데에도 이상적입니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 0e2c529e61ed1c9c85dbd826029cf64346f865ff
workflow-type: tm+mt
source-wordcount: '1555'
ht-degree: 0%

---

# 다음 [!DNL Adobe Workfront] 사용자 정의 샌드박스 환경 새로 고침

사용자 지정 새로 고침 샌드박스는 프로덕션 환경의 데이터를 사용하여 테스트하고 작업할 수 있는 환경입니다. 또한 교육을 실행하고 설정 기능을 결정하는 데에도 이상적입니다.

>[!NOTE]
>
>이는 를 복제하는 테스트 환경이기도 한 미리보기 샌드박스와는 다릅니다 [!DNL Workfront] 프로덕션 환경.
>
>* 프로덕션 환경에서는 미리보기 샌드박스에 새로운 기능을 사용할 수 있습니다.
>* 새로운 기능은 프로덕션에서 제공되기 전에 사용자 지정 새로 고침 샌드박스에 도입되지 않습니다.
>
>  또한 Preview 샌드박스에 필요하지 않은 Custom Refresh 샌드박스를 얻는 추가 비용이 있습니다.
>
>  미리보기 샌드박스에 대한 자세한 내용은 [다음 [!DNL Adobe Workfront] 샌드박스 환경 미리보기](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 플랜</td> 
   <td> <p>[!UICONTROL Business] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 라이센스</p> </td> 
   <td> <p>[!UICONTROL 계획] </p> <p>다음이어야 합니다: [!DNL Workfront] 관리자. 다음에 대한 정보: [!DNL Workfront] 관리자, 참조 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">지원 패키지</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] 또는 [!UICONTROL Enterprise]</p> <p>표준 지원 패키지는 사용자 정의 새로 고침 샌드박스에 액세스할 수 없지만 미리보기 샌드박스에 액세스할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 정의 새로 고침 샌드박스 새로 고침

사용자 정의 새로 고침 샌드박스에는 실제 프로덕션 데이터가 포함되어 있으며 이를 예약하기 전까지 새로 고쳐지지 않습니다. 언제든지 편리하게 일주일에 한 번처럼 자주 새로 고침을 예약할 수 있습니다.

>[!NOTE]
>
>* 현재 날짜의 새로 고침을 예약할 수 없습니다. 예를 들어 오늘이 6월 1일인 경우 새로 고침을 예약할 수 있는 가장 빠른 날은 6월 2일입니다.
>* 예약된 새로 고침은 요청을 제출한 사용자의 시간대를 기준으로 지정된 날짜의 오전 12시에 수행됩니다.
>* 사용자 정의 새로 고침 샌드박스는 항상 프로덕션 환경과 동일한 제품 기능을 갖습니다. 그러나 사용자 지정 새로 고침 샌드박스를 새로 고칠 때 로그인 화면 배경색에 대해서만 브랜딩이 유지됩니다. 로그인 화면 및 탐색 막대 로고가 로 재설정됩니다. [!DNL Workfront] 기본값과 새로 고침 전에 수정한 브랜딩 이미지는 표시되지 않습니다.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 프로덕션 환경에서 사용자 정의 새로 고침 샌드박스에 액세스 {#access-the-custom-refresh-sandbox-from-your-production-environment}

로서의 [!DNL Workfront] 관리자는 프로덕션 환경에서 사용자 정의 샌드박스 새로 고침에 액세스할 수 있습니다.

>[!NOTE]
>
>계정이 클러스터 4(EMEA 클러스터)에 있는 경우 프로덕션 환경에서 사용자 정의 새로 고침 샌드박스에 액세스할 수 없습니다. 클러스터 4에 계정이 있을 때 사용자 지정 새로 고침 샌드박스에 액세스하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [클러스터 4(EMEA 계정)의 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [클러스터 4(EMEA 계정)의 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 시스템]** >**[!UICONTROL 환경 설정]**.

1. 다음에서 **[!UICONTROL 테스트 환경]** 섹션, 클릭 **[!UICONTROL 샌드박스 1]** 또는 **[!UICONTROL 샌드박스 2]**.

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

   https://companyname.sb01.workfront.com (이전 URL:https://cr1.attasksandbox.com/.)

   또는 위의 URL 외에 두 개의 사용자 정의 새로 고침 샌드박스가 있는 경우 다음 URL로 이동하여 두 번째 사용자 정의 새로 고침 샌드박스에 액세스할 수도 있습니다.

   https://companyname.sb02.workfront.com (이전 URL:https://cr2.attasksandbox.com/)

1. 로그인 화면에서 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.
1. 사용자 정의 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않는 한, 사용자 정의 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.

### 클러스터 4(EMEA 계정)의 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스 {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

다음의 경우 [!DNL Workfront] 계정이 클러스터 4(EMEA 클러스터)에 있으므로 URL을 사용해야만 사용자 지정 새로 고침 샌드박스에 액세스할 수 있습니다. 계정이 속한 클러스터를 확인하려면 고객 지원 팀에 문의하십시오.

지원 패키지에 따라 하나 또는 두 개의 사용자 정의 새로 고침 샌드박스에 액세스할 수 있어야 합니다.

URL을 사용하여 사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. 사용자 정의 새로 고침 샌드박스가 하나만 있는 경우 이 URL로 이동합니다.

   https://companyname.sb01.workfront.com (이전 URL:https://cr3.attasksandbox.com)

   또는

   사용자 지정 새로 고침 샌드박스가 두 개 있는 경우 다음 URL 중 하나로 이동합니다.

   https://companyname.sb01.workfront.com (이전 URL:https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (이전 URL:https://cr4.attasksandbox.com)

1. 로그인 화면에서 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.

   사용자 정의 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않는 한, 사용자 정의 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.

## 사용자 지정 새로 고침 샌드박스 새로 고침 예약

>[!IMPORTANT]
>
>새로 고침 기간은 새로 고치는 데이터의 크기에 따라 다릅니다. 새로 고침 프로세스 중에 사용자 정의 새로 고침 샌드박스 환경이 API 호출 및 통합 등 어떤 식으로든 사용되고 있지 않으면 샌드박스 새로 고침이 성공적으로 완료되지 않을 수 있습니다. [!DNL Workfront] 샌드박스 새로 고침이 시작되기 전에 사용자 정의 샌드박스 환경을 비활성화하지만 활성 세션을 종료하여 샌드박스 새로 고침이 성공했는지 확인해야 합니다.

사용자 정의 새로 고침 샌드박스의 새로 고침을 예약한 후 다음을 클릭하여 취소할 수 있습니다. [!UICONTROL 취소] 을 클릭합니다. 나중에 다시 예약할 수도 있습니다.

>[!NOTE]
>
>자동 샌드박스 새로 고침을 예약할 수 없습니다.

고객 새로 고침 샌드박스의 새로 고침을 예약하려면:

1. 사용자 지정 새로 고침 샌드박스에 로그인합니다.
1. 클릭 **[!UICONTROL 예약]** 화면 상단의 배너에서 달력에서 날짜를 선택합니다.
1. 새로 고침을 수행할 날짜를 선택한 다음 을 클릭합니다. **[!UICONTROL 새로 고침 예약]**.

## 사용자 지정 새로 고침 샌드박스에서 프로덕션으로 전환

1. 사용자 지정 새로 고침 샌드박스에 로그인합니다.

   사용자 지정 새로 고침 샌드박스에 액세스하는 방법에 대한 자세한 내용은 [프로덕션 환경에서 사용자 정의 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-from-your-production-environment) 또는 [URL을 사용하여 사용자 정의 새로 고침 샌드박스에 액세스](#access-the-custom-refresh-sandbox-using-a-url).

1. 클릭 **[!UICONTROL 프로덕션으로 이동]** 를 클릭합니다.

   샌드박스에서 수행된 작업은 [!UICONTROL production] 환경은 프로덕션에서 사용자 정의 새로 고침 샌드박스로 단일 방식으로 데이터를 전송하고 반대 방향으로는 전송하지 않습니다.

## 사용자 정의 새로 고침 샌드박스에서 이메일 수신

[!DNL Workfront] 사용자 지정 새로 고침 샌드박스 환경에서 모든 이메일 통신을 비활성화합니다. 사용자 지정 새로 고침 샌드박스 환경에서 이메일 알림을 수신하려면 사용자 설정에서 이 기능을 활성화해야 합니다. 사용자 지정 새로 고침 샌드박스 환경에서 이메일 알림을 활성화하는 방법에 대한 자세한 내용은 [미리보기 샌드박스 환경에서 이메일 게재 활성화](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>모바일 앱의 보고서 배달 및 푸시 알림은 사용자 지정 새로 고침 샌드박스 환경에 대해 항상 비활성화됩니다. 너도, 너도 [!DNL Workfront] 사용자 지정 새로 고침 샌드박스 환경에 액세스하면 관리자가 모바일 앱에 대해 보고서 배달 또는 푸시 알림을 활성화할 수 있습니다.\
>프로덕션 환경의 보고서 게재에 대한 자세한 내용은 [보고서 게재 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).프로덕션 환경용 모바일 앱의 푸시 알림에 대한 자세한 내용은 의 섹션을 참조하십시오.

## 사용자 지정 새로 고침 샌드박스에서 Single Sign-On 구성

단일 사인온 솔루션에서 작동하도록 사용자 지정 새로 고침 샌드박스를 구성하려면 프로덕션 환경과 별도로 구성하여 이 작업을 수행할 수 있습니다. 사용자 정의 새로 고침 샌드박스의 SSO 구성은 프로덕션 환경의 SSO 구성과 독립적입니다.\
사용자 정의 새로 고침 샌드박스를 새로 고칠 때 SSO 정보는 프로덕션 환경에서 복사되어 사용자 정의 새로 고침 샌드박스 구성을 덮어쓰지 않습니다.

사용자 지정 새로 고침 샌드박스에서 SSO(Single Sign-On)를 구성하는 단계는 프로덕션 환경에서 구성하는 단계와 유사합니다.\
구성에 대한 자세한 내용 [!DNL Workfront] sso를 사용하여 다음을 참조하십시오. [Adobe Workfront의 Single Sign-On 개요](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>조직의 경우 사용할 수 없습니다. [!DNL Workfront] 인스턴스가 Adobe IMS에서 활성화됩니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

## 의도한 사용 및 가용성

[!DNL Workfront] 사용자 정의 새로 고침 샌드박스 환경은 성능 또는 로드 테스트를 위한 것이 아닙니다. 대신 이러한 환경을 사용하여 조직의 기존 워크플로우로 기능 기능을 검증할 수 있습니다.

[!DNL Workfront] 사용자 정의 새로 고침 샌드박스 환경은 항상 사용할 수 있도록 설계되었습니다. 정규 업무 시간 동안 Workfront 사용자 정의 새로 고침 샌드박스 환경의 중단은 프로덕션 문제가 해결된 후 즉시 최우선 순위가 됩니다(존재하는 경우). 주말(토요일 및 일요일)에 발생한 Workfront 사용자 정의 새로 고침 샌드박스 환경의 중단은 월요일 업무 시간 동안 환경이 실행되도록 처리됩니다.
