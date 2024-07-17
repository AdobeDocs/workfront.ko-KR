---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ' [!DNL Adobe Workfront] 샌드박스 환경 미리 보기'
description: 미리보기 샌드박스는 라이브 환경의 복제본 역할을 하는 테스트 환경입니다. 그것은 Workfront에 의해 매 주말마다 새로 고쳐집니다. 금요일에 라이브 환경에 추가된 데이터는 다음 월요일까지 미리보기 샌드박스에 표시됩니다. 모든 지원 패키지는 이 샌드박스에 액세스할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# [!DNL Adobe Workfront] 미리 보기 샌드박스 환경

<!-- Audited: 12/2023 -->

[!DNL Workfront] 프로덕션 환경의 복제본인 [!DNL Workfront]에 대한 두 가지 테스트 환경이 있습니다.

* 미리보기 샌드박스

  미리 보기 샌드박스는 라이브 환경의 복제본 역할을 하는 테스트 환경이며 매주 주말마다 [!DNL Workfront]에 의해 새로 고쳐집니다. 금요일에 라이브 환경에 추가된 데이터는 다음 월요일까지 미리보기 샌드박스에 표시됩니다.

  모든 지원 패키지는 미리보기 샌드박스에 액세스할 수 있습니다.

* 사용자 정의 새로 고침 샌드박스

  사용자 지정 새로 고침 샌드박스는 사용자가 수동으로 새로 고치는 별도의 테스트 환경입니다. 사용자 지정 새로 고침 샌드박스를 얻는 데 추가 비용이 있습니다. 이 환경에 대한 자세한 내용은 [사용자 지정 샌드박스 환경 새로 고침](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)을 참조하십시오. [!DNL Adobe Workfront] 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard] 지원 패키지</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus], [!UICONTROL Preferred] 및 [!UICONTROL Enterprise] 지원 패키지</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>샌드박스 미리 보기</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>샌드박스 새로 고침 사용자 지정</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## 샌드박스 미리 보기

미리보기 샌드박스는 조직의 사용자가 프로덕션 환경에 영향을 주지 않고 프로덕션 환경의 데이터를 안전하게 테스트하고 작업할 수 있는 환경 역할을 합니다.

미리보기 샌드박스에는 실제 프로덕션 데이터가 포함됩니다. 그러나 데이터는 프로덕션 환경에 비해 최대 1주일 뒤쳐질 수 있도록 매주 새로 고쳐집니다. 마지막 새로 고침 시간 이후 생성된 항목은 다음 새로 고침이 수행되기 전까지 미리보기 샌드박스 환경에 있습니다.

데이터는 방향이 단방향이며, 프로덕션에서 미리보기로 전송됩니다. 미리 보기 환경 새로 고침은 항상 주말마다 [!DNL Workfront]에 의해 예약됩니다.

미리 보기 샌드박스를 사용하면 [!DNL Workfront]이(가) 프로덕션 환경에 배포할 준비가 되기 전에 안전한 환경에서 새 기능을 배포할 수도 있습니다. 미리 보기 샌드박스에 액세스하여 새로운 기능을 테스트하고 해당 기능에 대한 피드백을 [!DNL Workfront]할 수 있습니다. 이러한 이유로 데이터가 매주 새로 고쳐지지만 미리 보기 샌드박스의 코드가 프로덕션 코드보다 항상 우선합니다.

미리보기 환경은 교육을 실행하고, 새로운 기능을 테스트하고, 설정 기능을 결정하는 데 이상적입니다.

>[!NOTE]
>
>Preview Sandbox에 액세스하면 화면 상단에 파란색 배너가 표시됩니다. 이 환경에서 작업하는 동안에는 배너를 제거할 수 없습니다.
>
>액세스하고 있는 환경의 이름(미리보기)과 코드의 릴리스 버전이 배너에 표시됩니다. 해당 릴리스에 대한 자세한 내용을 보려면 **[!UICONTROL 새로운 기능 보기]**&#x200B;를 클릭하십시오.
>
>![](assets/preview-banner-nwe-350x161.png)

## 미리보기 샌드박스 액세스

기본적으로 [!DNL Workfront] 관리자는 [!UICONTROL 미리 보기] 샌드박스 환경에 액세스할 수 있습니다. 이 섹션에 설명된 대로 [!UICONTROL 미리 보기] 샌드박스 환경에 액세스할 수 없는 경우 [!DNL Workfront] 관리자 또는 고객 지원 팀에 문의하십시오.


### [!DNL Workfront] 인터페이스에서 미리 보기 샌드박스에 액세스 {#accessing-the-preview-sandbox-from-the-workfront-interface}

[!DNL Workfront] 관리자는 [!DNL Workfront] 인터페이스를 통해 미리 보기 샌드박스에 액세스할 수 있습니다.

미리보기 샌드박스에 액세스하려면:

1. [!DNL Adobe Workfront]의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을 클릭합니다.

1. **[!UICONTROL 시스템]** > **[!UICONTROL 기본 설정]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 테스트 환경]** 섹션에서 **[!UICONTROL 샌드박스 미리 보기]**&#x200B;를 클릭합니다.

1. 미리보기 자격 증명으로 로그인합니다.

   미리 보기가 새로 고침된 후 프로덕션에서 변경하지 않는 한 프로덕션 자격 증명과 동일해야 합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.

### URL을 사용하여 미리보기 샌드박스 액세스 {#accessing-the-preview-sandbox-using-a-url}

URL을 사용하여 미리보기 샌드박스에 액세스할 수 있습니다.

