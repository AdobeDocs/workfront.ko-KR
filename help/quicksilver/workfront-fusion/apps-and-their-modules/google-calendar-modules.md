---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Google 달력 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오는 Google Calendar를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있는 것입니다.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3773'
ht-degree: 0%

---

# [!DNL Google Calendar] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!UICONTROL Google 달력]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

를 사용하려면 [!DNL Google Calendar] 모듈이면 반드시 [!DNL Google] 계정이 필요합니다.

## [!DNL Google Calendar] 모듈 및 해당 필드

구성 시 [!DNL Google Calendar] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Google Calendar] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [이벤트](#events)
* [캘린더](#calendars)
* [액세스 제어 규칙](#access-control-rules)
* [반복기(더 이상 사용되지 않음)](#iterators-deprecated)
* [기타](#other)

### 이벤트

* [[!UICONTROL 이벤트 보기]](#watch-events)
* [[!UICONTROL 이벤트 검색]](#search-events)
* [[!UICONTROL 이벤트 가져오기]](#get-an-event)
* [[!UICONTROL 이벤트 만들기]](#create-an-event)
* [[!UICONTROL 이벤트 업데이트]](#update-an-event)
* [[!UICONTROL 이벤트 삭제]](#delete-an-event)


#### [!UICONTROL 이벤트 보기]

이 트리거 모듈은 지정한 달력에서 새 이벤트가 추가, 업데이트, 삭제, 시작 또는 종료되면 시나리오를 실행합니다. 이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 또는 레코드와 연관된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>모듈이 작업할 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>생성된 날짜, 업데이트된 날짜, 시작 날짜 또는 종료 날짜별로 이벤트를 감시할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 삭제된 이벤트 표시]</td> 
   <td> <p>삭제된 이벤트를 포함하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] </td> 
   <td> <p>검색할 텍스트를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제한]</td> 
   <td> <p> 최대 이벤트 수 설정 [!DNL Workfront Fusion] 은 한 주기 동안(시나리오 실행당 반복 횟수) 를 사용합니다. 이 값을 너무 높게 설정하면 지정된 타사 서비스(시간 초과)의 측에서 연결이 중단될 수 있습니다. [!DNL Workfront Fusion] 는 이 작업에 영향을 주지 않습니다. 더 낮은 값을 설정하고 최대 주기 수에 대해 더 높은 값을 정의하거나 시나리오를 더 자주 실행하는 것이 좋습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 검색]

이 작업 모듈은 선택한 달력에서 이벤트를 검색합니다.

검색의 달력 및 매개 변수를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 이벤트 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>연결 방법에 대한 지침은 [!DNL Google Calendar] Workfront Fusion 계정, <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion에 대한 연결 만들기 - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>검색할 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 시작 날짜]</td> 
   <td> <p> 이벤트가 시작되는 날짜를 입력하거나 매핑합니다. 또한 이 모듈은 입력한 시작 날짜에 계속 발생하는 이 날짜 이전의 이벤트를 검색합니다. </p> <p>지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종료 날짜]</td> 
   <td> <p> 이벤트가 종료될 날짜를 입력하거나 매핑합니다. </p> <p> 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Single Events]</td> 
   <td> <p> 반복 이벤트를 단일 인스턴스로 처리하려면 이 옵션을 활성화합니다. 예를 들어, 주별 회의가 있고 이 옵션이 활성화되어 있으면 이 모듈은 각 주의 회의를 별도의 이벤트로 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>검색할 검색어를 입력하거나 매핑합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>결과에서 반환된 이벤트의 순서를 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 시작 시간]</strong>: 시작 날짜 및 시간(오름차순)별로 정렬합니다. 단일 이벤트를 쿼리할 때만 사용할 수 있습니다.</li> 
     <li><strong>[!UICONTROL 업데이트된 시간]</strong>: 마지막 수정 시간까지 정렬(오름차순).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제한]</td> 
   <td> <p>최대 이벤트 수 설정 [!DNL Workfront Fusion] 한 실행 주기 동안 를 반환합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 가져오기]

이 작업 모듈은 지정된 달력의 단일 이벤트에 대한 메타데이터를 반환합니다.

달력 및 이벤트를 지정합니다.

이 모듈은 연결된 모든 필드 및 사용자 지정 필드와 함께 이벤트의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>가져올 이벤트가 포함된 달력 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 ID] </td> 
   <td> <p>기존 이벤트의 이벤트 ID를 입력합니다 [!DNL Google Calendar] 가져올 이벤트입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 만들기]

