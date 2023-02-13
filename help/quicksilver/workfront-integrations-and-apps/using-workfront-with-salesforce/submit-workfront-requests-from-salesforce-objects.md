---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 제출 [!DNL Adobe Workfront] 요청 [!DNL Salesforce] 개체
description: 설치 후 [!DNL Adobe Workfront] 대상 [!DNL Salesforce], you can submit [!DNL Workfront] 요청 [!DNL Salesforce] 기회 및 계정 이 기능은 Classic 및 Lightning Experience 프레임워크 모두에 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# 제출 [!DNL Adobe Workfront] 요청 [!DNL Salesforce] 개체

설치 후 [!DNL Adobe Workfront for Salesforce], 제출할 수 있습니다. [!DNL Workfront] 요청 [!DNL Salesforce] 기회 및 계정 이 기능은 [!DNL Classic] 및 [!DNL Lightning Experience] 프레임워크.

## 액세스 요구 사항

이 문서에 설명된 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 플랜*</p></td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 라이센스*</p></td> 
   <td> <p>[!UICONTROL 계획]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

을(를) 제출하려면 [!DNL Workfront] 다음에서 요청 [!DNL Salesforce] Opportunity 또는 Account 는 사용자 환경에 다음 내용이 있는지 확인합니다.

* 사용자 [!DNL Workfront] 관리자가 설치됨 [!DNL Workfront for Salesforce].\
   설치에 대한 자세한 정보 [!DNL Workfront for Salesforce]를 참조하십시오. [설치 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 사용자 [!DNL Workfront] 관리자가 추가되었습니다. [!DNL Workfront] 섹션에 대한 섹션을 참조하십시오. [!UICONTROL 기회] 및 [!UICONTROL 계정] 페이지 레이아웃.\
   추가 정보에 대한 자세한 정보 [!DNL Workfront] 페이지 레이아웃에 대한 자세한 내용은 [구성 [!DNL Adobe Workfront] 섹션 [!DNL Salesforce] 사용자](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 다음을 수행합니다. [!DNL Workfront] 계정 및에서 로그인할 수 있습니다. [!DNL Workfront] 섹션을 참조하십시오.\
   로그인하면 [!UICONTROL 새 요청] 탭: 요청 입력을 시작할 수 있습니다.

## 제출 [!DNL Workfront] 요청 [!DNL Salesforce]

1. Salesforce에서 Opportunity 또는 Account 로 이동합니다.
1. 로 이동합니다. [!DNL Workfront] 섹션을 참조하십시오.
1. 에서 **[!UICONTROL 새 요청]** 탭에서 요청 유형을 선택합니다 **[!UICONTROL 요청 유형 선택]** 드롭다운 메뉴

   Workfront에서 볼 수 있는 액세스 권한이 있는 동일한 요청 큐를 볼 수 있습니다.

1. 요청에 사용 가능한 필드 작성을 시작합니다.

   다음에서 요청 제출 [!DNL Salesforce] 는 요청에서 제출하는 것과 동일합니다. [!DNL Workfront] 웹 응용 프로그램입니다.

   >[!NOTE]
   >
   >를 사용하여 문서 업로드 [!DNL Workfront] 플러그인 [!DNL Salesforce] 일시적으로 사용할 수 없습니다.

   에 설명된 단계를 계속 수행합니다. [만들기 및 제출 [!DNL Adobe Workfront] 요청](../../manage-work/requests/create-requests/create-submit-requests.md).

1. 클릭 **[!UICONTROL 제출]**.

## 보기 [!DNL Workfront] 요청

1. 의 Opportunity 또는 Account 로 이동합니다. [!DNL Salesforce].
1. 로 이동합니다. **[!DNL Workfront]** 섹션을 참조하십시오.

   >[!NOTE]
   >
   >사용자의 [!DNL Workfront] 관리자가 이 섹션을 구성했는데 다른 이름이 있을 수 있습니다.

1. 을(를) 선택합니다 **[!UICONTROL 제출된 요청]** 탭.

   이 탭에서 사용자나 다른 사람이 이 Opportunity 또는 Account에서 제출한 모든 요청을 볼 수 있습니다.웹 응용 프로그램에서 이 요청 대기열에 제출된 요청은 이 목록에 표시되지 않습니다 [!DNL Salesforce].

   >[!NOTE]
   >
   >웹 응용 프로그램의 이 요청 큐에 제출된 요청은 Salesforce의 이 목록에 표시되지 않습니다.

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   제출된 요청에 대해 다음 정보를 볼 수 있습니다.

   * 요청 이름(에서) [!UICONTROL 제목] column)
   * 참조 번호
   * 요청 유형
   * 상태
   * 제출 날짜
   * 이름으로 요청
   * 이름에 할당됨\

      이 정보는에서 업데이트됩니다. [!DNL Workfront]도 이 목록에 업데이트됩니다.

1. (선택 사항) 요청 이름을 클릭하여 열기 [!DNL Workfront].

1. (선택 사항) **[!UICONTROL 이동[!DNL Salesforce]]** 문제가 Workfront의 다음 영역에서 발생한 영업 기회 또는 계정에 액세스하려면

   * 에서 [!UICONTROL 세부 사항] 문제의 섹션
   * 목록에서 문제를 선택할 때 [요약] 패널에서 [!UICONTROL 요약 열기] ![](assets/summary-panel-icon.png) 를 클릭합니다.
   * 문제 헤더에서 [!UICONTROL 통합] 필드를 사용할 수 있습니다. 시스템 또는 그룹 관리자가 [!UICONTROL 통합] 문제 헤더에서 Salesforce로 이동 링크를 보려면 레이아웃 템플릿에 필드를 추가합니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >다음 [!UICONTROL Salesforce로 이동] 링크가 모두 표시됩니다 [!DNL Workfront] 문제를 볼 수 있는 사용자입니다. 다음을 수행해야 합니다. [!DNL Salesforce] 이(가) [!DNL Salesforce] 문제가 기록된 기회 또는 계정입니다.