#### 클러스터 1, 2, 3 및 5의 계정에 대한 미리보기 샌드박스 액세스 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

미리 보기 샌드박스의 URL: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Preview 샌드박스의 이전 URL에 책갈피가 연결되어 있는 경우, 이 변경 사항을 기록하고 책갈피의 URL을 업데이트하십시오.

URL을 사용하여 미리보기 샌드박스에 로그인하려면 다음과 같이 하십시오.

1. 다음 URL로 이동: `https://companyname.preview.workfront.com/`.

   EMEA 고객이고 계정이 클러스터 4에 있는 경우 아래 클러스터 4(EMEA 계정)의 계정에 대한 샌드박스 미리보기 액세스 섹션을 참조하십시오.

1. 미리보기 자격 증명을 사용하여 로그인합니다.

   >[!TIP]
   >
   >미리보기 새로 고침이 발생한 후 프로덕션에서 변경하지 않는 한 미리보기 자격 증명은 프로덕션 자격 증명과 동일해야 합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.


#### 클러스터 4(EMEA 계정)의 계정에 대한 샌드박스 미리 보기 액세스 {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

URL을 사용하여 미리보기 샌드박스에 로그인하려면 다음과 같이 하십시오.

1. 다음 URL로 이동: `https://companyname.preview.workfront.com/`.

   [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login)(으)로 이동하여 미리 보기 샌드박스에 액세스할 수도 있습니다.

1. 미리보기 자격 증명을 사용하여 로그인합니다.

   미리보기 새로 고침이 발생한 후 프로덕션에서 변경하지 않는 한 미리보기 자격 증명은 프로덕션 자격 증명과 동일해야 합니다. 새로 고침이 발생할 때만 로그인이 동기화됩니다. 자동으로 동기화되지 않습니다.

## 미리보기 샌드박스에서 이메일 수신

Workfront은 미리보기 샌드박스 환경에서 모든 이메일 통신을 비활성화합니다. 미리보기 샌드박스 환경에서 이메일 알림을 수신하려면 사용자 설정에서 이 기능을 활성화해야 합니다. 미리 보기 샌드박스 환경에서 전자 메일 알림을 사용하는 방법에 대한 자세한 내용은 [미리 보기 샌드박스 환경에서 전자 메일 배달 사용](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)을 참조하십시오.

>[!NOTE]
>
>모바일 앱의 보고서 배달 및 푸시 알림은 미리보기 샌드박스 환경에 대해 항상 비활성화됩니다. 미리 보기 샌드박스 환경에 액세스할 때 사용자와 [!DNL Workfront] 관리자 모두 모바일 앱에 대해 보고서 배달이나 푸시 알림을 활성화할 수 없습니다.
>
>프로덕션 환경에 대한 보고서 배달에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하십시오.


## SSO(Single Sign-On)

SSO를 사용하는 경우 고객 지원 팀과 함께 SSO 자격 증명을 사용하여 [!UICONTROL 미리 보기] 샌드박스에 로그인할 수 있도록 올바르게 구성되었는지 확인하십시오. 초기 로그인에 실패하는 경우 일반 지원 담당자 또는 [!DNL Workfront] 관리자에게 지원을 요청하십시오.

SSO(Single Sign-On)에 대한 자세한 내용은 [Adobe Workfront의 SSO 개요](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)를 참조하십시오.

## 미리보기 샌드박스에서 Single Sign-On 구성

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 [!DNL Adobe Admin Console]에 아직 온보딩되지 않은 조직에만 적용됩니다. 조직이 [!DNL Adobe Admin Console]에 온보딩되었다면 별도의 작업이 필요하지 않습니다.
>
>조직이 [!DNL Adobe Admin Console]에 온보딩되었는지 여부에 따라 다른 프로시저 목록을 보려면 [플랫폼 기반 관리 차이점([!UICONTROL Adobe Workfront]/[!UICONTROL 비즈니스 플랫폼 Adobe])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)을 참조하십시오.


SSO(Single Sign-On) 솔루션에서 작동하도록 미리보기 샌드박스를 구성하려면 프로덕션 환경에서 별도로 구성하여 이 작업을 수행할 수 있습니다. 미리보기 샌드박스의 SSO 구성은 프로덕션 환경의 SSO 구성과 독립적입니다.

미리보기 샌드박스를 새로 고칠 때(주말마다), SSO 정보는 프로덕션 환경에서 복사되어 미리보기 샌드박스 구성을 덮어쓰지 않습니다.

미리보기 샌드박스에서 SSO(Single Sign-On)를 구성하는 단계는 프로덕션 환경에서 구성하는 단계와 유사합니다.

SSO를 사용하여 [!DNL Workfront]을(를) 구성하는 방법에 대한 자세한 내용은 [Adobe Workfront의 Single Sign-On 개요](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)를 참조하십시오.

## 환경 성능 및 가용성 미리보기

[!DNL Workfront] 미리 보기 환경은 성능 또는 부하 테스트를 위한 것이 아닙니다. 대신 이러한 환경을 사용하여 조직의 기존 워크플로우로 기능 기능을 검증할 수 있습니다.

[!DNL Workfront] 미리 보기 환경은 항상 사용할 수 있습니다.

프로덕션 문제가 해결되면 정규 업무 시간 동안 [!DNL Workfront] 미리 보기 환경이 중단되는 것이 즉시 우선 순위가 됩니다.

주말(토요일 및 일요일)에 [!DNL Workfront] 미리 보기 환경에 대한 중단은 월요일의 업무 시간 동안 환경이 실행되도록 처리됩니다.