이 작업 모듈은 이벤트를 만듭니다.

이벤트의 달력 및 매개 변수를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 이벤트 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>연결 방법에 대한 지침은 [!DNL Google Calendar] Workfront Fusion 계정, <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion에 대한 연결 만들기 - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 만들기]</td> 
   <td> <p>이벤트를 만들 방법을 선택합니다.</p> 
    <ul> 
     <li><b>[!UICONTROL 세부 정보]</b><p>이 옵션을 사용하면 이벤트에 대해 자세히 입력할 수 있습니다.<br></p></li> 
     <li><b>[!UICONTROL Fast]</b><p>달력을 선택하고 이벤트 이름을 입력하기만 하면 됩니다. 이름과 이름에 시간과 장소 세부 사항을 포함할 수 있습니다. [!DNL Google Calendar] 은 해당 장소 및 시간에 대한 이벤트를 예약합니다.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>이벤트를 표시할 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>캘린더에 이벤트가 표시되는 색상을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 이름]</td> 
   <td> <p> 이벤트의 이름을 입력하거나 매핑합니다. </p> <p>참고: [!UICONTROL 이벤트 만들기] 필드에서 [!UICONTROL 빠른 추가]를 선택한 경우 이벤트의 날짜 및 시간을 포함할 수 있습니다. [!DNL Workfront Fusion] 해당 날짜 및 시간에 대한 이벤트를 만듭니다. 예: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. [!UICONTROL 빠른 추가]를 선택했지만 이벤트 이름에 날짜 및 시간을 포함하지 않으면 이벤트가 현재 시간에서 만들어지고 1시간이 지속됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 하루 종일 이벤트]</td> 
   <td>이벤트가 하루 종일 이벤트인 경우 이 옵션을 활성화합니다(시작 및 종료 시간이 필요하지 않음).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 시작 날짜]</td> 
   <td> <p>하루 종일 이벤트인 경우 이벤트의 시작 날짜를 입력합니다. </p> <p>지원되는 날짜 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 종료 날짜]</td> 
   <td> <p> 종일 이벤트인 경우 이벤트의 종료 날짜를 입력합니다. </p> <p>지원되는 날짜 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Description]</td> 
   <td>이벤트의 설명을 입력하거나 매핑합니다. 이 필드는 HTML을 지원합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>이벤트의 위치를 텍스트 양식에 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이 이벤트에 대한 기본 미리 알림 설정 사용]</td> 
   <td>기본 미리 알림 설정을 사용하려면 이 옵션을 활성화하십시오. [!UICONTROL 미리 알림] 필드에서 사용자 지정 미리 알림을 설정하면 이 값이 아니오로 설정됩니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 미리 알림] </td> 
   <td> <p>이벤트에 대한 미리 알림을 추가합니다. 각 미리 알림에 대해 상기할 방법을 선택하고, 메시지를 표시할 이벤트 전 시간(분)을 정의합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 참석자]</td> 
   <td>참석자를 이벤트에 추가합니다. 각 참석자의 이름과 전자 메일 주소를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 다음으로 표시]</td> 
   <td>일정을 보는 사람이 이 이벤트 중에 사용자를 사용 중 또는 사용 가능으로 표시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibility] </td> 
   <td> <p>이 이벤트의 가시성을 선택합니다. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Default]</b></p> <p>이벤트에는 달력 설정에서 설정한 가시성이 있습니다.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>캘린더가 공유되는 모든 사용자는 이 이벤트를 볼 수 있습니다.</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>참석자만 이 이벤트를 볼 수 있습니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 만들기에 대한 알림 보내기]</td> 
   <td> <p>모든 게스트에게 새 이벤트 만들기에 대한 알림을 전송할지 여부를 선택합니다.[!DNL Google Calendar] 손님들, 아무에게도</p> <p>팁: 마이그레이션 사용 사례에 대해서만 [!UICONTROL 없음] 옵션을 사용하는 것이 좋습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 게스트가 이벤트를 수정할 수 있음]</td> 
   <td> <p>게스트가 이 이벤트를 수정할 수 있도록 하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 되풀이]</td> 
   <td>이 이벤트에 적용할 되풀이 규칙을 추가합니다. 각 규칙에는 반복 이벤트에 대한 [!UICONTROL RRULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] 및 [!UICONTROL EXDATE] 라인 목록이 필요합니다. [!UICONTROL DTSTART] 및 [!UICONTROL DTEND] 줄은 이 필드에 허용되지 않습니다. 이벤트 시작 및 종료 시간은 시작 및 종료 필드에 지정됩니다. 이 필드는 단일 이벤트 또는 반복 이벤트 인스턴스에 대해 생략됩니다. 자세한 내용은 <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 업데이트]

