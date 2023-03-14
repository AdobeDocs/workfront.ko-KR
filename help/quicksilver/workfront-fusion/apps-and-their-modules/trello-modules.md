---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Trello 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오는 Trelo를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '5039'
ht-degree: 0%

---

# [!UICONTROL 트렐로] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!UICONTROL 트렐로]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL Trello] 모듈이면 반드시 [!UICONTROL 트렐로] 계정이 필요합니다.

## Connect [!UICONTROL 트렐로] to [!DNL Workfront Fusion]

연결 방법에 대한 지침은 [!UICONTROL 트렐로] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. [연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL 트렐로] 모듈 및 해당 필드

구성 시 [!UICONTROL 트렐로] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!UICONTROL 트렐로] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [보드](#boards)
* [목록](#lists)
* [카드](#cards)
* [멤버](#members)
* [확인 목록](#checklists)
* [레이블](#labels)
* [댓글](#comments)

### 보드

+++ **[!UICONTROL 보기 보드]**

이 트리거 모듈은 새 보드가 추가될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 보드 수 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 보드 만들기]**

이 작업 모듈은 선택한 설정으로 새 보드를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>새 보드의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>필요한 경우 보드 설명을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 조직 ID]</p> </td> 
   <td> <p>조직의 ID를 입력하거나 매핑합니다. 조직 ID는 감시 활동 모듈과 같은 다른 모듈을 사용하여 검색할 수 있습니다.</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 권한 수준]</p> </td> 
   <td> <p>보드에는 각 권한 수준에 대해 서로 다른 투표 및 주석 처리 규칙이 있습니다. 예: 보드가 [!UICONTROL Private]이고 투표 및 주석 처리 규칙을 [!UICONTROL All]로 설정하면 오류가 발생합니다. </p> <p>투표 및 논평은 각 권한 수준에 대해 다음 그룹으로 제한됩니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: —&gt;구성원, 구성원 및 관찰자</li> 
     <li><strong>[!UICONTROL For Organization]</strong>: —&gt;구성원, 구성원 및 관찰자, 조직 구성원</li> 
     <li><strong>[!UICONTROL Public]</strong>: —&gt;구성원, 구성원 및 관찰자, 조직 구성원, 모두</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>이 보드에 투표할 수 있는 사람을 지정하려면 옵션을 선택하십시오. 권한 수준에 대한 투표 제한 사항에 대해서는 [!UICONTROL 권한 수준] 필드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>이 보드의 카드에 댓글을 달 수 있는 사용자를 지정하려면 옵션을 선택합니다. 권한 수준에 대한 제한 사항에 대해서는 [!UICONTROL 권한 수준] 필드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitations]</p> </td> 
   <td> <p>이 보드에 다른 사람을 초대할 수 있는 사람을 선택하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Self-Join]</p> </td> 
   <td> <p>팀 구성원이 이사회에 직접 참여할 수 있는지 아니면 초대해야 하는지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 기본 레이블]</p> </td> 
   <td> <p>새 보드에 기본 레이블 세트를 사용할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 기본 목록]</p> </td> 
   <td> <p>기본 목록 세트를 보드([!UICONTROL To Do], [!UICONTROL Doing], [!UICONTROL Done])에 추가할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보드 소스 ID]</p> </td> 
   <td> <p>새 보드에 복사할 보드의 ID를 선택하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card Codes]</p> </td> 
   <td> <p>선택 <strong>[!UICONTROL Yes]</strong> 보드에 대해 카드 덮개를 활성화하려면</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Background]</p> </td> 
   <td> <p>배경색 또는 사용자 정의 배경을 선택합니다.</p> <p>참고: 사용자 지정 배경에는 [!UICONTROL Trello Gold 및 Business Class] 구독자만 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card Aging]</p> </td> 
   <td> <p>카드 에이징 두 가지 모드 중에서 선택합니다. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: 카드는 나이가 들수록 점점 더 투명해진다. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: 카드는 그들이 늙어가면서 오래된 해적판처럼 찢어지고, 노랗게 갈라질 것이다.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 보드 편집]**

