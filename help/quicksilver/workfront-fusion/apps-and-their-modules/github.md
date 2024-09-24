---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: GitHub 모듈
description: ' [!DNL Adobe Workfront Fusion] 시나리오에서는 GitHub를 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 16cd5dee183153540bcccea8ce469a461d0e8562
workflow-type: tm+mt
source-wordcount: '1839'
ht-degree: 0%

---

# [!DNL GitHub]개 모듈

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!UICONTROL GitHub]를 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 전제 조건

[!DNL GitHub] 모듈을 사용하려면 [!DNL GitHub] 계정이 있어야 합니다.

## [!DNL GitHub]을(를) [!DNL Workfront Fusion]에 연결

[!DNL GitHub] 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법에 대한 지침은 [[!UICONTROL Adobe Workfront Fusion에 연결 만들기] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)을 참조하십시오.

## [!DNL GitHub]개 모듈 및 해당 필드.

[!DNL GitHub] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL GitHub] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)

### 트리거

* [[!UICONTROL 문제 보기]](#watch-issues)
* [[!UICONTROL 저장소 보기]](#watch-repositories)
* [[!UICONTROL 분기점 보기]](#watch-forks)
* [[!UICONTROL 댓글 보기]](#watch-comments)
* [[!UICONTROL 끌어오기 요청 보기]](#watch-pull-requests)

#### [!UICONTROL 문제 보기]

이 모듈은 새 문제가 추가되거나 기존 문제가 수정되면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보고 싶습니다]</td> 
   <td>모든 저장소를 감시할지 하나의 저장소만 감시할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>한 저장소에서만 문제를 확인하도록 선택한 경우 확인하려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 문제 수]</td> 
   <td>한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 문제만 감시할지, 새 문제 및 모든 변경 사항을 감시할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>감시할 문제를 연결된 방법별로 필터링할 수 있습니다.</p> 
    <ul> 
     <li>[!UICONTROL 모든 문제]</li> 
     <li>[!UICONTROL만 나에게 할당된 문제]</li> 
     <li>[!UICONTROL 내가 만든 문제만 해당]</li> 
     <li>[!UICONTROL만 나를 언급하는 문제]</li> 
     <li>[!UICONTROL 다음에 대한 업데이트를 구독하는 문제만 발생]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상태]</td> 
   <td>진행 중인 문제만 볼 것인지 종료된 문제만 볼 것인지 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블]</td> 
   <td>태그를 추가합니다. 모듈은 이 태그의 문제를 감시합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 저장소 보기]

이 모듈은 저장소가 생성되거나 수정되면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 저장소 수]</td> 
   <td>한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 저장소 및 모든 변경 사항을 감시할지 또는 새 저장소만 감시할지 여부를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 분기점 보기]

이 모듈은 새 포크를 만들 때 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>포크를 검사할 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 포크 수]</td> 
   <td>한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 보기]

이 모듈은 새 댓글이 추가되거나 기존 댓글이 수정되면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>보려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제 번호]</td> 
   <td>특정 문제에 대한 새로운 의견만 검색하여 검색을 제한하려면 문제 번호를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 문제 수]</td> 
   <td>한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 주석만 감시할지 또는 주석 및 모든 변경 사항을 감시할지 여부를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 끌어오기 요청 보기]

