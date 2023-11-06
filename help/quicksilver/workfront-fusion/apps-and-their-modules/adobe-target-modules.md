---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] 모듈을 사용하면 레코드를 만들거나, 읽거나, 업데이트하거나, 삭제하고, 지정된 유형의 모든 레코드를 나열하거나, 지정한 기준을 기반으로 레코드를 검색하거나, [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 51db439995430dad86e41190520824743216df69
workflow-type: tm+mt
source-wordcount: '2646'
ht-degree: 0%

---

# [!DNL Adobe Target] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Adobe Target]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다. [!DNL Adobe Target] 모듈을 사용하면 레코드를 , 만들거나, 읽거나, 업데이트하거나, 삭제하고, 지정된 유형의 모든 레코드를 나열하거나, 지정한 기준을 기반으로 레코드를 검색하거나, [!DNL Adobe Target] API.


시나리오를 만드는 방법에 대한 지침이 필요한 경우 [시나리오 만들기](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
      <td>
        <p>[!UICONTROL Pro] 이상</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td>
      <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">제품</td>
      <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td>
    </tr>
    </tr>
  </tbody>
</table>


보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

을(를) 사용하기 전에 [!DNL Adobe Target] connector에서 다음 전제 조건이 충족되는지 확인해야 합니다.

* 활성 상태가 있어야 합니다. [!DNL Adobe Target] 계정입니다.

## 에 대한 연결 만들기 [!DNL Adobe Target]

에 대한 연결을 만들려면 [!DNL Adobe Target] 모듈:

1. 클릭 **[!UICONTROL 추가]** 연결 상자 옆에 있습니다.

1. 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL 연결 이름]</td>
        <td>
          <p>이 연결의 이름을 입력하십시오.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] 클라이언트 ID. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] 클라이언트 암호. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 조직 ID]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] 조직 ID. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 기술 계정 ID]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] 기술 계정 ID. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> 테넌트를 찾으려면 [!DNL Adobe Experience Cloud], 열기 [!DNL Target]을(를) 클릭하고 [!DNL Target] 카드. URL 하위 도메인에 언급된 대로 테넌트 ID 값을 사용합니다.</p>
          <p>예를 들어 로 로그인할 때 URL이 [!DNL Adobe Target] 은(는) <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> 그러면 테넌트 ID는 "mycompany"입니다.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 메타 범위]</td>
        <td>입력 <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 개인 키]</td>
        <td>
          <p>에서 자격 증명을 만들 때 생성된 개인 키를 입력합니다. [!DNL Adobe Developer Console]. </p>
          <p>개인 키 또는 인증서를 추출하려면 다음을 수행하십시오.</p>
          <ol>
            <li value="1">
              <p>클릭 <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>추출 중인 파일 유형을 선택합니다.</p>
            </li>
            <li value="3">
              <p>개인 키 또는 인증서가 포함된 파일을 선택합니다.</p>
            </li>
            <li value="4">
              <p>파일의 암호를 입력합니다.</p>
            </li>
            <li value="5">
              <p>클릭 <b>[!UICONTROL 저장]</b> 를 클릭하여 파일을 추출하고 연결 설정으로 돌아갑니다.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 저장하고 모듈로 돌아갑니다.

## [!DNL Adobe Target] 모듈 및 해당 필드