이 작업 모듈은 기존 보드의 설정을 편집합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보드 ID]</p> </td> 
   <td> <p>모듈을 만들 보드의 고유한 [!UICONTROL Trello] ID를 입력하거나 매핑합니다. 시계 보드 모듈과 같은 다른 모듈을 사용하여 보드 ID를 검색할 수 있습니다</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 이름]</td> 
   <td> <p> 보드의 새 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 설명]</td> 
   <td> <p> 필요한 경우 새 보드 설명을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 조직 ID]</p> </td> 
   <td> <p>모듈을 편집할 보드의 고유 [!UICONTROL Trello] ID를 입력하거나 매핑합니다. 와 같은 다른 모듈을 사용하여 보드 ID를 검색할 수 있습니다. [!DNL Watch Activities] 모듈.</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>실행 중인 사용자가 보드에 가입되어 있는지 여부를 지정하려면 옵션을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 권한 수준]</p> </td> 
   <td> <p>보드에는 각 권한 수준에 대해 서로 다른 투표 및 주석 처리 규칙이 있습니다. 예: 보드가 [!UICONTROL Private]이고 투표 및 주석 처리 규칙을 [!UICONTROL All]로 설정하면 오류가 발생합니다. </p> <p>투표 및 논평은 각 권한 수준에 대해 다음 그룹으로 제한됩니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: —&gt;구성원, 구성원 및 관찰자</li> 
     <li><strong>[!UICONTROL For Organization]</strong>: —&gt;구성원, 구성원 및 관찰자, 조직 구성원</li> 
     <li><strong>[!UICONTROL Public]</strong>: —&gt;구성원, 구성원 및 관찰자, 조직 구성원, 모두</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>이 보드에 투표할 수 있는 사람을 지정하려면 옵션을 선택하십시오. 권한 수준에 대한 투표 제한 사항에 대해서는 [!UICONTROL 권한 수준] 필드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>이 보드의 카드에 댓글을 달 수 있는 사용자를 지정하려면 옵션을 선택합니다. 권한 수준에 대한 제한 사항에 대해서는 [!UICONTROL 권한 수준] 필드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitations] </td> 
   <td> <p>이 보드에 사용자를 초대할 수 있는 사람을 선택하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-Join]</td> 
   <td> <p> 팀 구성원이 이사회에 직접 참여할 수 있는지 아니면 초대해야 하는지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card Codes]</td> 
   <td> <p> 이 보드에 카드 덮개를 표시할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background] </td> 
   <td> <p>배경색 또는 사용자 정의 배경을 선택합니다.</p> <p>참고: 사용자 지정 배경에는 [!UICONTROL Trello Gold 및 Business Class] 구독자만 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background ID]</td> 
   <td> <p> [!UICONTROL Background] 필드에서 사용자 지정 배경을 사용하도록 선택한 경우, 사용할 배경의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card Aging]</p> </td> 
   <td> <p>카드 에이징 두 가지 모드 중에서 선택합니다. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: 카드는 나이가 들수록 점점 더 투명해진다. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>: 카드는 그들이 늙어가면서 오래된 해적판처럼 찢어지고, 노랗게 갈라질 것이다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 달력 피드 사용]</td> 
   <td> <p> 달력 피드의 활성화 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;color&gt; 레이블 이름]</td> 
   <td> <p> 원하는 색상 레이블에 이름을 지정합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>보드를 보관(닫기)할지 여부를 나타내는 옵션을 선택합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 보드 가져오기]**

이 작업 모듈은 보드의 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보드 ID]</p> </td> 
   <td> <p>정보를 검색할 보드의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

이 검색 모듈은 지정한 보드에 대한 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>정보를 얻을 보드의 이름(또는 이름 일부)을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 보드 수]</td> 
   <td> <p> 최대 보드 수를 입력합니다 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다. 이 값은 1000보다 작거나 같아야 합니다.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partial] </p> </td> 
   <td> <p>기본적으로 이 모듈은 구성원 컨텐츠에서 쿼리의 각 단어의 정확한 일치 여부를 검색합니다. [!UICONTROL Partial]이 활성화되어 있으면 모듈은 쿼리의 임의의 단어로 시작하는 콘텐츠를 찾습니다.</p> <p> 예를 들어 "development"라는 단어를 사용하여 "My Development Status Report"라는 보드를 찾는 경우 기본적으로 전체 단어를 검색해야 합니다. [!UICONTROL Partial]이 활성화되어 있으면 "dev"를 검색할 수 있지만 "development"는 검색할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Boards] </td> 
   <td> <p>"mine"을 입력하거나, 쉼표로 구분된 보드 ID 목록을 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 보드 보관 또는 보관 해제]**