이 모듈은 새 끌어오기 요청이 추가되거나 기존 끌어오기 요청이 수정되면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>보려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 풀 요청 수]</td> 
   <td>한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상태]</td> 
   <td>[!UICONTROL only open pull] 요청, [!UICONTROL only closed ones] 또는 모든 pull 요청을 시청할지 여부를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>새 끌어오기 요청만 감시할지, 새 끌어오기 요청 및 모든 변경 사항을 감시할지 여부를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 문제 검색]](#search-for-an-issue)
* [[!UICONTROL 문제 만들기]](#create-an-issue)
* [[!UICONTROL 문제 업데이트]](#update-an-issue)
* [[!UICONTROL 문제 가져오기]](#get-an-issue)
* [[!UICONTROL 피할당자 추가]](#add-assignees)
* [[!UICONTROL 피할당자 제거]](#remove-assignees)
* [[!UICONTROL 문제에 레이블 추가]](#add-labels-to-an-issue)
* [[!UICONTROL 문제에서 레이블 제거]](#remove-a-label-from-an-issue)
* [[!UICONTROL 댓글 만들기]](#create-a-comment)
* [[!UICONTROL 댓글 나열]](#list-comments)

#### [!UICONTROL 문제 검색]

이 모듈은 검색 기준과 일치하는 문제를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 문제 수]</td> 
   <td>[!DNL Workfront Fusion]이(가) 한 주기 동안 사용할 최대 결과 수(시나리오 실행당 반복 횟수)를 설정하십시오. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 기준]</td> 
   <td> <p>검색 결과를 정렬할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 최적 일치] </p> </li> 
     <li>[!UICONTROL 만든 날짜]</li> 
     <li>[!UICONTROL 날짜 업데이트됨]</li> 
     <li>[!UICONTROL 댓글 수]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬 방향]</td> 
   <td> <p>오름차순 또는 내림차순을 선택합니다. </p> <p>날짜의 경우 <strong>[!UICONTROL 내림차순]</strong>을(를) 선택하면 가장 최근 날짜가 먼저 반환됩니다. </p> <p>[!UICONTROL number of comments]에 대해 <strong>[!UICONTROL descending]</strong>을(를) 선택하면 댓글 수가 가장 많은 문제가 먼저 반환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>검색 쿼리를 입력하거나 매핑합니다. 검색 옵션에 대한 자세한 설명은 [!DNL GitHub] 도움말 사이트에서 <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">문제 및 가져오기 요청 검색</a>을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제 만들기]

이 모듈은 선택한 저장소에 새 문제를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>문제를 만들려는 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 담당자]</td> 
   <td>문제에 할당할 사람을 선택합니다. 사용 가능한 할당자에는 저장소에 대한 쓰기 권한이 있는 모든 사용자와 저장소에 대한 읽기 권한이 있는 조직 구성원이 포함됩니다. </td> 
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
   <td>새 문제의 제목을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>설명 또는 추가 정보 등 문제의 본문을 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제 업데이트]

이 모듈은 기존 [!DNL GitHub] 문제를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>문제를 업데이트할 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 담당자]</td> 
   <td>문제에 할당할 사람을 선택합니다. 사용 가능한 할당자에는 저장소에 대한 쓰기 권한이 있는 모든 사용자와 저장소에 대한 읽기 권한이 있는 조직 구성원이 포함됩니다. </td> 
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
   <td>업데이트하려는 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상태]</td> 
   <td>문제를 업데이트할 상태를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>문제에 대한 제목을 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>설명 또는 추가 정보 등 문제의 본문을 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제 가져오기]

이 모듈은 지정된 문제에 대한 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>세부 정보를 가져올 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>세부 정보를 검색할 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 피할당자 추가]

이 모듈은 지정된 문제에 피할당자를 추가합니다

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>피할당자를 추가하려는 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 담당자]</td> 
   <td>문제에 할당할 사람을 선택합니다. 사용 가능한 할당자에는 저장소에 대한 쓰기 권한이 있는 모든 사용자와 저장소에 대한 읽기 권한이 있는 조직 구성원이 포함됩니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>피할당자를 추가하려는 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 피할당자 제거]

이 모듈은 지정된 문제에서 피할당자를 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>피할당자를 제거하려는 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 담당자]</td> 
   <td>문제에서 제거할 사람을 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>피할당자를 제거할 문제의 문제 번호를 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 문제에 레이블 추가]

이 모듈은 문제에 레이블을 추가합니다. 레이블은 저장소 수준에서 정의되며 저장소에 대한 쓰기 권한이 있는 사용자만 만들 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
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

#### [!UICONTROL 문제에서 레이블 제거]

이 모듈은 문제에서 단일 레이블을 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>레이블을 제거할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블]</td> 
   <td>문제에서 제거할 레이블을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>레이블을 제거할 문제의 문제 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 만들기]

이 모듈은 지정된 문제에 대한 주석을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>댓글을 작성하려는 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>댓글을 작성하려는 문제의 문제 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>주석의 내용을 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 댓글 나열]

이 모듈에는 지정된 문제에 대한 모든 주석이 나열됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL GitHub] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]에 연결 만들기 - 기본 지침</a>을 참조하세요.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장소]</td> 
   <td>의견을 나열할 문제가 포함된 저장소를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>주석을 나열할 문제의 문제 번호를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>모듈은 이 날짜 이후에 작성된 주석을 반환합니다. 지원되는 날짜 형식 목록을 보려면 [!DNL Adobe Workfront Fusion]</a>의 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 변환을 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 주석 수]</td> 
   <td>한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오. </td> 
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
