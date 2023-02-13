---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 일정
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오 Microsoft Office 365 Calendar를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1835'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Microsoft Office 365 Calendar]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

를 사용하려면 [!DNL Office 365 Calendar] with [!DNL Adobe Workfront Fusion]를 채울 때는 [!DNL Office 365 Excel] 계정이 필요합니다. 에서 만들 수 있습니다 [www.office.com](http://www.office.com/).

Office 365 계정 연결에 대한 지침은 [!DNL Workfront Fusion]를 참조하십시오. [Adobe 연결 만들기 [!DNL Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

동의를 부여하면 다음 위치로 다시 리디렉션됩니다. [!UICONTROL Workfront Fusion] 시나리오를 계속 작성할 수 있는 관리 페이지입니다.

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

를 사용하려면 [!DNL Microsoft Office 365 Calendar] 모듈이면 반드시 [!DNL Microsoft Office 365 Calendar] 계정이 필요합니다.

## [!DNL Microsoft Office 365 Calendar] 모듈 및 해당 필드

구성 시 [!DNL Microsoft Office 365 Calendar] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Microsoft Office 365 Calendar] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Event](#event)
* [캘린더](#calendar)
* [기타](#other)

### Event

* [[!UICONTROL 이벤트 보기]](#watch-events)
* [[!UICONTROL 이벤트 검색]](#search-events)
* [[!UICONTROL 이벤트 가져오기]](#get-an-event)
* [[!UICONTROL 이벤트 만들기]](#create-an-event)
* [[!UICONTROL 이벤트 업데이트]](#update-an-event)
* [[!UICONTROL 이벤트 삭제]](#delete-an-event)

#### [!UICONTROL 이벤트 보기]

이 트리거 모듈은 선택한 달력에서 이벤트가 생성, 업데이트, 삭제, 시작 또는 종료될 때 이벤트의 세부 사항을 검색합니다.

>[!NOTE]
>
>이벤트 시리즈의 삭제된 발생 항목을 보려면 [!UICONTROL 업데이트한 시간] 에서 [!UICONTROL 이벤트 보기] 필드. 이 모듈은 삭제된 단일 이벤트 또는 삭제된 이벤트 시리즈를 감시하지 않습니다.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch 이벤트]</td> 
   <td> <p>이벤트를 볼 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By Created Time]</strong> </p> <p>새로운 이벤트를 확인하십시오.</p> </li> 
     <li> <p><strong>[!UICONTROL By Updated Time]</strong> </p> <p>업데이트된 이벤트를 확인하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 그룹 ID]</td> 
   <td>이벤트를 볼 달력이 포함된 [!UICONTROL 달력 그룹]을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>보려는 특정 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>결과를 제목, 이벤트 ID 또는 본문별로 필터링하려면 필터 조건을 설정합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>최대 메시지 수를 입력합니다 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 검색]

이 검색 모듈은 선택한 달력에서 이벤트가 생성, 업데이트, 삭제, 시작 또는 종료될 때 이벤트의 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 그룹 ID]</td> 
   <td>이벤트를 볼 달력이 포함된 [!UICONTROL 달력 그룹]을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>보려는 특정 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>필터 조건을 설정하여 결과를 필터링합니다. 다음 속성으로 필터링할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL Subject]</li> 
     <li>[!UICONTROL 이벤트 ID]</li> 
     <li>[!UICONTROL Created Date Time]</li> 
     <li>[!UICONTROL Last Modified Date Time]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>결과를 정렬할 방법을 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, 오름차순 또는 내림차순</li> 
     <li><strong>[!UICONTROL Created Date Time]</strong>, 오름차순 또는 내림차순</li> 
     <li><strong>[!UICONTROL Last Modified Date Time]</strong>, 오름차순 또는 내림차순</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 이벤트 수 입력 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 가져오기]

이 작업 모듈은 지정된 이벤트의 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td> <p>세부 사항을 검색할 이벤트의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 만들기]

이 작업 모듈은 새 이벤트를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>생성된 이벤트의 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
   <td> 이벤트가 결합된 날짜 및 시간 표현으로 시작하는 단일 시점을 입력합니다. 형식 사용 <code>({date}T{time}</code>; 예 <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 날짜]</td> 
   <td> 이벤트가 결합된 날짜 및 시간 표현으로 끝나는 단일 시점을 입력합니다. 형식 사용 <code>{date}T{time}</code>; 예 <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 미리 알림 온]</td> 
   <td>이 이벤트에 대한 미리 알림을 활성화할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 미리 알림]</td> 
   <td>미리 알림을 트리거해야 하는 이벤트 시작 전 분 수를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>이 이벤트의 중요도를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 민감도] </td> 
   <td> <p>이 이벤트의 민감도를 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>수신자에게는 "[!UICONTROL 개인]" 메시지가 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>수신자에게는 "[!UICONTROL 이것을 Private]" 메시지가 표시됩니다. 이 이벤트는 수신자의 받은 편지함 규칙에 의해 전달되거나 리디렉션되지 않습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>수신자에게는 "[!UICONTROL 이것을 기밀]으로 취급하십시오" 메시지가 표시됩니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body 콘텐츠 형식]</td> 
   <td>본문 내용이 일반 텍스트인지 HTML인지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>이벤트와 연관된 메시지 본문을 입력하거나 매핑합니다. HTML 또는 텍스트 형식(위의 [!UICONTROL Body Content Type] 필드에 지정됨)일 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>이벤트 위치 세부 사항을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응답 요청]</td> 
   <td>선택 <strong>[!UICONTROL Yes]</strong> 초대받은 사람에게 이벤트 초대에 대한 응답을 보내도록 요청하려면</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 다른 이름으로 표시]</td> 
   <td> <p>일정을 보는 사람에게 이벤트를 표시할 방법을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL 임시]</li> 
     <li>[!UICONTROL 사용 중]</li> 
     <li>[!UICONTROL 부재 중]</li> 
     <li>[!UICONTROL 다른 곳에서 작업]</li> 
     <li>[!UICONTROL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 참석자]</p> </td> 
   <td> <p>이벤트의 참석자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>참석자의 이름을 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>참석자의 전자 메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>일정에서 이벤트를 표시할 카테고리를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 업데이트]