이 작업 모듈은 지정한 보드를 닫거나 다시 엽니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보드 ID]</td> 
   <td> <p> 닫거나 다시 열 보드의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 아카이브 또는 아카이브 해제]</td> 
   <td> <p> 보드를 닫을지(아카이브) 또는 보드를 다시 열지를(보관 해제) 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 보드에 구성원 할당]**

이 작업 모듈은 지정된 보드에 구성원을 지정합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보드 ID]</td> 
   <td> <p> 구성원을 추가할 보드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email address]</td> 
   <td> <p> 보드에 추가할 구성원의 전자 메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 멤버 유형]</p> </td> 
   <td> <p>보드에 추가할 멤버 유형을 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>: 보드 관리자는 보드에서 모든 보드 작업을 수행할 수 있습니다.</li> 
     <li><strong>[!UICONTROL Normal]</strong>: 일반 멤버는 단지 이사회의 구성원일 뿐입니다.</li> 
     <li><strong>[!UICONTROL Observer]</strong>: 관찰자는 보드에 대한 읽기 전용 액세스 권한을 가진 멤버입니다. <br>관찰자는 [!UICONTROL Trello Business Class]를 사용하는 팀에서만 사용할 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 전체 이름]</td> 
   <td> <p> 보드에 추가할 사용자의 전체 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 보드에서 구성원 할당 취소]**

이 작업 모듈은 보드에서 멤버를 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보드 ID]</td> 
   <td> <p> 사용자를 제거할 보드의 ID를 입력(매핑 또는 선택)합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member] </td> 
   <td> <p>보드에서 제거할 멤버를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 목록

+++ **[!UICONTROL 목록으로 이동한 감시 카드]**

이 트리거 모듈은 카드를 특정 목록으로 이동하면 활성화됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>카드를 확인할 목록이 포함된 보드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>카드를 표시할 목록을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 카드 수 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 목록 만들기]**

이 작업 모듈은 지정된 보드에 목록을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보드 ID]</td> 
   <td> <p> 목록을 만들 보드의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>새 목록의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>목록을 맨 위에 추가할지 또는 카드 하단에 추가할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 복사]</td> 
   <td> <p> 복사할 목록의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>수동으로 입력</strong> </p> <p>에서 <strong>[!UICONTROL 목록 ID]</strong> 필드에서 복사할 목록의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>선택</strong> </p> <p>복사할 목록이 들어 있는 보드를 선택한 다음 목록을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 목록 편집]**

이 작업 모듈은 기존 목록을 편집합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 ID]</td> 
   <td> <p> 업데이트할 목록의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>목록의 새 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보드 ID]</td> 
   <td> <p> 목록을 이동할 보드를 매핑하거나 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>목록을 맨 위에 추가할지 또는 카드 하단에 추가할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 가입]</td> 
   <td> <p>목록에 활성 멤버를 가입하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 목록 가져오기]**

이 작업 모듈은 특정 목록에 대한 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 목록 ID]</p> </td> 
   <td> <p>정보를 검색할 목록의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 카드

+++ **[!UICONTROL 카드 보기]**

새 카드가 추가되면 이 트리거 모듈이 활성화됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Viewed 개체]</td> 
   <td> <p>카드를 볼 위치를 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 모든 카드]</strong> </li> 
     <li> <p><strong>특정 보드의 카드</strong> </p> <p>카드를 시청할 보드를 선택합니다</p> </li> 
     <li> <p><strong>[!UICONTROL 특정 목록의 카드]</strong> </p> <p>카드를 확인할 목록이 포함된 보드를 선택한 다음 목록을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 카드 수 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 카드 만들기]**