를 구성할 때 [!DNL Adobe Target] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Target] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [액션](#actions)

* [검색 결과](#searches)


### 액션

* [[!UICONTROL 레코드 만들기]](#create-a-record)

* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)

* [[!UICONTROL 레코드 삭제]](#delete-a-record)

* [[!UICONTROL 레코드 읽기]](#read-a-record)

* [[!UICONTROL 레코드 업데이트]](#update-a-record)


#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 AB 또는 XT 활동, 오퍼 또는 대상을 만듭니다.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Target], 참조 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Target]</a> 이 문서에서.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 레코드 유형]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>만들려는 레코드 유형을 선택합니다.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>계속 <a href="#ab-activity-fields" class="MCXref xref" >AB 활동 필드</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT 활동]</p>
          <p>계속 <a href="#xt-activity-fields" class="MCXref xref" >XT 활동 필드</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL 오퍼]</p>
          <p>계속 <a href="#offer-fields" class="MCXref xref" >오퍼 필드</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL 대상]</p>
          <p>계속 <a href="#audience-fields" class="MCXref xref" >대상 필드</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB 활동 필드

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>이 활동의 이름을 입력하거나 매핑합니다. 이름은 250자를 초과할 수 없습니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>활동에 추가하려는 각 옵션에 대해 <b>[!UICONTROL 항목 추가]</b> 다음 필드를 채웁니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 옵션 로컬 ID]</b>
            </p>
            <p>API 요청 전반에서 옵션을 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 이름]</b>
            </p>
            <p>옵션 이름을 입력하거나 매핑합니다. 이름은 250자 이하여야 합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 오퍼 ID]</b>
            </p>
          </li>
          <li>
            <p>옵션과 연결된 오퍼를 선택하거나 매핑합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 위치]</td>
      <td>
        <p>활동에 추가할 각 Mbox에 대해 다음을 클릭합니다. <b>[!UICONTROL 항목 추가]</b> 다음 필드를 채웁니다.</p>
        <ul>
          <li>
            <p>[!UICONTROL 대상 ID]</p>
            <p>Mbox에 추가할 각 대상자에 대해 <b>[!UICONTROL 항목 추가]</b> 대상 ID를 선택합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 위치 로컬 ID]</b>
            </p>
            <p>API 요청에서 위치를 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 이름]</b>
            </p>
            <p>위치의 이름을 입력하거나 매핑합니다. 이름은 250자 이하여야 합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 경험]</td>
      <td>
        <p>컨텐츠 오퍼가 제공되는 페이지의 위치 목록입니다. 위치에는 다음 항목이 포함됩니다.
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience 로컬 ID]</b>
            </p>
            <p>경험의 ID 입력 또는 매핑</p>
          </li>
          <li>
            <p><b>[!UICONTROL 이름]</b>
            </p>
            <p>경험 이름 입력 또는 매핑

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>경험을 보려는 각 대상에 대해 <b>[!UICONTROL 항목 추가]</b> 대상 ID를 입력합니다.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL 방문자 비율]</b>
            </p>
            <p>경험에 할당된 방문자 비율을 입력하거나 매핑합니다</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 타사 ID]</td>
      <td>이 활동을 식별하려면 ID를 입력하거나 매핑하십시오. 이 ID를 선택할 수 있습니다. 이 ID는 다른 활동과 같을 수 없으며 250자를 초과할 수 없습니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 시작 시간]</td>
      <td>활동을 시작할 날짜 및 시간을 형식으로 입력하거나 매핑합니다. <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 종료 시간]</td>
      <td>형식으로 활동을 종료할 날짜 및 시간을 입력하거나 매핑합니다. <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 상태]</td>
      <td>
        <p>활동의 상태를 입력하거나 매핑합니다.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL 비활성화됨]</p>
          </li>
          <li>
            <p>[!UICONTROL 일시 중지됨]</p>
          </li>
          <li>
            <p>[!UICONTROL 저장됨] </p>
          </li>
          <li>
            <p>[!UICONTROL 삭제됨]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 우선 순위]</td>
      <td>활동의 우선 순위를 정의하는 숫자를 입력합니다. 숫자가 높을수록 우선 순위가 높습니다. 이 값은 0에서 999 사이여야 합니다. 기본값은 5입니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자동 할당 트래픽]</td>
      <td>
        <p>트래픽을 자동으로 할당하려면 이 옵션을 활성화합니다. 자동 할당은 더 성공적인 경험으로 더 많은 트래픽을 전송합니다.</p>
        <p>어떤 경험이 더 성공적인지를 판단할 평가 기준을 선택하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 작업 영역]</td>
      <td>활동이 연관된 작업 영역 입력 또는 매핑</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 속성 ID] </td>
      <td>활동에 추가할 각 속성에 대해 <b>[!UICONTROL 항목 추가]</b> 속성의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 보고 대상]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>활동에 추가하려는 각 보고 대상에 대해 [!UICONTROL 항목 추가]를 클릭하고 다음 정보를 입력합니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 보고 대상 로컬 ID]</b>
            </p>
            <p>API 요청에서 보고 대상을 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 대상 ID]</b>
            </p>
            <p>보고에 사용할 세그먼트 입력 또는 매핑</p>
          </li>
          <li>
            <p><b>[!UICONTROL 지표 로컬 ID]</b>
            </p>
            <p>API 요청에서 지표를 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### XT 활동 필드

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>이 활동의 이름을 입력하거나 매핑합니다. 이름은 250자를 초과할 수 없습니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>활동에 추가하려는 각 옵션에 대해 <b>[!UICONTROL 항목 추가]</b> 다음 필드를 채웁니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 옵션 로컬 ID]</b>
            </p>
            <p>API 요청 전반에서 옵션을 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 이름]</b>
            </p>
            <p>옵션 이름을 입력하거나 매핑합니다. 이름은 250자 이하여야 합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 오퍼 ID]</b>
            </p>
          </li>
          <li>
            <p>옵션과 연결된 오퍼를 선택하거나 매핑합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 위치]</td>
      <td>
        <p>활동에 추가할 각 Mbox에 대해 다음을 클릭합니다. <b>[!UICONTROL 항목 추가]</b> 다음 필드를 채웁니다.</p>
        <ul>
          <li>
            <p>[!UICONTROL 대상 ID]</p>
            <p>Mbox에 추가할 각 대상자에 대해 <b>[!UICONTROL 항목 추가]</b> 대상 ID를 선택합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 위치 로컬 ID]</b>
            </p>
            <p>API 요청에서 위치를 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 이름]</b>
            </p>
            <p>위치의 이름을 입력하거나 매핑합니다. 이름은 250자 이하여야 합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 경험]</td>
      <td>
        <p>컨텐츠 오퍼가 제공되는 페이지의 위치 목록입니다. 위치에는 다음 항목이 포함됩니다.
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience 로컬 ID]</b>
            </p>
            <p>경험의 ID 입력 또는 매핑</p>
          </li>
          <li>
            <p><b>[!UICONTROL 이름]</b>
            </p>
            <p>경험 이름 입력 또는 매핑

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>경험을 보려는 각 대상에 대해 <b>[!UICONTROL 항목 추가]</b> 대상 ID를 입력합니다.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL 방문자 비율]</b>
            </p>
            <p>경험에 할당된 방문자 비율을 입력하거나 매핑합니다</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 타사 ID]</td>
      <td>이 활동을 식별하려면 ID를 입력하거나 매핑하십시오. 이 ID를 선택할 수 있습니다. 이 ID는 다른 활동과 같을 수 없으며 250자를 초과할 수 없습니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 시작 시간]</td>
      <td>활동을 시작할 날짜 및 시간을 형식으로 입력하거나 매핑합니다. <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 종료 시간]</td>
      <td>형식으로 활동을 종료할 날짜 및 시간을 입력하거나 매핑합니다. <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 상태]</td>
      <td>
        <p>활동의 상태를 입력하거나 매핑합니다.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL 비활성화됨]</p>
          </li>
          <li>
            <p>[!UICONTROL 일시 중지됨]</p>
          </li>
          <li>
            <p>[!UICONTROL 저장됨] </p>
          </li>
          <li>
            <p>[!UICONTROL 삭제됨]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 우선 순위]</td>
      <td>활동의 우선 순위를 정의하는 숫자를 입력합니다. 숫자가 높을수록 우선 순위가 높습니다. 이 값은 0에서 999 사이여야 합니다. 기본값은 5입니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 자동 할당 트래픽]</td>
      <td>
        <p>트래픽을 자동으로 할당하려면 이 옵션을 활성화합니다. 자동 할당은 더 성공적인 경험으로 더 많은 트래픽을 전송합니다.</p>
        <p>어떤 경험이 더 성공적인지를 판단할 평가 기준을 선택하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 작업 영역]</td>
      <td>활동이 연관된 작업 영역 입력 또는 매핑</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 속성 ID] </td>
      <td>활동에 추가할 각 속성에 대해 <b>[!UICONTROL 항목 추가]</b> 속성의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 보고 대상]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>활동에 추가하려는 각 보고 대상에 대해 [!UICONTROL 항목 추가]를 클릭하고 다음 정보를 입력합니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 보고 대상 로컬 ID]</b>
            </p>
            <p>API 요청에서 보고 대상을 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 대상 ID]</b>
            </p>
            <p>보고에 사용할 세그먼트 입력 또는 매핑</p>
          </li>
          <li>
            <p><b>[!UICONTROL 지표 로컬 ID]</b>
            </p>
            <p>API 요청에서 지표를 추적하는 데 사용할 문자열을 입력하거나 매핑합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 오퍼 필드

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>이 활동의 이름을 입력하거나 매핑합니다. 이름은 250자를 초과할 수 없습니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>사용자에게 표시될 오퍼의 콘텐츠를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 작업 영역]</td>
      <td>
        <p>오퍼와 연결된 작업 공간 ID를 입력하거나 매핑합니다. 비워 두면 오퍼가 계정의 기본 작업 영역과 연결됩니다. 이 기능은 에만 적용됩니다. [!DNL Target] 프리미엄 계정.</p>
      </td>
    </tr>
  </tbody>