이 작업 모듈은 기존 이벤트를 변경합니다.

달력 및 이벤트 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 이벤트 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>작업할 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 ID] </td> 
   <td> <p>앞에서 만든 이벤트 ID를 입력합니다 [!DNL Google Calendar] 업데이트할 이벤트입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

원하는 필드에 새 값을 입력하여 이벤트 정보를 업데이트할 수 있습니다. 개별 필드에 대한 자세한 내용은 [[!UICONTROL 이벤트 만들기]](#create-an-event).

#### [!UICONTROL 이벤트 삭제]

이 작업 모듈은 이벤트를 삭제합니다.

달력 및 이벤트 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 이벤트 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>삭제할 이벤트가 포함된 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 ID]</td> 
   <td> <p> 이전에 만든 이벤트 ID를 입력합니다 [!DNL Google Calendar] 삭제할 이벤트입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이벤트 삭제에 대한 알림 보내기]</td> 
   <td>이벤트 삭제에 대한 알림을 사용하지 않는 게스트에게 전송할지 여부를 선택합니다 [!DNL Google Calendar]또는 아무도 없습니다.</td> 
  </tr> 
 </tbody> 
</table>

### 캘린더

* [[!UICONTROL 일정 나열]](#list-calendars)
* [[!UICONTROL 달력 가져오기]](#get-a-calendar)
* [[!UICONTROL 달력 만들기]](#create-a-calendar)
* [[!UICONTROL 달력 업데이트]](#update-a-calendar)
* [[!UICONTROL 달력 삭제]](#delete-a-calendar)
* [[!UICONTROL 달력 지우기]](#clear-a-calendar)

#### [!UICONTROL 일정 나열]

이 작업 모듈은 사용자의 달력 목록에 있는 달력을 반환합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 달력 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최소 액세스 역할]</td> 
   <td> <p>사용자의 최소 액세스 역할을 선택합니다. 모듈은 이 최소 액세스 역할에 따라 달력을 반환합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: 사용자는 약속 있음/없음 정보를 읽을 수 있습니다. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: 사용자는 이벤트를 읽고 수정할 수 있으며 컨트롤 목록에 액세스할 수 있습니다. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: 사용자는 비공개 이벤트가 아닌 이벤트를 읽을 수 있습니다. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: 사용자는 이벤트를 읽고 수정할 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 숨겨진 달력 표시]</td> 
   <td>모듈에서 반환하는 목록에 숨겨진 달력을 포함하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 일정 수 설정 [!DNL Workfront Fusion] 한 실행 주기 동안 를 반환합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 가져오기]

이 작업 모듈은 달력을 검색합니다.

검색할 달력의 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td> <p>검색할 달력을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 만들기]

이 작업 모듈은 새 달력을 만듭니다.

달력의 이름을 지정합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 달력 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 이름]</td> 
   <td> <p> 새 달력의 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 업데이트]

이 작업 모듈은 달력을 업데이트합니다.

업데이트할 달력의 ID를 지정합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 달력 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>업데이트할 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 이름]</td> 
   <td> <p> 달력의 새 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 삭제]

이 작업 모듈은 달력을 삭제합니다.

삭제할 달력의 ID를 지정합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 달력 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td> <p>삭제할 달력의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 지우기]

이 작업 모듈은 계정의 기본 달력에서 모든 이벤트를 제거합니다.

지울 달력이 포함된 계정에 연결하는 연결을 지정합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 달력 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### 액세스 제어 규칙