이 작업 모듈은 선택한 목록에 카드를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 목록 ID 입력]</td> 
   <td> <p> 카드를 추가할 목록의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL 목록 ID]</strong> 필드를 입력하거나 카드를 추가할 목록의 ID를 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>복사할 목록이 들어 있는 보드를 선택한 다음 목록을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블] </td> 
   <td> <p>카드에 추가할 각 레이블에 대해 레이블의 ID를 입력합니다. 예를 들어 [!UICONTROL Retrieve Labels] 모듈을 사용하여 ID를 검색할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members]</td> 
   <td>카드에 추가할 각 구성원에 대해 구성원의 ID를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>새 카드의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Description]</p> </td> 
   <td> <p>카드에 대한 설명을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>카드를 맨 위에 추가할지 또는 [!UICONTROL 추가] 카드를 목록의 맨 아래에 추가할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기한]</td> 
   <td> <p> 카드의 만기 일자를 입력합니다. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 완료]</td> 
   <td> <p> 기한 내에 카드가 완료되었음을 표시하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 URL]</td> 
   <td> <p>카드에 첨부 파일로 추가할 파일의 URL을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 소스 파일]</p> </td> 
   <td> <p>카드에 첨부 파일로 추가할 파일에 대한 정보를 입력하거나 매핑합니다.</p> 
    <ul> 
     <li>[!UICONTROL 파일 이름]: 파일 확장명을 포함하여 파일 이름을 입력하거나 매핑합니다.</li> 
     <li> 
     <p>이전 모듈에서 파일을 선택하거나 파일의 이름과 데이터를 매핑합니다</p> 
     <p>참고: 첨부 파일당 10MB의 파일 업로드 제한이 있습니다. 그러나 [!UICONTROL Business Class] 및 [!UICONTROL Trello Gold] 멤버에는 첨부 파일당 250MB의 파일 업로드 제한이 있습니다.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 복사]</td> 
   <td> <p> 복사할 카드 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드에서 복사할 카드의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>복사할 카드가 들어 있는 보드를 선택한 다음 카드가 들어 있는 목록을 선택한 다음 카드를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 카드 편집]**

이 작업 모듈은 기존 카드를 편집합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 입력]</td> 
   <td> <p> 편집할 카드의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드에서는 편집할 카드의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>편집할 카드가 들어 있는 보드를 선택한 다음 카드가 들어 있는 목록을 선택한 다음 카드를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 새 이름]</td> 
   <td> <p>카드의 새 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 새 설명]</p> </td> 
   <td> <p>카드에 대한 새 설명을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 카드 이동]</p> </td> 
   <td> <p>카드를 이동할 보드 및 목록을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레이블] </td> 
   <td> <p>카드에 추가할 레이블의 ID를 추가합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>카드를 맨 위에 추가할지 또는 [!UICONTROL 추가] 카드를 목록의 맨 아래에 추가할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기한]</td> 
   <td> <p> 카드의 만기 일자를 입력합니다. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 완료]</td> 
   <td> <p> 이 옵션을 활성화하면 만기일에 카드가 완료로 표시됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members] </td> 
   <td> <p>카드에 추가할 구성원의 ID를 추가하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 첨부 파일 덮개 ID]</p> </td> 
   <td> <p>카드에서 사용할 이미지 첨부 파일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>멤버를 카드에 가입할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>카드를 보관(닫기)할지 여부를 나타내는 옵션을 선택합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 카드 가져오기]**

이 작업 모듈은 선택한 카드의 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 보드 ID]</td> 
   <td> <p>세부 정보를 검색할 카드가 포함된 보드의 ID를 입력합니다. 이를 통해 보드의 사용자 지정 필드 이름을 볼 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 입력]</td> 
   <td> <p> 세부 사항을 검색할 카드의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드에서는 세부 사항을 검색할 카드의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>세부 사항을 검색할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 카드 검색]**

