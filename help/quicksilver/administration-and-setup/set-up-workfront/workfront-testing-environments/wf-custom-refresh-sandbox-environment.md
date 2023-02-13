---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 다음 [!DNL Adobe Workfront] 사용자 지정 새로 고침 샌드박스 환경
description: 사용자 지정 새로 고침 샌드박스는 프로덕션 환경의 데이터를 사용하여 테스트하고 작업할 수 있는 환경입니다. 교육 실행 및 설치 기능 결정에 이상적입니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# 다음 [!DNL Adobe Workfront] 사용자 지정 새로 고침 샌드박스 환경

사용자 지정 새로 고침 샌드박스는 프로덕션 환경의 데이터를 사용하여 테스트하고 작업할 수 있는 환경입니다. 교육 실행 및 설치 기능 결정에 이상적입니다.

>[!NOTE]
>
>이 기능은 미리 보기 샌드박스와 다릅니다. 미리 보기 샌드박스는 [!DNL Workfront] 프로덕션 환경입니다.
>
>* 새로운 기능은 프로덕션에서 사용하기 전에 미리 보기 샌드박스에 도입되었습니다.
>* 새 기능은 프로덕션에서 사용 가능하기 전에 사용자 지정 새로 고침 샌드박스에 소개되지 않습니다.
>
>  또한 미리 보기 샌드박스에 필요하지 않은 사용자 지정 새로 고침 샌드박스를 획득하는 데 추가 비용이 있습니다.
>
>  미리 보기 샌드박스에 대한 자세한 내용은 [다음 [!DNL Adobe Workfront] 샌드박스 환경 미리 보기](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


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
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 라이선스</p> </td> 
   <td> <p>[!UICONTROL 계획] </p> <p>넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">지원 패키지</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] 또는 [!UICONTROL Enterprise]</p> <p>표준 지원 패키지는 사용자 지정 새로 고침 샌드박스에 액세스할 수 없지만 미리 보기 샌드박스에 액세스할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 지정 새로 고침 샌드박스 새로 고침

사용자 지정 새로 고침 샌드박스에는 실제 프로덕션 데이터가 포함되어 있으며, 그렇게 하도록 예약하기 전까지 새로 고쳐지지 않습니다. 일주일에 한 번, 자주, 편리한 시간에 새로 고침을 예약할 수 있습니다.

>[!NOTE]
>
>* 현재 날짜에 대해 새로 고침을 예약할 수 없습니다. 예를 들어, 오늘이 6월 1일인 경우 새로 고침을 예약할 수 있는 가장 빠른 날은 6월 2일입니다.
>* 사용자 지정 새로 고침 샌드박스에는 항상 프로덕션 환경과 동일한 제품 기능이 있습니다. 그러나 사용자 지정 새로 고침 샌드박스를 새로 고치면 로그인 화면 배경색에만 브랜딩이 유지됩니다. 로그인 화면 및 탐색 막대 로고는 로 재설정됩니다. [!DNL Workfront] 기본값과 새로 고침 전에 수정한 브랜딩 이미지가 표시되지 않습니다.
>




<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 프로덕션 환경에서 사용자 지정 새로 고침 샌드박스 액세스 {#access-the-custom-refresh-sandbox-from-your-production-environment}

로서의 [!DNL Workfront] 관리자는 프로덕션 환경에서 사용자 지정 새로 고침 샌드박스에 액세스할 수 있습니다.

>[!NOTE]
>
>계정이 클러스터 4(EMEA 클러스터)에 있는 경우 프로덕션 환경에서 사용자 지정 새로 고침 샌드박스에 액세스할 수 없습니다. 클러스터 4에 계정이 있을 때 사용자 지정 새로 고침 샌드박스에 액세스할 수 있는 방법에 대한 자세한 내용은 [클러스터 4의 계정에 대한 사용자 지정 새로 고침 샌드박스 액세스(EMEA 계정)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [클러스터 4의 계정에 대한 사용자 지정 새로 고침 샌드박스 액세스(EMEA 계정)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 시스템]** >**[!UICONTROL 기본 설정]**.

1. 에서 **[!UICONTROL 테스트 환경]** 섹션을 클릭합니다. **[!UICONTROL 샌드박스 1]** 또는 **[!UICONTROL 샌드박스 2]**.

   지원 패키지는 사용자 지정 새로 고침 샌드박스에 액세스할 수 있는지 또는 두 개의 사용자 지정 새로 고침 샌드박스에 액세스할 수 있는지를 지정합니다.

1. 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.

   사용자 지정 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않은 한, 사용자 지정 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 로그인은 새로 고침이 발생하는 경우에만 동기화됩니다. 자동으로 동기화되지 않습니다.

   사용자 지정 새로 고침 샌드박스는 화면 상단의 배너에 버전 및 마지막 새로 고침 날짜를 표시합니다. 프로덕션의 모든 정보를 사용할 수 있으며 새로 고침이 완료된 후 작업할 준비가 되었습니다.

## URL을 사용하여 사용자 지정 새로 고침 샌드박스 액세스 {#access-the-custom-refresh-sandbox-using-a-url}

모든 사용자는 URL을 사용하여 사용자 지정 새로 고침 샌드박스에 액세스할 수 있습니다.

* [클러스터 1,2,3 및 5에서 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스합니다](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [클러스터 4의 계정에 대한 사용자 지정 새로 고침 샌드박스 액세스(EMEA 계정)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### 클러스터 1,2,3 및 5에서 계정에 대한 사용자 정의 새로 고침 샌드박스에 액세스합니다 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

지원 패키지에 따라 하나 또는 두 개의 사용자 지정 새로 고침 샌드박스에 액세스할 수 있어야 합니다.

URL을 사용하여 사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. 사용자 지정 새로 고침 샌드박스가 하나만 있는 경우 이 URL로 이동합니다.

   https://companyname.sb01.workfront.com (이전 URL):https://cr1.attasksandbox.com/.)

   또는 위의 URL 외에도 두 개의 사용자 지정 새로 고침 샌드박스가 있는 경우 다음 URL로 이동하여 두 번째 사용자 지정 새로 고침 샌드박스에 액세스할 수도 있습니다.

   https://companyname.sb02.workfront.com (이전 URL):https://cr2.attasksandbox.com/)

1. 로그인 화면에서 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.
1. 사용자 지정 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않은 한, 사용자 지정 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 로그인은 새로 고침이 발생하는 경우에만 동기화됩니다. 자동으로 동기화되지 않습니다.

### 클러스터 4의 계정에 대한 사용자 지정 새로 고침 샌드박스 액세스(EMEA 계정) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

만약 [!DNL Workfront] 계정이 클러스터 4(EMEA 클러스터)에 있는 경우 URL만 사용하여 사용자 지정 새로 고침 샌드박스에 액세스할 수 있습니다. 계정이 켜져 있는 클러스터를 확인하려면 고객 지원 팀에 문의하십시오.

지원 패키지에 따라 하나 또는 두 개의 사용자 지정 새로 고침 샌드박스에 액세스할 수 있어야 합니다.

URL을 사용하여 사용자 지정 새로 고침 샌드박스에 액세스하려면:

1. 사용자 지정 새로 고침 샌드박스가 하나만 있는 경우 이 URL로 이동합니다.

   https://companyname.sb01.workfront.com (이전 URL):https://cr3.attasksandbox.com)

   또는

   두 개의 사용자 지정 새로 고침 샌드박스가 있는 경우 다음 URL 중 하나로 이동합니다.

   https://companyname.sb01.workfront.com (이전 URL):https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (이전 URL):https://cr4.attasksandbox.com)

1. 로그인 화면에서 사용자 지정 새로 고침 샌드박스 자격 증명을 사용하여 로그인합니다.

   사용자 지정 새로 고침 샌드박스를 마지막으로 새로 고친 후 프로덕션 자격 증명을 변경하지 않은 한, 사용자 지정 새로 고침 샌드박스 자격 증명은 프로덕션 자격 증명과 동일합니다. 로그인은 새로 고침이 발생하는 경우에만 동기화됩니다. 자동으로 동기화되지 않습니다.

## 사용자 지정 새로 고침 샌드박스의 새로 고침 예약

>[!IMPORTANT]
>
>새로 고침 기간은 새로 고치는 데이터의 크기에 따라 달라집니다. 새로 고침 프로세스 중에 사용자 지정 새로 고침 샌드박스 환경이 어떤 식으로든(API 호출 및 통합 포함)에서 사용되지 않는 것이 중요합니다. 이렇게 하면 샌드박스 새로 고침이 성공적으로 완료되지 않습니다. [!DNL Workfront] 은 시작하기 전에 사용자 지정 새로 고침 샌드박스 환경을 비활성화하지만, 샌드박스 새로 고침이 성공했는지 확인하려면 활성 세션을 종료해야 합니다.

사용자 지정 새로 고침 샌드박스의 새로 고침을 예약한 후 을 클릭하여 취소할 수 있습니다 [!UICONTROL 취소] 를 클릭합니다. 나중에 다시 예약할 수도 있습니다

>[!NOTE]
>
>자동 샌드박스 새로 고침을 예약할 수 없습니다.

고객 새로 고침 샌드박스의 새로 고침을 예약하려면:

1. 사용자 지정 새로 고침 샌드박스에 로그인합니다.
1. 클릭 **[!UICONTROL 예약]** 화면 상단의 배너에서 달력에서 날짜를 선택합니다.
1. 새로 고침이 발생할 날짜를 선택한 다음 **[!UICONTROL 예약 새로 고침]**.

## 사용자 지정 새로 고침 샌드박스에서 프로덕션으로 전환

1. 사용자 지정 새로 고침 샌드박스에 로그인합니다.

   사용자 지정 새로 고침 샌드박스 액세스에 대한 자세한 내용은 [프로덕션 환경에서 사용자 지정 새로 고침 샌드박스 액세스](#access-the-custom-refresh-sandbox-from-your-production-environment) 또는 [URL을 사용하여 사용자 지정 새로 고침 샌드박스 액세스](#access-the-custom-refresh-sandbox-using-a-url).

1. 클릭 **[!UICONTROL 프로덕션으로 이동]** 화면 상단의 배너에 있습니다.

   샌드박스에서 수행된 작업이 [!UICONTROL production] 환경은 데이터 전송이 단방향이므로 생성에서 사용자 지정 새로 고침 샌드박스로 전송되고 역방향으로 전송되지 않습니다.

## 사용자 지정 새로 고침 샌드박스에서 이메일 수신

[!DNL Workfront] 사용자 지정 새로 고침 샌드박스 환경에서 모든 이메일 통신을 비활성화합니다. 사용자 지정 새로 고침 샌드박스 환경에서 이메일 알림을 수신하려면 사용자 설정에서 이 기능을 활성화해야 합니다. 사용자 지정 새로 고침 샌드박스 환경에서 전자 메일 알림을 활성화하는 방법에 대한 자세한 내용은 [미리 보기 샌드박스 환경에서 전자 메일 게재 활성화](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>모바일 앱의 보고서 전달 및 푸시 알림은 항상 사용자 지정 새로 고침 샌드박스 환경에 대해 비활성화됩니다. 너도 아니고 [!DNL Workfront] 관리자는 사용자 지정 새로 고침 샌드박스 환경에 액세스할 때 모바일 앱에 대한 보고서 전달 또는 푸시 알림을 활성화할 수 있습니다.\
>프로덕션 환경을 위한 보고서 게재에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)프로덕션 환경용 모바일 앱의 푸시 알림에 대한 자세한 내용은 의 섹션을 참조하십시오.

## 사용자 지정 새로 고침 샌드박스에서 단일 사인온 구성

단일 사인온 솔루션에서 작동하도록 사용자 지정 새로 고침 샌드박스를 구성하려면 프로덕션 환경과 별도로 구성하여 이 작업을 수행할 수 있습니다. 사용자 지정 새로 고침 샌드박스의 SSO 구성은 프로덕션 환경의 SSO 구성과 독립적입니다.\
사용자 지정 새로 고침 샌드박스를 새로 고치면 SSO 정보가 프로덕션 환경에서 복사되지 않아 사용자 지정 새로 고침 샌드박스 구성을 덮어씁니다.

사용자 지정 새로 고침 샌드박스에서 단일 사인온을 구성하는 단계는 프로덕션 환경에서 구성하는 단계와 유사합니다.\
구성에 대한 자세한 정보 [!DNL Workfront] SSO를 사용하는 경우 [Adobe Workfront의 단일 사인온 개요](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>조직의 [!DNL Workfront] Adobe IMS에서 인스턴스를 사용할 수 있습니다. 자세한 내용은 네트워크 또는 IT 관리자에게 문의하십시오.

## 사용 목적 및 가용성

[!DNL Workfront] 사용자 지정 새로 고침 샌드박스 환경은 성능 또는 로드 테스트를 위한 것이 아닙니다. 대신 이러한 환경을 사용하여 조직의 기존 워크플로우를 통해 기능 기능을 확인합니다.

[!DNL Workfront] 사용자 지정 새로 고침 샌드박스 환경은 항상 사용할 수 있도록 되어 있습니다. 운영 문제가 있는 경우 해결된 즉시 일반 업무 시간 동안 Workfront 사용자 지정 새로 고침 샌드박스 환경에 대한 중단이 가장 우선 순위가 됩니다. 주말(토요일 및 일요일)에 Workfront 사용자 지정 새로 고침 샌드박스 환경에 대한 모든 중단은 월요일의 영업시간 동안 환경이 실행되도록 전달됩니다.
