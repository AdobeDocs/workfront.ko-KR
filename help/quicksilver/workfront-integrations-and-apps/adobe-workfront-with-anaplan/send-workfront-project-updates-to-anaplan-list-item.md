---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Anaplan] 목록 항목에  [!DNL Adobe Workfront] 프로젝트 업데이트 보내기'
description: 이 통합 시나리오는  [!DNL Adobe Workfront] 프로젝트의 진행 상황, 상태 및 주요 일정 세부 정보를  [!DNL Anaplan] 예산 목록 항목과 공유합니다. 이 정보를 공유하면  [!DNL Anaplan] 이(가) 제공하는 지출 최적화 및 재무 분석을 더 잘 활용할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 프로젝트 업데이트를 [!DNL Anaplan] 목록 항목으로 보내기

이 통합 시나리오는 [!DNL Adobe Workfront] 프로젝트의 진행 상황, 상태 및 주요 일정 세부 정보를 [!DNL Anaplan] 예산 목록 항목과 공유합니다. 이 정보를 공유하면 [!DNL Anaplan]에서 제공하는 지출 최적화 및 재무 분석을 더 잘 활용할 수 있습니다.

>[!IMPORTANT]
>
>이 문서의 &quot;캠페인&quot;은 이 시나리오가 나타내는 마케팅 캠페인 사용 사례를 참조합니다. [!DNL Workfront]에서 [!DNL Workfront Fusion] Adobe Campaign 커넥터 또는 최근에 더 이상 사용되지 않는 [!UICONTROL 캠페인] 개체에 연결할 수 없습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>작업 자동화 및 통합을 위한 Workfront Fusion </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구입해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

&#42;&#42;라이선스 [!DNL Adobe Workfront Fusion]에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 이벤트 트리거 중

이 시나리오는 15분마다 실행되도록 예약되어 있습니다.

## [!DNL Workfront] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Workfront]에 다음 항목이 있어야 합니다.

* [!DNL Workfront]의 사용자 프로필(이름이 **[!UICONTROL [!DNL Anaplan]통합]**&#x200B;임)에 시스템 관리자 권한이 있습니다.

  [!DNL Workfront]에서 사용자를 만드는 방법에 대한 자세한 내용은 [사용자 추가](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)를 참조하십시오.

* Anaplan으로 보낼 사용자 지정 데이터 값을 저장하기 위해 프로젝트 개체에 **[!UICONTROL Campaign Brief]** 사용자 지정 양식이 첨부되었습니다.

  다음 필드는 Anaplan에 대한 데이터 매핑을 지원하기 위해 사용자 정의 양식에 포함할 수 있는 필드의 예를 나타내지만, 이 통합 시나리오에 필수는 아닙니다.

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>필드 이름</th> 
     <th>필드 유형</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">시장 시작 날짜의 [!UICONTROL]</td> 
     <td>[!UICONTROL 날짜] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">시장 종료 날짜의 [!UICONTROL]</td> 
     <td>[!UICONTROL 날짜]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL 캠페인 개요]</td> 
     <td>[!UICONTROL 단락 텍스트 필드]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL 키 메시지]</td> 
     <td>[!UICONTROL 단락 텍스트 필드]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL 드롭다운]</p> <p>프로세스에 맞는 옵션을 포함합니다.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## [!DNL Anaplan] 구성이 필요합니다.

이 시나리오를 사용하려면 [!DNL Anaplan]에 다음 항목이 있어야 합니다.

* [!DNL Anaplan]의 사용자 프로필(이름이 **[!UICONTROL [!DNL Workfront]통합]**&#x200B;임)에 시스템 관리자 권한이 있습니다.
* 이 시나리오에 사용할 [!DNL Anaplan] 모델입니다.
* 이 시나리오에 사용할 [!DNL Anaplan] 모델 내의 목록입니다.
* 다음 열이 순서대로 포함된 **[!UICONTROL 프로젝트 업데이트 가져오기]** 파일:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] 프로젝트 GUID]

3. [!UICONTROL 캠페인 이름]

4. [!UICONTROL 완료율]

5. [!UICONTROL 계획된 시작 일자]

6. [!UICONTROL 계획된 완료 일자]

7. [!UICONTROL 계획된 시간]

8. [!UICONTROL 계획된 비용]

9. [!UICONTROL 계획된 경비]

10. [!UICONTROL 실제 인건비]

11. [!UICONTROL 계획된 인건비]

12. [!UICONTROL 상태]

[!UICONTROL [!DNL Anaplan] 계획된 경비 가져오기] 파일을 준비하려면:

1. 다음 내용을 복사하여 텍스트 편집기 또는 [!DNL Excel]에 붙여 넣으십시오.
1. 파일을 CSV 형식으로 저장
1. 파일을 Anaplan에 업로드합니다.

   지침은 파일에서 모듈로 데이터를 가져오는 방법에 대한 [!DNL Anaplan] 설명서를 참조하십시오.