이 작업 모듈은 검색 쿼리와 일치하는 카드를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>검색할 보드를 선택합니다. 보드를 선택하지 않으면 모든 보드가 검색됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Query]</p> </td> 
   <td> <p>검색 쿼리를 입력합니다. 다음 검색 연산자를 사용하여 검색을 개선할 수 있습니다.</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>모든 연산자에 "-"를 추가하여 다음과 같은 음수 검색을 수행할 수 있습니다. <code>[!UICONTROL -has:members]</code> 구성원이 할당되지 않은 카드를 검색합니다.</p> </li> 
     <li><code><strong>@name</strong></code> <p>멤버에 할당된 카드를 반환합니다. 를 사용할 수도 있습니다 <code>member:</code>. 사용 <code>@me</code> 귀하의 카드만 포함시키려면</p> </li> 
     <li><code><strong>#label</strong></code> <p>레이블이 지정된 카드를 반환합니다. 를 사용할 수도 있습니다 <code>label:</code>. 예, <code>label:"FIX IT"</code> 은 "FIX IT"라는 레이블이 있는 카드를 반환합니다.</p> </li> 
     <li><code><strong>board:id</strong></code> <p>특정 보드 내에서 카드를 반환합니다. 예, <code>board:Trello</code> 은 보드 이름에 [!UICONTROL Trello]가 있는 보드에 카드를 반환합니다.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>이름이 "name"인 목록 내의 카드를 반환합니다.</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>첨부 파일이 있는 카드를 반환합니다. 다음 <code>has</code>: 연산자는 다음과 같은 다른 속성과 함께 사용할 수도 있습니다. <code>has:description</code>, <code>has:cover</code>, <code>has:members</code>, 또는 <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>24시간 이내에 반납해야 하는 카드를 반환합니다. 다음 <code>due:</code> 연산자는 다음과 같은 다른 타임프레임에서도 사용할 수 있습니다 <code>due:week</code>, <code>due:month</code>, 또는 <code>due:overdue</code>. 특정 날짜 범위를 검색할 수도 있습니다. 예를 들어, <code>due:14</code> 검색하는 데 앞으로 14일 내에 지불해야 하는 카드가 포함됩니다.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>지난 24시간 내에 만든 카드를 반환합니다. 다음<code> created:</code> 연산자는 와 같은 다른 타임프레임에서도 사용할 수 있습니다. <code>created:week</code> 또는 <code>created:month</code>. 특정 날짜 범위를 검색할 수도 있습니다. 예를 들어, <code>created:14</code> 검색하는 데 지난 14일 동안 생성된 카드가 포함됩니다.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>지난 24시간 동안 편집한 카드를 반환합니다. 다음 <code>edited:</code> 연산자는 다음과 같은 다른 타임프레임에서도 사용할 수 있습니다 <code>edited:week</code> 또는 <code>edited:month</code>. 특정 날짜 범위를 검색할 수도 있습니다. 예를 들어, <code>edited:21</code> 검색에는 지난 21일 동안 편집한 카드가 포함됩니다.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>카드 설명, 확인 목록, 주석 또는 이름의 텍스트와 일치하는 카드를 반환합니다. 예를 들어, comment:"FIX IT"는 주석에 "FIX IT"가 있는 카드를 반환합니다.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>열거나 보관한 카드를 반환합니다. 둘 다 지정하지 않은 경우 [!UICONTROL Trello]는 두 유형을 모두 반환합니다.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>별표에 카드만 포함됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 카드 수]</td> 
   <td> <p> 최대 카드 수 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다. 이 값은 1000보다 작거나 같아야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>기본적으로 이 모듈은 구성원 컨텐츠에서 쿼리의 각 단어의 정확한 일치 여부를 검색합니다. [!UICONTROL Partial]이 활성화되어 있으면 모듈은 쿼리의 임의의 단어로 시작하는 콘텐츠를 찾습니다.</p> <p> 예를 들어 "development"라는 단어를 사용하여 "My Development Status Report"라는 보드를 찾는 경우 기본적으로 전체 단어를 검색해야 합니다. [!UICONTROL Partial]이 활성화되어 있으면 "dev"를 검색할 수 있지만 "development"는 검색할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cards] </td> 
   <td> <p>특별히 검색할 카드를 추가합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 카드 보관 또는 보관 해제]**

