---
title: Adobe Workfront Planning 요청 제출
description: 누군가가 Adobe Workfront Planning의 레코드 유형 페이지에서 요청 양식에 대한 링크를 귀하에게 공유하면 요청을 추가하여 요청 양식과 연관된 레코드 유형에 대한 레코드를 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: f3f33d870859408db5ec3dc306cf1d4209c126a3
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Adobe Workfront Planning 요청을 제출하여 레코드 생성

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

누군가가 Adobe Workfront Planning의 레코드 유형 페이지에서 요청 양식에 대한 링크를 귀하에게 공유하면 요청을 추가하여 요청 양식과 연관된 레코드 유형에 대한 레코드를 생성할 수 있습니다.

Workfront 사용자와 외부 사용자는 Planning 레코드 유형에 요청을 제출하고 레코드를 생성할 수 있습니다. <!--double check on the external users-->

이 문서에서는 레코드 유형에 새 레코드를 추가하도록 요청을 제출하는 방법에 대해 설명합니다.

작업 영역 관리자가 요청 양식을 만들고 레코드 유형과 연결하는 방법에 대한 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront 계획<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td>
   <td>
<p>다음 Workfront 플랜 중 하나:</p>
<ul><li>선택</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td>
   <td>
<p>임의 </p>  
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td>
   <td>
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>External, Contributor, Light 또는 Standard 라이센스</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <p>Workfront 사용자인 경우 작업 영역에 대한 이상의 권한 보기</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront의 계획 영역에 액세스하려면 주 메뉴에서 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>
   <p> 하지만 Workfront Planning에 요청을 제출하는 데 계획 영역에 액세스할 필요는 없습니다. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

Workfront Planning 요청 양식에 요청을 제출하려면 먼저 다음 조건을 충족해야 합니다.

* Workfront Planning에는 다음이 있어야 합니다.

   * 작업 영역
   * 요청 양식과 연결된 레코드 유형입니다. 자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

* 액세스 가능한 방식으로 요청 양식을 링크와 공유해야 합니다. 다음과 같은 시나리오가 있습니다.

   * Workfront 계정이 있는 경우 링크는 내부 직원하고만 공유되었으며 작업 영역에 대한 기여 이상의 액세스 권한이 있습니다. Workfront 외부 사용자는 내부적으로 공유된 링크에 액세스할 수 없습니다.
   * Workfront 계정이 없는 경우 링크가 외부 사용자와 공유되었습니다. Workfront 사용자는 외부 사용자와 공유되는 링크에 액세스할 수도 있습니다.

* 양식에 대한 링크가 만료되지 않아야 합니다.

## Workfront Planning에 요청 제출에 대한 고려 사항

* 양식에 대한 특정 링크에서만 Workfront Planning 요청에 대한 요청 양식에 액세스할 수 있습니다.
* 요청을 Workfront Planning에 제출한 후에는 요청을 편집할 수 없습니다.
* 제출된 각 요청은 양식이 승인과 연계되어 있지 않거나 모든 승인자가 승인을 부여한 경우 사용하는 양식과 연계된 레코드 유형에 대한 레코드를 생성합니다.
* 요청 양식을 제출하여 생성된 레코드는 다른 방법을 통해 추가된 레코드와 구분할 수 없습니다. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
* 제출된 요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭에 표시됩니다.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Workfront Planning에 요청 제출

<!--
<div class="preview">

Submitting requests to Workfront Planning differs depending on what environment you use. 

### Submit a request to Workfront Planning in the Preview Environment

>[!NOTE]
>
>After the monthly releases to Production, the features described in this section are also available in the Production environment for customers who enabled fast releases.

{{step1-to-requests}}

1. Enable the **Switch to a new experience** setting, in the upper-right corner of he screen. 
   Enabling this setting makes the Workfront Planning request forms available in the **Requests** area of Workfront.

   >[!TIP]
   >
   >   This setting is available only when your company has purchased a Workfront Planning package. 