* [[!UICONTROL 액세스 제어 규칙 나열]](#list-access-control-rules)
* [[!UICONTROL 액세스 제어 규칙 가져오기]](#get-an-access-control-rule)
* [[!UICONTROL 액세스 제어 규칙 만들기]](#create-an-access-control-rule)
* [[!UICONTROL 액세스 제어 규칙 업데이트]](#update-an-access-control-rule)
* [[!UICONTROL 액세스 제어 규칙 삭제]](#delete-an-access-control-rule)

#### [!UICONTROL 액세스 제어 규칙 나열]

이 작업 모듈은 달력의 액세스 제어 목록에 있는 규칙을 반환합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td> <p>검색할 액세스 제어 규칙이 포함된 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 한 실행 주기 동안 를 반환합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 액세스 제어 규칙 가져오기]

이 작업 모듈은 액세스 제어 규칙의 메타데이터를 반환합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td> <p>검색할 액세스 제어 규칙이 포함된 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 액세스 제어 규칙 ID]</td> 
   <td>검색할 액세스 제어 규칙을 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 액세스 제어 규칙 만들기]

이 작업 모듈은 새 액세스 제어 규칙을 만듭니다.

달력의 이름을 지정합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 액세스 제어 규칙의 ID 및 관련 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>액세스 제어 규칙을 만들 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 역할]</td> 
   <td> <p>액세스 규칙에 지정할 역할을 선택합니다. </p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: 사용자는 약속 있음/없음 정보를 읽을 수 있습니다. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: 사용자는 이벤트를 읽고 수정할 수 있으며 컨트롤 목록에 액세스할 수 있습니다. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: 사용자는 비공개 이벤트가 아닌 이벤트를 읽을 수 있습니다. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: 사용자는 이벤트를 읽고 수정할 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>범위 유형을 선택합니다. </p> 
    <ul> 
     <li><strong>[!UICONTROL Default]</strong>: 공개 범위. 기본값이 됩니다. </li> 
     <li><strong>[!UICONTROL User]</strong>: 범위를 단일 사용자로 제한합니다. </li> 
     <li><strong>[!UICONTROL Group]</strong>: 범위를 그룹으로 제한합니다. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: 범위를 도메인으로 제한합니다. </li> 
    </ul> <p>참고: [!UICONTROL Default] 또는 공개에 부여된 권한은 인증되거나 인증되지 않은 모든 사용자에게 적용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td>범위 유형에 따라 사용자 또는 그룹의 이메일 주소 또는 도메인 이름을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 알림 보내기]</td> 
   <td> <p>액세스 변경에 대한 알림을 전송하려면 이 옵션을 활성화합니다. </p> <p>참고: 액세스 제거에 대한 알림이 없습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 액세스 제어 규칙 업데이트]

이 작업 모듈은 액세스 제어 규칙을 업데이트합니다.

달력의 이름을 지정합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 액세스 제어 규칙의 ID 및 관련 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>업데이트할 액세스 제어 규칙이 포함된 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 액세스 제어 규칙 ID]</td> 
   <td>업데이트할 액세스 제어 규칙을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 역할]</td> 
   <td> <p>액세스 규칙에 지정할 역할을 선택합니다. </p> 
    <ul> 
     <li><strong>[!UICONTROL None]</strong>: 이 역할에서는 액세스할 수 없습니다.</li> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: 사용자는 약속 있음/없음 정보를 읽을 수 있습니다. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: 사용자는 이벤트를 읽고 수정할 수 있으며 컨트롤 목록에 액세스할 수 있습니다. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: 사용자는 비공개 이벤트가 아닌 이벤트를 읽을 수 있습니다. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: 사용자는 이벤트를 읽고 수정할 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 알림 보내기]</td> 
   <td> <p>액세스 변경에 대한 알림을 전송하려면 이 옵션을 활성화합니다. </p> <p>참고: 액세스 제거에 대한 알림이 없습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 액세스 제어 규칙 삭제]

이 작업 모듈은 액세스 제어 규칙을 삭제합니다.

달력의 이름을 지정합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 액세스 제어 규칙의 ID 및 관련 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 달력 ID]</td> 
   <td> <p>삭제할 액세스 제어 규칙이 포함된 달력의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 액세스 제어 규칙 ID]</td> 
   <td>삭제할 액세스 제어 규칙의 ID를 선택하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 반복기(더 이상 사용되지 않음)