이 작업 모듈은 카드를 보관하거나 보드에 다시 보냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card ID]</td> 
   <td> <p> 보관하거나 보드에 다시 전송할 카드의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 아카이브 또는 아카이브 해제]</td> 
   <td> <p> 카드를 닫을지(아카이브) 아니면 보드(보관 해제)로 다시 보낼지 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 첨부 파일 추가]**

이 작업 모듈은 선택한 카드에 첨부 파일을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 입력]</td> 
   <td> <p> 세부 사항을 검색할 카드의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>수동으로 입력</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드에서는 세부 사항을 검색할 카드의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>세부 사항을 검색할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 첨부 파일 유형]</p> </td> 
   <td> <p>파일을 직접 업로드할지 또는 파일에 URL을 제공할지를 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File]</strong> </p> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>파일의 URL을 입력하고 첨부 파일의 이름을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 멤버

+++ **[!UICONTROL 보드에 구성원 할당]**

참조:[!UICONTROL 보드에 구성원 할당]아래에 [보드](#boards).

+++

+++ **[!UICONTROL 보드에서 구성원 할당 취소]**

참조:[!UICONTROL 보드에서 구성원 할당 취소]아래에 [보드](#boards).

+++

+++ **[!UICONTROL 카드에 구성원 추가]**

이 작업 모듈은 지정된 멤버를 지정된 카드에 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 카드 ID 및 멤버 ID 입력]</p> </td> 
   <td> <p>카드 ID와 구성원 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>을 입력하거나 매핑합니다 <strong>[!UICONTROL Card ID]</strong> 그리고 <strong>[!UICONTROL 멤버 ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>구성원을 추가할 카드가 포함된 보드를 선택한 다음 카드, 카드 자체 및 카드에 추가할 멤버가 포함된 목록을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 멤버 검색]**

이 작업 모듈은 [!UICONTROL 트렐로] 멤버.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>찾을 사용자의 전체 이름 또는 사용자 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>기본적으로 이 모듈은 구성원 컨텐츠에서 쿼리의 각 단어의 정확한 일치 여부를 검색합니다. [!UICONTROL Partial]이 활성화되어 있으면 모듈은 쿼리의 임의의 단어로 시작하는 콘텐츠를 찾습니다.</p> <p> 예를 들어 "development"라는 단어를 사용하여 "My Development Status Report"라는 보드를 찾는 경우 기본적으로 전체 단어를 검색해야 합니다. [!UICONTROL Partial]이 활성화되어 있으면 "dev"를 검색할 수 있지만 "development"는 검색할 수 없습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 멤버 수]</td> 
   <td> <p> 최대 멤버 수 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 확인 목록

+++ **[!UICONTROL 검사 목록 만들기]**

이 작업 모듈은 선택한 카드에 체크리스트를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 입력]</td> 
   <td> <p> 체크리스트를 추가할 카드의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드를 입력하거나 체크리스트를 추가할 카드의 ID를 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>체크리스트를 추가할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>검사 목록 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>체크리스트를 맨 위에 추가할지 또는 [!UICONTROL에서] 체크리스트를 카드 하단에 추가할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 검사 목록 ID 입력]</p> </td> 
   <td> <p>새 확인 목록에 복사할 소스 확인 목록의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 검사 목록 항목 만들기]**

이 작업 모듈은 특정 체크리스트에 항목을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검사 목록 ID 입력]</td> 
   <td> <p> 항목을 추가할 체크리스트 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL 검사 목록 ID]</strong> 필드를 입력하거나 체크리스트를 추가할 카드의 ID를 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>체크리스트를 추가할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택한 다음 체크리스트를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 항목 이름]</p> </td> 
   <td> <p>새 항목의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>항목을 맨 위에 추가할지 또는 [!UICONTROL 추가]를 검사 목록 맨 아래에 추가할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 선택됨]</p> </td> 
   <td> <p>항목을 이미 선택된 상태로 추가하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 검사 목록 항목 편집]**