</table>

##### 대상 필드

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>이 대상자의 이름을 입력하거나 매핑합니다. 이름은 250자를 초과할 수 없습니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>이 대상자에 대한 설명을 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 대상 규칙]</td>
      <td>
        <p>토글을 활성화하여 규칙을 AND로 만듭니다. 즉, 모든 규칙이 적용되어야 합니다.</p>
        <p>대상에 적용할 각 규칙에 대해 <b>[!UICONTROL 항목 추가]</b> 적용할 규칙의 JSON을 입력합니다. </p>
        <div class="example"><span class="autonumber"><span><b>예: </b></span></span>
          <p>예시:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 작업 영역]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>대상자와 연결된 작업 공간 ID를 입력하거나 매핑합니다. 비워 두면 오퍼가 계정의 기본 작업 영역과 연결됩니다. 이 기능은 에만 적용됩니다. [!DNL Target Premium] 계정.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 사용자 지정 API 호출 만들기]

이 모듈에서는에 대한 사용자 지정 API 호출을 만듭니다. [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Target], 참조 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Target]</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] 기본 URL]</td>
      <td>입력 또는 매핑 [!DNL Target] 기본 URL.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 경로]</p>
      </td>
      <td>
        <p>상대 경로 입력 {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 메서드]</p>
      </td>
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 인증 헤더 및 x-api-key 헤더를 자동으로 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 쿼리 문자열]  </td>
      <td>
        <p>요청 쿼리 문자열을 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 단일 AB 활동, XT 활동, 오퍼 또는 대상을 삭제합니다.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Target], 참조 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Target]</a> 이 문서에서.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 레코드 유형]</td>
    <td>삭제할 레코드 유형을 선택합니다.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 레코드 ID]</td>
    <td>삭제할 레코드의 ID를 입력하거나 매핑합니다.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 단일 활동, 오퍼, 대상, 속성 또는 보고서에 대한 데이터를 검색합니다.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Target], 참조 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Target]</a> 이 문서에서.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 레코드 유형]</td>
    <td>읽으려는 레코드 유형을 선택합니다.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 레코드 ID]</td>
    <td>읽으려는 레코드의 ID를 입력하거나 매핑합니다.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 활동, 오퍼 또는 대상자를 업데이트합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Target], 참조 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Target]</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 레코드 유형]</td>
      <td>
        <p>업데이트할 레코드 유형을 선택합니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>에서 필드 설명 보기 <a href="#ab-activity-fields" class="MCXref xref" >AB 활동 필드</a> 아래에 <a href="#create-a-record" class="MCXref xref" >레코드 만들기</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT 활동]</b>
            </p>
            <p>에서 필드 설명 보기 <a href="#xt-activity-fields" class="MCXref xref" >XT 활동 필드</a> 아래에 <a href="#create-a-record" class="MCXref xref" >레코드 만들기</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Other Activity]</b>
            </p>
            <p>값을 갱신할 필드를 선택한 다음 필드에 새 값을 입력합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 오퍼]</b>
            </p>
            <p>에서 필드 설명 보기 <a href="#offer-fields" class="MCXref xref" >오퍼 필드</a> 아래에 <a href="#create-a-record" class="MCXref xref" >레코드 만들기</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>에서 필드 설명 보기 <a href="#audience-fields" class="MCXref xref" >대상 필드</a> 아래에 <a href="#create-a-record" class="MCXref xref" >레코드 만들기</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 레코드 ID]</td>
      <td>업데이트할 레코드의 ID를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

