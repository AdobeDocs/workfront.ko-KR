---
product-area: projects
navigation-topic: use-the-home-area
title: 내 요청 위젯 사용
description: 내 요청 위젯에서 요청을 제출할 수 있습니다. 필터 및 열을 사용하여 위젯을 사용자 정의할 수도 있습니다.
author: Becky
feature: Get Started with Workfront
source-git-commit: 68379a6c41db1b694e2968d93de259cb7b0d8bc4
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 3%

---


# 내 요청 위젯 사용

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요.

내 요청 위젯은 조직에 제출된 요청을 표시합니다. 요청을 필터링하거나 특정 요청을 검색하거나 열 순서 및 가시성을 조정할 수 있습니다. 내 요청 위젯에서 새 요청을 만들 수도 있습니다.

>[!NOTE]
>
>내 요청 위젯이 로드되면 최대 50개의 요청이 표시됩니다. 요청을 더 표시하려면 목록을 아래로 스크롤합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Product]</strong></td> 
   <td> <ul><li>Adobe Workfront</li><li>Planning 요청 또는 요청 양식을 보려면 Adobe Workfront Planning이 있어야 합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>새로운 기능: 기여자 이상</p>
   또는   
   <p>현재: [!UICONTROL Request] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>대화에서 태그 지정되었거나 승인을 해결해야 하는 오브젝트(프로젝트, 작업, 문제, 문서)에 대한 액세스 권한 이상 보기</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>대화에서 태그가 지정되었거나 승인을 해결해야 하는 프로젝트, 작업, 문제, 문서에 대한 [!UICONTROL 보기] 이상의 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 만들기

내 요청 위젯에서 직접 요청을 만들 수 있습니다.

지침은 홈 영역에서 작업 항목 및 프로젝트 만들기 문서에서 [요청 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request)를 참조하십시오.

## 요청 필터링

내 요청 위젯에는 사용자 정의 가능한 필터가 있어 위젯에 표시되는 요청을 제어할 수 있습니다. 다양한 필드 및 값에 대해 이 필터를 구성하고 AND 및 OR를 사용하여 조건을 스택할 수 있습니다.

내 요청 위젯에서 필터를 구성하려면 다음을 수행합니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾습니다.
1. 내 요청 위젯에서 **필터**&#x200B;를 클릭합니다.
1. 맨 왼쪽 필드에서 필터링 기준으로 사용할 항목을 선택합니다. 사용 가능한 옵션은 다음과 같습니다.

   * 작업 영역
   * 오브젝트 유형
   * 입력 일자
   * 요청 양식
   * 상태
   * 작성자

1. 다음 필드에서 이 필터 조건에 사용할 연산자를 선택합니다. 사용 가능한 연산자는 선택한 필드에 따라 다릅니다.
1. (조건부) 연산자 오른쪽에 필드가 나타나면 필터링할 값을 선택합니다.
1. (선택 사항) 다른 필터 조건을 추가하려면 **조건 추가**&#x200B;를 클릭하고 4-6단계를 반복합니다.
1. (선택 사항 및 조건부) 여러 조건이 있는 경우 조건 왼쪽에 있는 **And** 또는 **Or**&#x200B;을 클릭하여 And 또는 Or 값을 전환합니다.

필터는 자동으로 저장됩니다.

>[!TIP]
>
>조직에서 Workfront Planning을 구매한 경우 내 요청 위젯에 Workfront 및 Workfront Planning 요청이 모두 포함됩니다.
> 
>* Workfront 요청만 필터링하려면 필터를 **개체 유형** > **다음 중 하나가 있습니다** > **문제**(으)로 설정하십시오.
>* Workfront Planning 요청만 필터링하려면 필터를 **개체 유형** > **다음 항목 없음** > **문제**(으)로 설정하십시오.

## 열 조정

내 요청 위젯에 표시할 사용 가능한 열을 선택하고 해당 순서를 설정할 수 있습니다.

사용 가능한 열은 다음과 같습니다.

* 제목
* 생성된 오브젝트
* 오브젝트 유형
* 상태
* 요청 양식
* 입력 일자
* 작성자

내 요청 위젯의 열을 조정하려면 다음을 수행합니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾습니다.
1. 내 요청 위젯에서 **열**&#x200B;을 클릭합니다.
1. (선택 사항)열 순서를 바꾸려면 이동할 열의 드래그 핸들 ![드래그 핸들](assets/drag-handle.png)을 클릭하고 원하는 위치로 드래그합니다. 목록 맨 위에 있는 열은 내 요청 위젯에서 가장 왼쪽 열로 표시됩니다.
1. (선택 사항) 토글을 사용하여 열이 내 요청 위젯에 표시되는지 여부를 제어합니다.

열 환경 설정은 자동으로 저장됩니다.

## 검색 요청

내 요청 위젯에서 특정 요청을 검색하려면 다음을 수행합니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾습니다.
1. 내 요청 위젯의 오른쪽 상단 근처에 있는 검색 막대에서 검색할 용어를 입력합니다.

   용어가 포함된 요청은 주황색으로 강조 표시됩니다.

1. (선택 사항) 강조 표시된 요청으로 이동하려면 검색 막대에서 위쪽 또는 아래쪽 화살표를 클릭합니다.





