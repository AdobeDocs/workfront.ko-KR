---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: GitHub 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오는 GitHub를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!UICONTROL GitHub]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL GitHub] 모듈이면 [!DNL GitHub] 계정이 필요합니다.

## Connect [!DNL GitHub] to [!DNL Workfront Fusion]

연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!UICONTROL Workfront Fusion]를 참조하십시오. [연결 만들기 [!UICONTROL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] 모듈 및 해당 필드.

구성 시 [!DNL GitHub] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL GitHub] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)

### Triggers

* [[!UICONTROL 감시 문제]](#watch-issues)
* [[!UICONTROL 저장소 보기]](#watch-repositories)
* [[!UICONTROL 포크 보기]](#watch-forks)
* [[!UICONTROL 댓글 보기]](#watch-comments)
* [[!UICONTROL 가져오기 요청 보기]](#watch-pull-requests)

#### [!UICONTROL 감시 문제]

이 모듈은 새 문제가 추가되거나 기존 문제가 수정되면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보고 싶습니다]</td> 
   <td>모든 리포지토리를 표시할지 아니면 한 저장소만 볼지를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>한 저장소에서만 문제를 확인하도록 선택한 경우 보려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 문제 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 문제만 감시할지, 새 문제와 모든 변경 사항을 감시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>감시하려는 문제를 관련된 방식으로 필터링할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL 모든 문제]</li> 
     <li>[!UICONTROL 나에게 할당된 문제만]</li> 
     <li>[!UICONTROL만 내가 만든 문제]</li> 
     <li>[!UICONTROL 나를 언급하는 문제만]</li> 
     <li>[!UICONTROL 업데이트 구독 중인 문제만]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>열려 있는 문제만 표시할지 아니면 닫힌 문제만 감시할지를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블]</td> 
   <td>태그를 추가합니다. 모듈은 이 태그의 문제를 확인합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 저장소 보기]

이 모듈은 저장소가 만들어지거나 수정되면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 저장소 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 리포지토리와 모든 변경 내용을 감시할지 또는 새 리포지토리만 보호할지 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 포크 보기]

이 모듈은 새 포크를 만들 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>포크를 감시하려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 포크 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 보기]

이 모듈은 새 주석이 추가되거나 기존 주석이 수정될 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>보려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제 번호]</td> 
   <td>특정 문제에 대한 새 주석만 검색하여 검색을 제한하려면 문제 번호를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 문제 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 주석이나 주석 및 모든 변경 사항에 대해 감시할지 여부를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 가져오기 요청 보기]