1. Click **New request**. (********* update scree shot at release ********)

   ![New request box with unified Workfront and Planning cards](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   The New request area opens with the following information: 

   * The 6 most recently accessed Workfront request queues and Planning request forms display in the Recent section. 
   * 50 additional Workfront request queues and Planning request forms display in alphabetical order in the **All request forms** section. You can search for a request queue that does not display by default. 

1. Do one of the following:

   * Click the card for one of the Planning request forms in the Recent or All request forms sections
   * Start typing the name of a Planning request form in the search box, then click the card when it displays in the list. 

   The request form opens.

1. Update the fields available in the request form. Fields with a red asterisk are required. 
1. Click **Submit**.
    
   The request form closes and you return to the **Requests** area. 

   Your form is submitted and the following things occur:

   * If the request form was not associated with an approval, the request is added to the Planning tab of the Submitted section of the Workfront Requests area and a new record is added to the record type associated with the form.
   
   * If the request form was associated with an approval, the request is added to the Planning tab of the Submitted section of the Workfront Requests area. A new record is added to the record type page only after all the approvers have approved it.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      ![](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

      >[!IMPORTANT]
      >
      >All users who have access to at least one workspace can view the Planning tab in the Requests area. You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. (******** ensure this is correct; asking team in slack **************)

   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.

      >[!NOTE]
      >
      >The email and in-app notifications are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.

1. (Optional) Click the **Planning** tab in the Requests area to view your request. 
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Record** field. 

   The record's page opens. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

</div>

### Submit a request to Workfront Planning in the Production environment

-->

1. Workfront Planning 레코드 유형에서 사용자와 공유되는 링크로 이동합니다.

1. 양식에서 사용할 수 있는 필드를 업데이트합니다. 별표가 있는 필드는 필수입니다.

   >[!TIP]
   >
   >   **제목** 필드를 사용할 수 있는 경우 요청이 제출된 후에는 Workfront Planning에 표시되지 않습니다.
   >
   >Workfront Planning의 레코드 유형에 추가될 때 새 레코드를 식별할 수 있도록 요청의 필드를 가능한 한 많이 업데이트하는 것이 좋습니다.

1. **제출**&#x200B;을 클릭합니다.

   양식이 제출되고 다음 사항이 발생합니다.

   * 요청 양식이 승인과 연결되어 있지 않은 경우 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 요청이 추가되고 양식에 연결된 레코드 유형에 새 레코드가 추가됩니다.

   * 요청 양식이 승인과 연결된 경우 Workfront 요청 영역의 제출됨 섹션에 있는 계획 탭에 요청이 추가됩니다. 새 레코드는 모든 승인자가 승인한 후에만 레코드 유형 페이지에 추가됩니다.

     자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >하나 이상의 작업 영역에 액세스할 수 있는 모든 사용자는 요청 영역에서 계획 탭을 볼 수 있습니다. 볼 수 있는 권한 이상이 있는 작업 영역에 사용자 또는 다른 사람이 제출한 요청만 볼 수 있습니다. Workfront 관리자는 시스템의 작업 영역에 제출된 모든 요청을 볼 수 있습니다. <!--ensure this is correct; asking team in slack-->

   * 요청이 성공적으로 제출되었거나 검토를 위해 전송되었다는 인앱 및 이메일 알림을 받게 됩니다.
   * 요청 양식이 승인과 연결된 경우 승인자는 요청을 검토하고 승인하기 위한 인앱 및 이메일 알림을 수신합니다.

     >[!NOTE]
     >
     >이메일 및 인앱 알림은 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩될 때만 표시됩니다.

1. (선택 사항) 요청을 보려면 요청 영역에서 **계획** 탭을 클릭합니다.
1. (조건부) 요청 양식이 승인과 연결되어 있지 않거나 요청이 승인된 경우 요청 이름을 클릭한 다음 **레코드** 필드의 레코드 이름을 클릭합니다.

   레코드 페이지가 열립니다.

   >[!TIP]
   >
   >* 레코드 이름이 요청 양식에 추가되지 않은 경우 요청의 레코드 필드에 있는 레코드 이름이 **제목 없음**&#x200B;으로 표시됩니다.
   >
   >* 요청 양식이 승인과 연결된 경우 요청 페이지에서 레코드에 액세스하려면 승인을 받아야 합니다.