이 작업 모듈은 기존 이벤트를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td>업데이트할 이벤트의 ID를 입력, 매핑 또는 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>생성된 이벤트의 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
   <td> 이벤트가 결합된 날짜 및 시간 표현으로 시작하는 단일 시점을 입력합니다. 형식 사용 <code>{date}T{time}</code>; 예 <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 날짜]</td> 
   <td> 이벤트가 결합된 날짜 및 시간 표현으로 끝나는 단일 시점을 입력합니다. 형식 사용 <code>({date}T{time}</code>; 예 <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 미리 알림 온]</td> 
   <td>이 이벤트에 대한 미리 알림을 활성화할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 미리 알림]</td> 
   <td>미리 알림을 트리거해야 하는 이벤트 시작 전 분 수를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>이 이벤트의 중요도를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 민감도] </td> 
   <td> <p>이 이벤트의 민감도를 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>수신자에게는 "[!UICONTROL 개인]" 메시지가 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>수신자에게는 "[!UICONTROL 이것을 Private]" 메시지가 표시됩니다. 이 이벤트는 수신자의 받은 편지함 규칙에 의해 전달되거나 리디렉션되지 않습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>수신자에게는 "[!UICONTROL 이것을 기밀]으로 취급하십시오" 메시지가 표시됩니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body 콘텐츠 형식]</td> 
   <td>이벤트와 연결된 메시지의 본문 내용이 일반 텍스트인지 HTML인지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>이벤트와 연관된 메시지 본문을 입력하거나 매핑합니다. HTML 또는 텍스트 형식(위의 [!UICONTROL Body Content Type] 필드에 지정됨)일 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>이벤트 위치 세부 사항을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응답 요청]</td> 
   <td>선택 <strong>[!UICONTROL Yes]</strong> 초대받은 사람에게 이벤트 초대에 대한 응답을 보내도록 요청하려면</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 다른 이름으로 표시]</td> 
   <td> <p>일정을 보는 사람에게 이벤트를 표시할 방법을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL 임시]</li> 
     <li>[!UICONTROL 사용 중]</li> 
     <li>[!UICONTROL 부재 중]</li> 
     <li>[!UICONTROL 다른 곳에서 작업]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 참석자]</p> </td> 
   <td> <p>이벤트의 참석자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>참석자의 이름을 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>참석자의 전자 메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>일정에서 이벤트를 표시할 카테고리를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이벤트 삭제]

이 작업 모듈은 기존 이벤트를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td> <p>삭제할 이벤트의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 캘린더

* [[!UICONTROL 일정 나열]](#list-calendars)
* [[!UICONTROL 달력 가져오기]](#get-a-calendar)
* [[!UICONTROL 달력 만들기]](#create-a-calendar)
* [[!UICONTROL 달력 업데이트]](#update-a-calendar)
* [[!UICONTROL 달력 삭제]](#delete-a-calendar)

#### [!UICONTROL 일정 나열]

이 검색 모듈은 인증된 사용자의 모든 달력 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 그룹 ID]</td> 
   <td>나열할 달력이 포함된 [!UICONTROL 달력 그룹]을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 달력 수를 입력합니다 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 가져오기]

이 작업 모듈은 단일 달력에 대한 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td> <p>세부 사항을 검색할 달력의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 만들기]

이 작업 모듈은 Google 계정에 새 달력을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 이름]</td> 
   <td> <p>새 달력의 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 업데이트]

이 작업 모듈은 기존 달력을 편집합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td>업데이트할 달력의 [!UICONTROL 달력 ID]을 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 달력 이름]</td> 
   <td> <p>새 달력의 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 달력 삭제]

이 작업 모듈은 기존 달력을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td>삭제할 달력의 [!UICONTROL Calendar] ID를 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 기타

#### [!UICONTROL API 호출 만들기]

이 모듈에서 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Office 365] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>상대 경로 입력 <code>https://graph.microsoft.com</code>. 예:<code> /v1.0/me/events</code></p> </td> 
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