이 작업 모듈은 기존 체크리스트를 편집합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 및 체크리스트 항목 ID 입력]</td> 
   <td> <p> 항목을 편집할 카드 및 체크리스트의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL 검사 목록 ID]</strong> 필드를 입력하거나 체크리스트를 추가할 카드의 ID를 매핑합니다.</p> <p>에서 <strong>[!UICONTROL 검사 목록 항목 ID]</strong> 필드를 입력하거나 검사 목록 ID를 매핑합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>체크리스트를 추가할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택한 다음 체크리스트를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 검사 목록 ID]</td> 
   <td>검사 목록 항목을 이동할 검사 목록을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 항목 이름]</p> </td> 
   <td> <p>새 항목의 이름을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>항목을 맨 위에 추가할지 또는 검사 목록 맨 아래에 추가할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>검사 목록 항목이 완료되었는지 아니면 완료되지 않았는지 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 레이블

+++ **[!UICONTROL 카드에 레이블 추가]**

이 작업 모듈은 선택한 카드에 레이블을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 입력]</td> 
   <td> <p> 체크리스트를 추가할 카드의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드를 입력하거나 체크리스트를 추가할 카드의 ID를 매핑합니다. 에서<strong>[!UICONTROL Label ID]</strong> 필드에서는 추가할 레이블의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>체크리스트를 추가할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택합니다. </p> <p>카드에 추가할 레이블을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 댓글

+++ **[!UICONTROL 댓글 보기]**

지정한 위치에 새 주석이 있으면 주석 세부 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Viewed 개체]</td> 
   <td> <p>댓글을 확인할 위치를 선택합니다.</p> 
    <ul> 
     <li><strong>어디에서나 [!UICONTROL 모든 카드]</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>댓글을 확인할 보드를 선택합니다</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>메모를 확인할 목록이 포함된 보드를 선택한 다음 목록을 선택합니다.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>댓글을 확인할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택합니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td> <p>최대 댓글 수 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 카드에서 주석 만들기]**

이 작업 모듈은 선택한 카드에 주석을 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 입력]</td> 
   <td> <p> 댓글을 추가할 카드의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드에서는 설명을 추가할 카드의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>댓글을 추가할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment] </td> 
   <td> <p>선택한 카드에 추가할 설명을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 카드에 주석 나열]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!UICONTROL Trello] 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 카드 ID 입력]</td> 
   <td> <p> 댓글을 추가할 카드의 ID를 입력할 방법을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 수동으로 Enter]</strong> </p> <p>에서 <strong>[!UICONTROL Card ID]</strong> 필드에서는 설명을 추가할 카드의 ID를 입력하거나 매핑합니다.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>댓글을 추가할 카드가 포함된 보드를 선택한 다음 카드가 포함된 목록을 선택한 다음 카드를 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환된 최대 주석 수]</td> 
   <td> <p> 최대 댓글 수를 입력합니다 [!DNL Workfront Fusion] 은 한 실행 주기 동안 반환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since] </td> 
   <td> <p>설명이 생성된 기간의 시작 날짜를 설정합니다. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before] </td> 
   <td> <p>설명이 생성된 기간의 종료 날짜를 설정합니다. 지원되는 날짜 및 시간 형식 목록은 다음을 참조하십시오 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">형식 강제 적용 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL 트렐로] 개체 ID

* [에서 카드의 ID 또는 바로 가기 링크를 찾는 방법 [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [에서 다른 개체의 ID를 찾는 방법 [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### 에서 카드의 ID 또는 바로 가기 링크를 찾는 방법 [!DNL Trello]

카드를 편집하거나 새 주석을 만들려면 카드의 ID 또는 바로 가기 링크를 알고 있어야 합니다. 이 정보는 [!UICONTROL 새 카드] 트리거합니다. 카드를 열고 을 클릭하면 카드용 바로 가기를 얻을 수도 있습니다 [!UICONTROL 공유] 버튼을 클릭합니다. 바로 가기는 [!UICONTROL 이 카드에 연결] 다음 URL 끝에 있는 상자 `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### 에서 다른 개체의 ID를 찾는 방법 [!DNL Trello]

보드, 목록 및 주석 ID는 트리거를 사용해야만 가져올 수 있습니다. 다음 [!DNL trello.com] 웹 사이트에 이러한 ID가 표시되지 않습니다.
