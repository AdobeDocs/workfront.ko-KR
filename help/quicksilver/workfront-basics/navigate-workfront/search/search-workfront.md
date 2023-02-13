---
navigation-topic: search
title: 검색 [!DNL Adobe Workfront]
description: 에서 항목을 쉽게 찾을 수 있습니다 [!DNL Adobe Workfront] 정확한 위치를 기억할 수 없을 때 검색합니다.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 1%

---

# 검색 [!DNL Adobe Workfront]

에서 항목을 쉽게 찾을 수 있습니다 [!DNL Adobe Workfront] 정확한 위치를 기억할 수 없을 때 검색합니다.

다음을 볼 수 있습니다 [!UICONTROL 검색] 내 페이지의 오른쪽 위 모서리에 있는 상자 [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

검색에서 개체를 찾으려면 먼저 개체를 볼 수 있는 권한이 있어야 합니다. 이러한 이유로 검색 결과는 사용자마다 다릅니다.

## 액세스 요구 사항

+++ 이 섹션을 확장하여 이 문서의 단계를 수행하는 데 필요한 액세스 권한을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>개체 유형에 대한 [!UICONTROL View] 액세스 </p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>검색에서 개체를 찾으려면 먼저 개체를 볼 수 있는 권한이 있어야 합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

+++

## 검색 이해

* [[!UICONTROL 검색할 수 있는 객체]](#objects-available-for-search)
* [[!UICONTROL 검색할 수 있는 필드]](#fields-available-for-search)

### 검색할 수 있는 객체

Workfront에서 다음 개체를 검색할 수 있습니다.

* 프로젝트
* 작업
* 문제
* 보고서
* 사용자
* 템플릿
* 문서
* 포트폴리오
* 프로그램
* 대시보드
* 회사
* 메모

### 검색할 수 있는 필드

검색할 수 있는 필드는 검색 유형을 기반으로 합니다. 기본 또는 [!UICONTROL 고급 검색].

* **기본 검색**: 기본 검색에서 객체를 검색할 때 [!DNL Workfront] 다음 필드에 키워드를 포함할 수 있는 텍스트를 찾습니다.

   * 개체 이름
   * 설명
   * 사용자 지정 데이터 필드
   * 업데이트
   * 문서 이름(특정 문서에서 검색하거나 기본 검색에서)

   의 기본 검색에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [기본 검색](#basic-search) 참조하십시오.

* **[!UICONTROL 고급 검색]**: 에서 [!UICONTROL 고급 검색]기본 검색에서 사용할 수 없는 필드를 검색하도록 필터를 설정할 수 있습니다. 따라서, [!UICONTROL 고급 검색] 개체의 필드를 검색할 수 있습니다.

   에 대한 자세한 정보 [!UICONTROL 고급 검색]를 참조하십시오. [고급 검색](#advanced-search) 참조하십시오.

>[!NOTE]
>
>다음을 수행하려면 다음을 수행합니다 [!UICONTROL 고급 검색]를 선택해야 합니다. [!UICONTROL 고급 검색] 검색을 시작할 때 선택합니다. 기본 검색을 [!UICONTROL 고급 검색].

## 의 제한 사항 이해 [!DNL Workfront] 검색

를 사용할 때는 다음 제한 사항을 고려하십시오 [!UICONTROL 검색] in [!DNL Workfront]:

* 검색은 대소문자를 구분하지 않습니다
* [!DNL Workfront] 오타가 올바르지 않거나 이해되지 않음
* 검색 중 [!DNL Workfront] 와일드카드를 지원하지 않음
* 검색 중 [!DNL Workfront] 부분 단어 검색을 지원하지만 하위 문자열 검색은 지원하지 않습니다.\
   예를 들어 검색 키워드 &quot;스탠드&quot;는 &quot;standard&quot;라는 단어를 포함하는 결과를 반환하지만 &quot;understand&quot;라는 단어를 포함하는 결과는 반환하지 않습니다.

## 여러 단어 검색

검색에서 여러 단어를 포함하고 검색 상자의 모든 단어와 일치하는 객체만 찾으려면 임의의 순서로 단어를 입력할 수 있습니다.

예를 들어 &quot;마케팅 데모&quot;(따옴표 없이)를 검색하면 다음 이름이 있는 개체를 찾습니다.

* 마케팅 데모
* 데모 마케팅
* 1월 시장 분석 데모

또한 이름에 &quot;Marketing&quot;이 있고 설명에서 &quot;Demo&quot;가 있을 수 있는 개체를 찾습니다.

그러나 에서는 다음 작업을 수행할 수 있습니다 [!UICONTROL 검색] 표시되는 검색 결과를 조정하려면 상자를 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>큰따옴표 포함</td> 
   <td> <p>큰따옴표 안에 올바른 순서로 단어를 입력하면 정확히 일치하는 객체만 찾을 수 있습니다.<br>예를 들어 "마케팅 데모"(따옴표로 묶음)를 검색하면 다음 이름이 있는 객체를 찾습니다.</p> 
    <ul> 
     <li> 마케팅 데모</li> 
     <li> 1월 마케팅 데모</li> 
     <li>마케팅 데모 계획</li> 
    </ul> <p>그러나 이 검색에서는 "데모 마케팅"이라는 이름의 개체를 찾지 못합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>OR 포함</td> 
   <td> <p>"OR"(큰따옴표 없이)로 단어를 연결하면 [!UICONTROL 검색] 상자에 있는 단어 중 적어도 하나와 일치하는 개체만 찾을 수 있습니다. 이 단어들은 어떤 순서로도 입력할 수 있다.<br>예를 들어 "Marketing OR Demo"(따옴표 없이)를 검색하면 다음 이름이 있는 개체를 찾습니다.</p> 
    <ul> 
     <li> 시장 분석 데모</li> 
     <li>1월 시장 분석 데모</li> 
     <li>데모</li> 
     <li>시장 분석</li> 
    </ul> <p>참고: "OR"는 모든 대문자에 포함되어야 합니다. 그렇지 않으면 찾고 있는 구문에서 다른 단어로 해석됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>AND 포함</td> 
   <td> <p>"AND"(큰따옴표 없이)로 단어를 연결하면 [!UICONTROL 검색] 상자의 모든 단어와 일치하는 개체만 찾을 수 있습니다. 이 단어들은 어떤 순서로도 입력할 수 있다.<br>예를 들어 "Marketing AND Demo"(따옴표 없이)를 검색하면 다음 이름이 있는 개체를 찾습니다.</p> 
    <ul> 
     <li>마케팅 데모</li> 
     <li>데모 마케팅</li> 
     <li>1월 시장 분석 데모</li> 
    </ul> <p>참고: "AND"는 모두 대문자로 입력해야 합니다. 그렇지 않으면 찾고 있는 구문에서 다른 단어로 해석됩니다. 마찬가지로 "&amp;"(큰따옴표 없이)는 앰퍼샌드 문자를 포함하는 개체만 검색합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 검색 사용 위치 [!DNL Workfront]

[!DNL Workfront] 에서는 두 가지 유형의 검색을 제공합니다. 기본 및 고급 이름 또는 설명과 같은 공통 객체 필드에서 키워드를 찾으려면 기본 검색을 사용합니다. 사용 [!UICONTROL 고급 검색] 필터를 사용하여 다른 개체 필드를 검색하려는 경우.

* [기본 검색](#basic-search)
* [고급 검색](#advanced-search)

### 기본 검색

기본 검색을 사용하면 시스템의 모든 객체 또는 한 번에 하나의 객체(예: 프로젝트)에서 키워드를 검색할 수 있습니다. [!DNL Workfront] 그런 다음 몇 가지 특정 필드에서 해당 키워드를 검색합니다. 그런 다음 [!DNL Workfront].

기본 검색에서 검색한 특정 필드 목록을 보려면 [검색할 수 있는 필드](#fields-available-for-search) 참조하십시오.

>[!NOTE]
>
>다음을 수행하려면 다음을 수행합니다 [!UICONTROL 고급 검색]를 선택해야 합니다. [!UICONTROL 고급 검색] 검색을 시작할 때 선택합니다. 기본 검색을 [!UICONTROL 고급 검색].

* [기본 검색 수행](#perform-a-basic-search)
* [기본 검색 세분화](#refine-a-basic-search)

#### 기본 검색 수행

다음 방법 중 하나로 기본 검색을 수행할 수 있습니다.

* 시스템의 모든 개체(일반 검색)에 대해
* 한 번에 한 개체에서만(개체별 검색).

기본 검색을 수행하려면 다음을 수행하십시오.

1. 확대경을 클릭합니다 ![](assets/search-icon.png) 페이지의 오른쪽 위 모서리에서 을(를) 클릭합니다. 입력할 수도 있습니다 **[!UICONTROL ALT + /]** 또는 **[!UICONTROL Option + /]** 열다 [!UICONTROL 검색] 메뉴 아래의 제품에서 사용할 수 있습니다.

1. (선택 사항) 특정 개체를 검색하려면 **[!UICONTROL 모두]** 드롭다운 메뉴를 클릭하고 검색할 객체를 선택합니다.

   ![](assets/search-objecttype.png)

1. 에서 **[!UICONTROL 검색]** 상자에서 검색할 정보를 입력하기 시작합니다.\
   검색할 필드에 대한 정보 [!DNL Workfront]를 참조하십시오. [검색 이해](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   검색 창에 입력을 시작하면 [!DNL Workfront] 은 보기 기록을 기반으로 권장 사항을 만들고 파란색으로 검색 중인 키워드를 강조 표시합니다.

1. 찾고 있는 항목이 [!UICONTROL 서체] 메뉴에서 클릭합니다.

   또는

   누르기 **[!UICONTROL Enter 키]** 포괄적인 검색을 수행합니다. 이 검색은 가장 최근에 본 항목 대신 전체 데이터베이스를 쿼리합니다.

   다음 [!UICONTROL 검색 결과] 페이지 슬라이드는 왼쪽에서 열고 이전 페이지의 대부분을 다룹니다.

   일반 검색을 수행했다면, [!DNL Workfront] 에 설명된 대로 검색된 필드의 검색어와 일치하는 객체에 대한 결과를 반환합니다. [검색 이해](#understand-search). 검색과 일치하는 객체가 목록에 표시됩니다.

   >[!NOTE]
   >
   >검색된 항목 목록에 단어의 변형이 표시되는 경우가 있습니다.\
   >예를 들어 &quot;마케팅&quot;을 검색하면 이름에 &quot;marketing&quot; 또는 &quot;market&quot;이 포함된 개체가 표시됩니다.

1. (선택 사항) 검색에서 너무 많은 결과가 생성된 경우 다음에 설명된 대로 검색을 세분화합니다. [기본 검색 세분화](#refine-a-basic-search).
1. (선택 사항) 검색 전에 있었던 페이지로 돌아가려면 를 클릭합니다. **[!UICONTROL 닫기]** 오른쪽 상단 모서리에서

>[!NOTE]
>
>다음 [!UICONTROL 검색 결과] 페이지가 포커스에 있을 때만 열린 상태로 유지됩니다. 페이지에서 멀리 클릭하거나 다른 페이지를 열면 [!UICONTROL 검색 결과] 페이지.

#### 기본 검색 세분화

에 설명된 대로 기본 검색을 수행한 후 [[!UICONTROL 기본 검색 수행]](#perform-a-basic-search)- 검색을 세분화할 수 있습니다.

검색 결과 왼쪽에 있는 도구 모음을 사용하여 찾고 있는 정보를 좁힐 수 있습니다.

검색을 세분화하려면 다음을 수행하십시오.

1. (조건부) 일반 검색을 수행한 경우 검색 결과 왼쪽 위의 객체 목록에서 검색할 객체를 선택합니다.
1. 검색 결과의 왼쪽에 있는 도구 모음에서 검색에 표시되는 객체에 사용할 수 있는 필드를 찾습니다.\
   각 필드의 값이 개수로 정렬되어 각 필드에 대해 최대 10개의 값이 표시됩니다.
1. 결과 목록을 줄이는 데 사용할 수 있는 필드 안을 클릭합니다.\
   선택한 항목은 파란색으로 강조 표시되고 선택하지 않은 필드 값은 표시되지 않습니다.\
   각 새 값을 선택하면 해당 결과가 동적으로 업데이트됩니다.\
   ![](assets/qs-refine-search-350x175.png)

1. (선택 사항) 선택한 값을 클릭하여 선택 취소하고 각 필드에 대한 모든 값을 다시 표시합니다.

### [!UICONTROL 고급 검색]

[!UICONTROL 고급 검색] 기본 검색에 사용할 수 없는 필드 및 필터를 사용하여 검색할 수 있습니다. 예를 들어 특정 우선 순위 또는 문서 소유자 이름으로 프로젝트를 검색할 수 있습니다.

>[!NOTE]
>
>다음을 수행하려면 다음을 수행합니다 [!UICONTROL 고급 검색]를 선택해야 합니다. [!UICONTROL 고급 검색] 검색을 시작할 때 선택합니다. 기본 검색을 [!UICONTROL 고급 검색].

* [[!UICONTROL 고급 검색]을 사용합니다](#use-advanced-search)

#### [!UICONTROL 고급 검색]을 사용합니다

다음을 사용할 수 있습니다 [!UICONTROL 고급 검색] 특정 기준에 따라 검색을 필터링합니다.\
이 유형의 검색은 개체와 연결된 키워드를 기억할 수 없지만 객체에 대한 일부 특정 정보를 알고 있는 경우 유용합니다(예: 프로젝트 우선 순위, 문서 소유자 이름 등)

고급 검색을 수행하려면 다음을 수행하십시오.

1. 의 페이지 오른쪽 위 모서리 [!DNL Workfront]를 클릭하고 **[!UICONTROL 검색]** 아이콘 ![](assets/search-icon.png). 다음 [!DNL Search] 메뉴가 표시됩니다.

1. 아래쪽에서 [!UICONTROL 검색] 메뉴 아래의 **[!UICONTROL 고급 검색]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   다음 [!UICONTROL 고급 검색] 페이지 슬라이드는 오른쪽에서 열리고 이전 페이지의 대부분을 다룹니다.

1. 검색할 객체 유형을 선택합니다.\
   **[!UICONTROL 프로젝트]** 기본적으로 선택되어 있습니다.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (선택 사항) 목록 맨 위의 필드에 키워드를 입력합니다.
1. (선택 사항) **[!UICONTROL 결과 필터링]** 특정 필드 유형에 따라 검색 결과를 필터링하려면 목록에서 필드를 선택합니다. 필요한 경우 필드의 값도 선택합니다.\
   또는\
   새 필터를 추가합니다.

1. 클릭 **[!UICONTROL 검색]**.\
   검색과 일치하는 항목 목록이 오른쪽에 표시됩니다 [!UICONTROL 고급 검색] 도구 모음

1. (선택 사항) 검색 전에 있었던 페이지로 돌아가려면 를 클릭합니다. **[!UICONTROL 닫기]** 오른쪽 상단 모서리에서

>[!NOTE]
>
>다음 [!UICONTROL 검색 결과] 페이지가 포커스에 있을 때만 열린 상태로 유지됩니다. 페이지에서 멀리 클릭하거나 다른 페이지를 열면 [!UICONTROL 검색 결과] 페이지.
