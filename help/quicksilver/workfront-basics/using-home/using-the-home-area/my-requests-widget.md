---
product-area: projects
navigation-topic: use-the-home-area
title: 내 요청 위젯 사용
description: 내 요청 위젯에서 요청을 제출할 수 있습니다. 필터 및 열을 사용하여 위젯을 사용자 정의할 수도 있습니다.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 3893a57fb7ae31a1649b20beccc1f0b79f2421fb
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 3%

---

# 내 요청 위젯 사용

>[!IMPORTANT]
>
>이 문서에서는 새로운 내 요청 위젯에 대해 설명합니다. 새 위젯을 보려면 새 요청 경험을 활성화해야 합니다.
>요청 영역에서 새 요청 경험을 활성화할 수 있습니다.

내 요청 위젯은 사용자가 제출한 요청을 표시합니다. 요청을 필터링하거나 특정 요청을 검색하거나 열 순서 및 가시성을 조정할 수 있습니다. 내 요청 위젯에서 새 요청을 만들 수도 있습니다.

>[!NOTE]
>
>* 내 요청 위젯이 로드되면 최대 50개의 요청이 표시됩니다. 요청을 더 표시하려면 목록을 아래로 스크롤합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>모든 Workfront 또는 워크플로우 패키지</p>
   <p>Workfront Planning 요청 및 생성된 객체에 액세스할 수 있는 모든 Workfront Planning 패키지</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>대화에서 태그 지정되었거나 승인을 해결해야 하는 오브젝트(프로젝트, 작업, 문제, 문서)에 대한 액세스 권한 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>대화에서 태그가 지정되었거나 승인을 해결해야 하는 프로젝트, 작업, 문제, 문서에 대한 [!UICONTROL 보기] 이상의 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 만들기

내 요청 위젯에서 직접 요청을 만들 수 있습니다.

자세한 내용은 [홈 영역에서 작업 항목 및 프로젝트 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) 문서의 [요청 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) 섹션을 참조하십시오.

## 요청 복사

내 요청 위젯에서 요청을 복사하고 편집한 다음 새 요청으로 제출할 수 있습니다.

자세한 내용은 [요청 복사 및 제출](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)을 참조하십시오.

## 요청 필터링

내 요청 위젯에는 사용자 정의 가능한 필터가 있어 위젯에 표시되는 요청을 제어할 수 있습니다. 다양한 필드 및 값에 대해 이 필터를 구성하고 AND 및 OR 연산자를 사용하여 조건을 스택할 수 있습니다.

내 요청 위젯에서 필터를 구성하려면 다음을 수행합니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾은 다음 클릭하여 **Home**&#x200B;에 추가합니다.
1. **내 요청** 위젯에서 **필터**&#x200B;를 클릭합니다.
1. 필터링 기준으로 사용할 필드를 선택합니다. 사용 가능한 옵션은 다음과 같습니다.

   * 작업 영역
   * 오브젝트 유형
   * 입력 일자
   * 요청 양식
   * 상태
   * 작성자
   * 요청 또는 생성된 객체의 사용자 정의 필드

1. 다음 필드에서 이 필터 조건에 사용할 연산자를 선택합니다. 사용 가능한 연산자는 선택한 필드에 따라 다릅니다.
1. (조건부) 연산자 오른쪽에 필드가 나타나면 필터링할 값을 선택합니다.
1. (선택 사항) 다른 필터 조건을 추가하려면 **조건 추가**&#x200B;를 클릭하고 4~6단계를 반복합니다.
1. (선택 및 조건부) 조건이 여러 개인 경우 조건 왼쪽에 있는 **And** 또는 **Or**&#x200B;을 클릭하여 And 또는 Or 값을 전환합니다.

필터가 자동으로 저장됩니다.

>[!TIP]
>
>조직에서 Adobe Workfront 외에도 Workfront Planning을 구매한 경우 내 요청 위젯에 Workfront 및 Workfront Planning 요청이 모두 포함됩니다.
> 
>* Workfront 요청만 필터링하려면 필터를 **개체 유형** > **다음 중 하나가 있습니다** > **문제**(으)로 설정하십시오.
>* Workfront Planning 요청만 필터링하려면 필터를 **개체 유형** > **다음 항목 없음** > **문제**(으)로 설정하십시오.