### 검색 결과

* [[!UICONTROL 레코드 가져오기]](#get-records)

* [[!UICONTROL 검색]](#search)


#### [!UICONTROL 레코드 가져오기]

이 검색 모듈은 선택한 유형의 레코드 목록을 검색합니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Target], 참조 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Target]</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 레코드 유형]</td>
      <td>업데이트할 레코드 유형을 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 정렬 기준]</td>
      <td>정렬할 각 필드에 대해 <b>[!UICONTROL 항목 추가]</b> 필드를 선택하고 반환된 결과가 오름차순이어야 하는지 아니면 내림차순이어야 하는지 여부를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 시작 시간]</td>
      <td>
        <p>레코드를 검색할 가장 빠른 일자를 입력합니다. </p>
        <p>지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오. <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 변환 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 종료 시간]</td>
      <td>
        <p>레코드를 검색할 최신 날짜를 입력합니다. </p>
        <p>지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오. <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 변환 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 검색]

이 검색 모듈은 지정한 기준에 따라 활동, 오퍼 또는 대상을 검색합니다.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>에 대한 연결 만들기에 대한 지침: [!DNL Adobe Target], 참조 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >에 대한 연결 만들기 [!DNL Adobe Target]</a> 이 문서에서.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 레코드 유형]</td>
    <td>업데이트할 레코드 유형을 선택합니다.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 정렬 기준]</td>
    <td>정렬할 각 필드에 대해 <b>[!UICONTROL 항목 추가]</b> 필드를 선택하고 반환된 결과가 오름차순이어야 하는지 아니면 내림차순이어야 하는지 여부를 선택합니다.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 검색 기준]</td>
    <td>설정하려는 각 규칙에 대해 필드, 연산자 및 값을 선택합니다. 클릭 <b>[!UICONTROL Add AND RULE]</b> 추가 규칙을 만들려면</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>모듈이 반환하려는 첫 번째 응답의 번호를 입력합니다. 첫 번째 반환된 응답의 오프셋은 다음과 같습니다. <code>0</code>. 이 필드를 [!UICONTROL Maximum number of returned results] 필드와 함께 사용하여 응답의 페이지를 지정합니다.</p>
      <p>예를 들어 응답의 세 번째 페이지를 보려면 각 페이지에 응답이 10개일 때 [!UICONTROL Offset]을 20으로 설정하고 [!UICONTROL 반환되는 최대 결과 수]를 10으로 설정합니다.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 반환되는 최대 결과 수]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다. 이 필드를 [!UICONTROL Offset] 필드와 함께 사용하여 응답의 페이지를 지정합니다.</p>
      <p>예를 들어 응답의 세 번째 페이지를 보려면 각 페이지에 응답이 10개일 때 [!UICONTROL Offset]을 20으로 설정하고 [!UICONTROL 반환되는 최대 결과 수]를 10으로 설정합니다.</p>
    </td>
  </tr>
</tbody>
</table>
