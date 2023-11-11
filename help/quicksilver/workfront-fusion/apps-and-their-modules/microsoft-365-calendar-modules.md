---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 달력
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 Microsoft Office 365 캘린더를 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Microsoft Office 365 Calendar]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

를 사용하려면 [!DNL Office 365 Calendar] 포함 [!DNL Adobe Workfront Fusion], 다음을 수행해야 합니다. [!DNL Office 365 Excel] 계정입니다. 다음 위치에 만들 수 있습니다. [www.office.com](https://www.office.com/).

Office 365 계정 연결에 대한 자세한 내용 [!DNL Workfront Fusion], 참조 [Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

동의를 부여하면 다시 로 리디렉션됩니다. [!UICONTROL Workfront Fusion] 시나리오를 계속 만들 수 있는 관리 페이지

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
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

사용 [!DNL Microsoft Office 365 Calendar] 모듈, 다음이 있어야 합니다. [!DNL Microsoft Office 365 Calendar] 계정입니다.

## [!DNL Microsoft Office 365 Calendar] 모듈 및 해당 필드

를 구성할 때 [!DNL Microsoft Office 365 Calendar] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Microsoft Office 365 Calendar] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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

이 트리거 모듈은 선택한 달력에서 이벤트가 생성, 업데이트, 삭제, 시작 또는 종료될 때 이벤트의 세부 정보를 검색합니다.

>[!NOTE]
>
>이벤트 시리즈의 삭제된 발생 횟수를 보려면 다음을 선택합니다. [!UICONTROL 업데이트한 시간별] 다음에서 [!UICONTROL 이벤트 보기] 필드. 이 모듈은 삭제된 단일 이벤트 또는 삭제된 이벤트 시리즈를 감시하지 않습니다.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 감시 이벤트]</td> 
   <td> <p>이벤트 시청 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>만든 시간별 [!UICONTROL]</strong> </p> <p>새로운 이벤트를 확인하십시오.</p> </li> 
     <li> <p><strong>업데이트된 시간별 [!UICONTROL]</strong> </p> <p>업데이트된 이벤트를 확인하십시오.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 그룹 ID]</td> 
   <td>이벤트를 보려는 캘린더가 포함된 [!UICONTROL 캘린더 그룹]을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>보려는 특정 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>필터 조건을 설정하여 결과를 주제, 이벤트 ID 또는 본문별로 필터링합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>최대 메시지 수 입력 [!DNL Workfront Fusion] 한 시나리오 실행 주기 중에 를 반환해야 합니다.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 그룹 ID]</td> 
   <td>이벤트를 보려는 캘린더가 포함된 [!UICONTROL 캘린더 그룹]을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>보려는 특정 달력을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>결과를 필터링하려면 필터 조건을 설정하십시오. 다음 속성을 기준으로 필터링할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL Subject]</li> 
     <li>[!UICONTROL 이벤트 ID]</li> 
     <li>[!UICONTROL 만든 날짜 시간]</li> 
     <li>[!UICONTROL 마지막 수정 날짜 시간]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>결과 정렬 방법을 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, 오름차순 또는 내림차순</li> 
     <li><strong>[!UICONTROL 만든 날짜 시간]</strong>, 오름차순 또는 내림차순</li> 
     <li><strong>[!UICONTROL 마지막 수정 날짜 시간]</strong>, 오름차순 또는 내림차순</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 이벤트 수 입력 [!DNL Workfront Fusion] 한 시나리오 실행 주기 중에 를 반환해야 합니다.</td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td> <p>세부 정보를 검색할 이벤트 ID를 입력하거나 매핑합니다.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>생성된 이벤트의 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
   <td> 결합된 날짜 및 시간 표현에서 이벤트가 시작되는 단일 시점을 입력합니다. 형식 사용 <code>({date}T{time}</code>; 예, <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오. <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 변환 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 날짜]</td> 
   <td> 이벤트가 결합된 날짜 및 시간 표시로 끝나는 단일 시점을 입력합니다. 형식 사용 <code>{date}T{time}</code>; 예, <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오. <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 변환 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 미리 알림 설정]</td> 
   <td>이 이벤트에 대한 미리 알림을 활성화할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 알림 메시지]</td> 
   <td>미리 알림이 트리거되어야 하는 이벤트 시작 전 시간(분)을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 중요도]</td> 
   <td> <p>이 이벤트의 중요도를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 낮음]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL 높음]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 감도] </td> 
   <td> <p>이 이벤트의 민감도를 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>수신자에게 "[!UICONTROL Please treat this as Personal]" 메시지가 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>수신자에게 "[!UICONTROL Please treat this as Private]" 메시지가 표시됩니다. 이 이벤트는 수신자의 받은 편지함 규칙에 의해 전달되거나 리디렉션되지 않습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>수신자에게 "[!UICONTROL 기밀 정보로 취급하십시오]" 메시지가 표시됩니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 본문 컨텐츠 유형]</td> 
   <td>본문 컨텐츠가 일반 텍스트인지 HTML인지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>이벤트와 연계된 메시지 본문을 입력하거나 매핑합니다. HTML 또는 텍스트 형식일 수 있습니다(위의 [!UICONTROL Body Content Type] 필드에 지정된 대로).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 위치]</td> 
   <td> <p>이벤트 위치 세부 정보를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응답 요청됨]</td> 
   <td>선택 <strong>[!UICONTROL 예]</strong> 초대받은 사람에게 이벤트 초대에 대한 응답을 보내도록 요청합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 다음으로 표시]</td> 
   <td> <p>캘린더를 보는 사람에게 이벤트를 표시할 방법을 선택하십시오.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL 미정]</li> 
     <li>[!UICONTROL 사용 중]</li> 
     <li>[!UICONTROL 부재 중]</li> 
     <li>[!UICONTROL 다른 곳에서 작동]</li> 
     <li>[!UICONTROL 알 수 없음]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 참석자]</p> </td> 
   <td> <p>이벤트 참석자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 이름]</strong> </p> <p>참석자의 이름을 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>참석자의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 범주]</td> 
   <td>이벤트를 캘린더에 표시할 범주를 입력하거나 매핑합니다.</td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td>업데이트하려는 이벤트의 ID를 입력하거나 매핑하거나 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>생성된 이벤트의 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜]</td> 
   <td> 결합된 날짜 및 시간 표현에서 이벤트가 시작되는 단일 시점을 입력합니다. 형식 사용 <code>{date}T{time}</code>; 예, <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오. <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 변환 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 종료 날짜]</td> 
   <td> 이벤트가 결합된 날짜 및 시간 표시로 끝나는 단일 시점을 입력합니다. 형식 사용 <code>({date}T{time}</code>; 예, <code>2017-08-29T04:00:00.0000000</code>. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오. <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 변환 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 미리 알림 설정]</td> 
   <td>이 이벤트에 대한 미리 알림을 활성화할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 알림 메시지]</td> 
   <td>미리 알림이 트리거되어야 하는 이벤트 시작 전 시간(분)을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 중요도]</td> 
   <td> <p>이 이벤트의 중요도를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 낮음]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL 높음]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 감도] </td> 
   <td> <p>이 이벤트의 민감도를 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>수신자에게 "[!UICONTROL Please treat this as Personal]" 메시지가 표시됩니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>수신자에게 "[!UICONTROL Please treat this as Private]" 메시지가 표시됩니다. 이 이벤트는 수신자의 받은 편지함 규칙에 의해 전달되거나 리디렉션되지 않습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>수신자에게 "[!UICONTROL 기밀 정보로 취급하십시오]" 메시지가 표시됩니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 본문 컨텐츠 유형]</td> 
   <td>이벤트와 연결된 메시지의 본문 콘텐츠가 일반 텍스트인지 아니면 HTML인지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>이벤트와 연계된 메시지 본문을 입력하거나 매핑합니다. HTML 또는 텍스트 형식일 수 있습니다(위의 [!UICONTROL Body Content Type] 필드에 지정된 대로).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 위치]</td> 
   <td> <p>이벤트 위치 세부 정보를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 응답 요청됨]</td> 
   <td>선택 <strong>[!UICONTROL 예]</strong> 초대받은 사람에게 이벤트 초대에 대한 응답을 보내도록 요청합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 다음으로 표시]</td> 
   <td> <p>캘린더를 보는 사람에게 이벤트를 표시할 방법을 선택하십시오.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL 미정]</li> 
     <li>[!UICONTROL 사용 중]</li> 
     <li>[!UICONTROL 부재 중]</li> 
     <li>[!UICONTROL 다른 곳에서 작동]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 참석자]</p> </td> 
   <td> <p>이벤트 참석자를 추가합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 이름]</strong> </p> <p>참석자의 이름을 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>참석자의 이메일 주소를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 범주]</td> 
   <td>이벤트를 캘린더에 표시할 범주를 입력하거나 매핑합니다.</td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이벤트 ID]</td> 
   <td> <p>삭제할 이벤트의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 캘린더