## 열 조정 또는 추가

내 요청 위젯에 표시할 사용 가능한 열을 선택하고 해당 순서를 설정할 수 있습니다.

사용 가능한 열은 다음과 같습니다.

* 제목
* 생성된 오브젝트
* 오브젝트 유형
* 상태
* 요청 양식
* 입력 일자
* 작성자

내 요청 위젯의 열을 조정하려면 다음을 수행하십시오.

1. 오른쪽 상단에서 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾은 다음 클릭하여 **홈**&#x200B;에 추가합니다.
1. **내 요청** 위젯에서 **열**&#x200B;을 클릭합니다.
1. (선택 사항) 열의 순서를 바꾸려면 이동할 열의 드래그 핸들 ![드래그 핸들](assets/drag-handle.png)을 클릭하고 원하는 위치로 드래그합니다. 목록 맨 위에 있는 열이 내 요청 위젯에 첫 번째 열로 표시됩니다.
1. (선택 사항) 토글을 사용하여 요청 목록에서 열을 숨기거나 표시합니다.
1. 사용자 정의 필드를 열로 추가하려면 목록의 오른쪽 상단에 있는 **열 추가** 아이콘 ![열 추가](assets/add-column.png)를 클릭하고 위젯에 열로 추가할 사용자 정의 필드 옆에 있는 더하기 아이콘을 클릭합니다.

   목록의 개체에 첨부된 양식의 사용자 정의 필드를 열로 추가할 수 있습니다.

열 환경 설정은 자동으로 저장됩니다.

## 보기 만들기

내 요청 위젯에서 보기를 만들어 요청 목록에 정보가 표시되는 방식을 변경할 수 있습니다.

내 요청 위젯의 보기를 사용하여 작업할 때 다음 사항을 고려하십시오.

* 내 요청 위젯의 보기에는 보기에 적용된 열과 필터가 포함되어 있습니다.
* 보기를 만들고 다른 사용자와 공유할 수 있습니다. 공유하기 전에 보기에 대해 선택한 필터 및 열은 공유하는 보기에 포함됩니다.
* 다음은 편집, 공유 또는 삭제할 수 없는 시스템 보기입니다.

   * 위젯 통합 요청 기본 보기
* 내 요청 위젯에서 보기를 만들고 편집하는 것은 향상된 목록과 유사합니다. 자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.

## 검색 요청

내 요청 위젯에서 특정 요청을 검색하려면 다음을 수행합니다.

1. 오른쪽 상단에서 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾은 다음 클릭하여 **홈**&#x200B;에 추가합니다.
1. 내 요청 위젯의 오른쪽 상단에 있는 검색 막대에 검색할 용어를 입력합니다.

   용어가 포함된 요청은 주황색으로 강조 표시됩니다.

1. (선택 사항) 강조 표시된 요청으로 이동하려면 검색 막대에서 위쪽 또는 아래쪽 화살표를 클릭합니다.

## 요청에 의해 생성된 오브젝트로 이동

내 요청 위젯에서 요청에 의해 생성된 오브젝트를 찾을 수 있습니다.

>[!NOTE]
>
>생성된 객체에 대한 링크는 요청 자체가 객체를 생성한 경우 Planning 요청에 대해서만 새 요청 환경에서 사용할 수 있습니다. Workfront 요청이 프로젝트 또는 다른 오브젝트로 전환되는 경우 전환된 해당 오브젝트에 대한 링크를 새 요청 경험의 요청 목록에서 사용할 수 없습니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾은 다음 클릭하여 **Home**&#x200B;에 추가합니다.
1. 개체를 만든 요청을 찾습니다.
1. 해당 요청에 대한 **만들어진 개체** 열에서 개체 이름을 클릭합니다.

   객체의 페이지가 열립니다.