이 모듈은 새 가져오기 요청이 추가되거나 기존 가져오기 요청이 수정되면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>보려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 끌어오기 요청 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>[!UICONTROL만 열린 끌어오기] 요청만 감시할지, [!UICONTROL만 닫힌 끌어오기] 요청만 감시할지, 아니면 모든 끌어오기 요청을 감시할지를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 풀 요청만 감시할지, 새 풀 요청과 모든 변경 사항을 감시할지 여부를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 문제 검색]](#search-for-an-issue)
* [[!UICONTROL 문제 만들기]](#create-an-issue)
* [[!UICONTROL 문제 업데이트]](#update-an-issue)
* [[!UICONTROL 문제 가져오기]](#get-an-issue)
* [[!UICONTROL 할당 추가]](#add-assignees)
* [[!UICONTROL 할당 제거]](#remove-assignees)
* [[!UICONTROL 문제에 레이블 추가]](#add-labels-to-an-issue)
* [[!UICONTROL 문제에 대한 레이블 제거]](#remove-a-label-from-an-issue)
* [[!UICONTROL 댓글 만들기]](#create-a-comment)
* [[!UICONTROL 주석 나열]](#list-comments)

#### [!UICONTROL 문제 검색]

이 모듈은 검색 기준과 일치하는 문제를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 문제 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 주기 동안(시나리오 실행당 반복 횟수) 작동합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>검색 결과를 정렬할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Best Match] </p> </li> 
     <li>[!UICONTROL 만든 날짜]</li> 
     <li>[!UICONTROL 업데이트 날짜]</li> 
     <li>[!UICONTROL 주석 수]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 방향]</td> 
   <td> <p>오름차순 또는 내림차순을 선택합니다. </p> <p>날짜의 경우 <strong>[!UICONTROL 내림차순]</strong> 은 가장 최근 날짜를 먼저 반환합니다. </p> <p>[!UICONTROL Number of Comments]의 경우 <strong>[!UICONTROL 내림차순]</strong> 에서는 먼저 가장 많은 수의 주석이 있는 문제를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>검색 쿼리를 입력하거나 매핑합니다. 검색 옵션에 대한 자세한 설명은 다음을 참조하십시오 <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">문제 및 가져오기 요청 검색</a> on [!DNL GitHub] 도움말 사이트입니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제 만들기]

이 모듈은 선택한 리포지토리에 새 문제를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>에서 문제를 생성할 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>문제에 지정할 사람을 선택합니다. 사용 가능한 할당자에는 리포지토리에 대한 쓰기 권한이 있는 모든 사용자와 리포지토리에 대한 읽기 권한이 있는 조직 구성원이 포함됩니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이정표]</td> 
   <td>새 문제와 연결할 이정표를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블]</td> 
   <td>새 문제에 적용할 레이블을 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>새 문제에 대한 제목을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>설명 또는 추가 정보와 같은 문제 본문을 입력하거나 매핑합니다</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제 업데이트]

이 모듈은 기존 [!DNL GitHub] 문제.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>에서 문제를 업데이트할 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>문제에 지정할 사람을 선택합니다. 사용 가능한 할당자에는 리포지토리에 대한 쓰기 권한이 있는 모든 사용자와 리포지토리에 대한 읽기 권한이 있는 조직 구성원이 포함됩니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이정표]</td> 
   <td>문제와 연결할 이정표를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블]</td> 
   <td>문제에 적용할 레이블을 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>업데이트할 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>문제를 업데이트할 상태를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>문제에 대한 제목을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>설명 또는 추가 정보와 같은 문제 본문을 입력하거나 매핑합니다</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제 가져오기]

이 모듈은 지정된 문제에 대한 세부 정보를 검색합니다

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>세부 정보를 검색할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>세부 사항을 검색할 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 할당 추가]

이 모듈은 지정된 문제에 담당자를 추가합니다

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>담당자를 추가할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>문제에 지정할 사람을 선택합니다. 사용 가능한 할당자에는 리포지토리에 대한 쓰기 권한이 있는 모든 사용자와 리포지토리에 대한 읽기 권한이 있는 조직 구성원이 포함됩니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>담당자를 추가할 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 할당 제거]

이 모듈은 지정된 문제로부터 담당자를 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>할당을 제거할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignee]</td> 
   <td>문제와 제거할 사람을 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>담당자를 제거할 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제에 레이블 추가]

이 모듈은 문제에 레이블을 추가합니다. 레이블은 저장소 수준에서 정의되며 리포지토리에 대한 쓰기 액세스 권한이 있는 사용자만 생성할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>레이블을 추가할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블]</td> 
   <td>문제에 추가할 레이블을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>레이블을 추가할 문제의 문제 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제에 대한 레이블 제거]

이 모듈은 문제의 단일 레이블을 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>레이블을 제거할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블]</td> 
   <td>문제와 관련하여 제거할 레이블을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>레이블을 제거할 문제의 문제 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 만들기]

이 모듈은 지정된 문제에 대한 설명을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>주석을 작성할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>주석을 작성할 문제의 문제 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>주석의 컨텐츠를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 주석 나열]

이 모듈에는 지정된 문제에 대한 모든 주석이 나열됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL GitHub] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>설명을 나열할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>설명을 나열할 문제의 문제 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>모듈은 이 날짜 이후에 생성된 주석을 반환합니다. 지원되는 날짜 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 주석 수]</td> 
   <td>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다. </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