* [[!UICONTROL 목록 캘린더]](#list-calendars)
* [[!UICONTROL 캘린더 가져오기]](#get-a-calendar)
* [[!UICONTROL 캘린더 만들기]](#create-a-calendar)
* [[!UICONTROL 캘린더 업데이트]](#update-a-calendar)
* [[!UICONTROL 캘린더 삭제]](#delete-a-calendar)

#### [!UICONTROL 목록 캘린더]

이 검색 모듈은 인증된 사용자의 모든 캘린더 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 그룹 ID]</td> 
   <td>나열할 캘린더가 포함된 [!UICONTROL 캘린더 그룹]을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 달력 수 입력 [!DNL Workfront Fusion] 한 시나리오 실행 주기 중에 를 반환해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 캘린더 가져오기]

이 작업 모듈은 단일 캘린더에 대한 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td> <p>세부 정보를 검색할 달력의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 캘린더 만들기]

이 작업 모듈은 Google 계정에 새 달력을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar name]</td> 
   <td> <p>새 캘린더의 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 캘린더 업데이트]

이 작업 모듈은 기존 캘린더를 편집합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td>업데이트하려는 캘린더의 [!UICONTROL 캘린더 ID]를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 캘린더 이름]</td> 
   <td> <p>새 캘린더의 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 캘린더 삭제]

이 작업 모듈은 기존 캘린더를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 ID]</td> 
   <td>삭제할 달력의 [!UICONTROL Calendar] ID를 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 기타

#### [!UICONTROL API 호출 만들기]

이 모듈에서는 사용자 지정 API 호출을 수행할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Office 365] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">에 대한 연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
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
   <td> <p>표준 JSON 개체 형식으로 요청의 헤더를 추가합니다.예: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p> 표준 JSON 개체 형식으로 API 호출에 대한 쿼리를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:   <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