1. 파일에 지정한 이름을 기록해 두십시오. 이 이름은 [!UICONTROL Fusion] 시나리오 템플릿을 배포하는 동안 사용됩니다.

CSV 콘텐츠 예

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>선택적 열은 다음과 같습니다.

1. [!UICONTROL 캠페인 개요]

2. [!UICONTROL 키 메시지]

3. [!UICONTROL 시장 시작 날짜]

4. [!UICONTROL 마켓 종료 날짜의 ]

5. [!UICONTROL 대상]

또한 매핑에 설정하고자 하는 다른 필드도 포함합니다.

* 파일 업로드에 전달된 데이터 가져오기를 실행하기 위해 **[!UICONTROL 프로젝트 업데이트 가져오기]** 프로세스가 준비되었습니다.

이러한 작업에 대한 지침은 [!DNL Anaplan] 설명서를 참조하십시오.

## [!DNL Workfront Fusion]에 배포 중

다음 단계를 완료하여 이 통합 시나리오를 Fusion 계정에 배포합니다. 필요한 [!DNL Workfront] 및 [!DNL Anaplan] 구성을 완료한 후에만 이 작업을 수행해야 합니다.

1. [!DNL Workfront Fusion]의 [!UICONTROL 템플릿] 메뉴로 이동한 다음 **[!UICONTROL 목록 항목 [!DNL Anaplan]에 Workfront 프로젝트 업데이트 보내기]** 시나리오 템플릿을 클릭합니다.
1. 다음 [!DNL Anaplan]개 변수에 대한 변수 값을 바꿉니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>변수 이름</th> 
      <th>값 바꾸기</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>[!DNL Anaplan] 계정의 작업 영역 ID입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 모델 ID] </td> 
      <td>[!DNL Anaplan] 계정 및 선택한 작업 영역의 모델 ID.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 캠페인 목록 이름]</td> 
      <td>[!DNL Anaplan] 계정 및 선택한 작업 영역 및 모델의 목록 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 파일 이름: 프로젝트 업데이트 가져오기]</td> 
      <td>프로젝트 업데이트 데이터를 받을 파일의 이름입니다.<p>(예: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 프로세스 이름: 프로젝트 업데이트 가져오기]</td> 
      <td> <p>프로젝트 데이터 가져오기를 실행할 프로세스의 이름입니다.</p> <p>(예: WF Int - 캠페인 세부 정보 업데이트)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] 하위 도메인]</td> 
      <td>[!DNL Workfront] 계정의 하위 도메인입니다. 생성된 메모에서 [!DNL Workfront] 프로젝트에 대한 링크를 다시 만드는 데 사용됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

   파일 및 프로세스를 설정하는 방법에 대한 자세한 내용은 [!DNL Anaplan] 설치 설명서를 참조하세요.

1. [!DNL Anaplan] 연결 프로필을 선택하거나 추가하십시오.
1. 메시지가 표시되면 나머지 [!DNL Anaplan] 모듈을 모두 [!DNL Anaplan] 연결로 업데이트합니다.
1. [!DNL Workfront] 연결 프로필을 선택하거나 추가하십시오.

   필터는 모든 미완료 연결된 프로젝트와 지난 29분 내에 완료된 프로젝트를 가져오도록 구성되어 있습니다. [!DNL Fusion] 시나리오의 빈도를 변경하면 시나리오 템플릿을 배포한 후 이 값을 업데이트할 수 있습니다.

1. **[!UICONTROL 프로젝트 업데이트 CSV 빌드]** 모듈에서 프로젝트 특성을 CSV 열에 매핑하는 새 데이터 구조를 추가합니다.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. 메시지가 표시되면 나머지 [!DNL Workfront] 모듈을 모두 [!DNL Workfront] 연결로 업데이트합니다.

## 기타 권장 시나리오 템플릿

이 시나리오 템플릿은 다음과 같은 비용 최적화 시나리오 템플릿을 보완하며, 이 시나리오 템플릿 또한 배포할 수 있습니다.

* [[!UICONTROL 목록 항목  [!DNL Anaplan] 에 대한  [!DNL Adobe Workfront] 실제 시간 업데이트 보내기]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 목록 항목 [!DNL Anaplan] 에 경비 보내기 [!DNL Adobe Workfront] 경비]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

예산 요청 연결을 위한 추가 시나리오:

* [[!UICONTROL 예산 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3}]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 프로젝트에  [!DNL Anaplan] 예산 할당 적용 [!DNL Adobe Workfront] 프로젝트]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Campaign 요청 연결을 위한 추가 시나리오:

* [[!UICONTROL 캠페인 요청에서  [!DNL Anaplan] 목록 항목 만들기 [!DNL Adobe Workfront] 3}]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 캠페인 요청 또는 캠페인 프로젝트에  [!DNL Anaplan] 예산 할당 적용 [!DNL Adobe Workfront] 3}]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