다음 [!UICONTROL 첨부 파일 반복] 및 [!UICONTROL 참석자 상호 작용] 모듈은 더 이상 사용되지 않습니다. 첨부 파일 또는 참석자를 반복하려면 [!UICONTROL 흐름 제어] > [!UICONTROL 반복기] 모듈. 자세한 내용은 [의 반복기 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### 기타

* [[!UICONTROL API 호출 만들기]](#make-an-api-call)
* [[!UICONTROL 약속 있음/없음 정보 받기]](#get-freebusy-information)

#### [!UICONTROL API 호출 만들기]

이 모듈에서 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Google Calendar] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>상대 경로 입력 <code>https://www.googleapis.com/calendar</code>. 예: <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다. 예: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:   <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 약속 있음/없음 정보 받기]

이 작업 모듈은 일정 집합에 대한 약속 있음/없음 정보를 반환합니다.

이 모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 달력 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>연결 방법에 대한 지침은 [!DNL Google Calendar] Workfront Fusion 계정, <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion에 대한 연결 만들기 - 기본 지침</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 최소 시간]</td> 
   <td> <p> 정보를 검색할 간격의 시작을 입력합니다.</p> <p> 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 최대 시간]</td> 
   <td> <p> 정보를 검색할 간격의 끝을 입력합니다. </p> <p>지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>정보를 검색할 각 달력에 대해 <strong>추가</strong> 달력 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 이벤트 전에 시나리오 트리거

표준 지원을 사용하여 이벤트 전에 지정된 시간에 시나리오를 트리거할 수 있습니다 [!DNL Google Calendar] 전자 메일 미리 알림 및 [!UICONTROL Webhooks] >[!UICONTROL 사용자 지정 메일 후크] 모듈.

1. 를 사용하십시오 [!UICONTROL Google 달력] >[!UICONTROL 이벤트 업데이트] 전자 메일 미리 알림을 이벤트에 추가하는 모듈:

   ![](assets/trigger-scen-before-event-350x209.png)

1. 다음으로 시작하는 새 시나리오 만들기 [!UICONTROL Webhooks] >[!UICONTROL 사용자 지정 메일 후크] 모듈.

   1. 메일 후크의 이메일 주소를 복사합니다.
   1. 시나리오를 저장하고 실행합니다.

1. in [!DNL Gmail], 리디렉션 [!DNL Google Calendar] 전자 메일 미리 알림을 메일 후크 전자 메일 주소로 보냅니다.

   1. 다음 문서를 엽니다. **[!UICONTROL [!DNL Gmail]설정]**.
   1. 를 엽니다. **[!UICONTROL 전달 및 POP/IMAP]** 탭.
   1. 클릭 **[!UICONTROL 전달 주소 추가].**
   1. 복사한 mailhooks의 전자 메일 주소를 붙여 넣고 을 클릭합니다&#x200B;.**[!UICONTROL 다음]**, 확인 **[!UICONTROL 계속]** 팝업 창에서 **[!UICONTROL 확인]**.

   1. in [!DNL Workfront Fusion]확인 이메일을 수신하여 실행을 완료해야 하는 새 시나리오로 전환합니다.
   1. 모듈 위의 버블을 클릭하여 모듈의 출력을 검사합니다.
   1. 를 확장합니다. `Text` 항목을 선택하고 확인 코드를 복사합니다.

      ![](assets/confirmation-code-350x252.png)

   1. Gmail에서 편집 상자에 확인 코드를 붙여 넣고 을 &#x200B; 클릭합니다&#x200B;**[!UICONTROL 확인]**:

      ![](assets/paste-code-350x46.png)

   1. 를 엽니다. **[!UICONTROL 필터 및 차단된 주소]** 탭.
   1. 클릭 **[!UICONTROL 새 필터 만들기]**.
   1. 에서 오는 모든 이메일에 대한 필터 설정 `     calendar-notification@google.com` 을 클릭합니다&#x200B;.**[!UICONTROL 필터 만들기]**:
   1. 선택 **[!UICONTROL 전달]** 및 목록에서 mailhooks의 이메일 주소를 선택합니다.
   1. 클릭 **[!UICONTROL 필터 만들기]** 필터를 만듭니다.

1. (선택 사항) in [!DNL Workfront Fusion], 추가 [!UICONTROL 텍스트 파서] > [!UICONTROL 일치 패턴] 모듈 뒤 [!UICONTROL Webhooks] >[!UICONTROL 사용자 지정 메일 후크] 필요한 정보를 얻기 위해 이메일의 HTML 코드를 구문 분석하는 모듈입니다.

   예를 들어 다음과 같이 모듈을 구성하여 이벤트의 ID를 가져올 수 있습니다.

   *패턴*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *텍스트*: 다음 `HTML content` 에서 출력된 항목 [!UICONTROL Webhooks] >[!UICONTROL 사용자 지정 메일 후크] 모듈.
