---
product-area: user-management
navigation-topic: configure-your-user-profile
title: 사용자 정의 섹션 만들기
description: 에 표시되는 정보 [!DNL Workfront] 웹 응용 프로그램은 기본적으로 왼쪽 패널의 섹션에 표시되는 경우가 많습니다. 각 섹션에는 다음에 대한 다양한 정보가 포함되어 있습니다. [!DNL Workfront] 영역 또는 개체.
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 2%

---

# 사용자 정의 섹션 만들기

## [!DNL Adobe Workfront] 섹션

에 표시되는 정보 [!DNL Workfront] 웹 응용 프로그램은 기본적으로 왼쪽 패널 섹션에 표시되는 경우가 많습니다. 각 섹션에는 다음에 대한 다양한 정보가 포함되어 있습니다. [!DNL Workfront] 영역 또는 개체.\
의 기본 영역에 대한 자세한 정보 [!DNL Workfront], 문서 참조 [기본값 정보 [!DNL Adobe Workfront] 레이아웃](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

함께 제공되는 섹션 외 [!DNL Workfront] 기본적으로 워크플로우와 관련된 정보를 표시할 수 있는 대시보드를 추가할 수 있습니다. 모든 영역 및 개체에 대시보드를 추가할 수는 없습니다.

다음 표에는 [!DNL Workfront] 왼쪽 패널의 섹션이 포함된 영역 및 오브젝트 중 사용자 지정할 수 있는 영역 및 오브젝트는 다음과 같습니다.

| **[!DNL Workfront]영역 또는 개체** | **기본 시스템 섹션** | **사용자 정의 섹션** |
|---|---|---|
| [!UICONTROL 프로젝트] 영역 | ✓ 덧신 | ✓ |
| [!UICONTROL 팀] | ✓ |   |
| [!UICONTROL 요청] 영역 | ✓ |   |
| [!UICONTROL 타임시트] 영역 | ✓ |   |
| [!UICONTROL 포트폴리오] | ✓ | ✓ |
| [!UICONTROL 프로그램] | ✓ | ✓ |
| [!UICONTROL 프로젝트] | ✓ | ✓ |
| [!UICONTROL 작업] | ✓ |  ✓ |
| [!UICONTROL 문제] |  ✓ |  ✓ |
| [!UICONTROL 사용자] |  ✓ |  ✓ |
| [!UICONTROL 문서] |  ✓ |  ✓ |

{style="table-layout:auto"}

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td>[!UICONTROL Reviewer] 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td>객체 유형에 대한 액세스 보기</td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인하려면 다음으로 문의하십시오. [!DNL Workfront] 관리자.

## 의 왼쪽 패널에 대시보드 추가 [!DNL Workfront] 오브젝트 또는 영역

대시보드를 추가하려면 먼저 표시할 모든 정보를 사용하여 대시보드를 빌드해야 합니다. 외부 페이지를 작성할 수도 있습니다.\
대시보드 빌드에 대한 자세한 내용은 문서 를 참조하십시오 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
외부 페이지 빌드에 대한 자세한 내용은 문서 를 참조하십시오 [외부 웹 페이지를 대시보드에 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

대시보드 또는 외부 페이지를 작성한 후 왼쪽 패널에 추가할 수 있습니다.

1. 다음 중 하나로 이동 [!DNL Workfront] 왼쪽 패널에서 사용자 정의 섹션을 추가할 수 있는 영역 또는 개체입니다.\
   또는
1. 을(를) 추가할 수 있는 개체로 이동 [!UICONTROL 대시보드] 왼쪽 패널에서\
   사용자 정의 섹션을 추가할 수 있는 영역 및 객체에 대한 자세한 내용은 [[!DNL Adobe Workfront] 섹션](#adobe-workfront-sections).
1. 클릭 **[!UICONTROL 대시보드 추가]** 왼쪽 패널에서
1. 대시보드의 이름을 **[!UICONTROL 빠른 링크 이름]** 필드. 이 은(는) 귀하에게만 표시됩니다.
1. 에서 기존 대시보드 또는 외부 페이지의 이름을 입력하십시오. **[!UICONTROL 대시보드 선택]** 필드를 선택한 다음 목록에 표시될 때 대시보드를 선택합니다.
1. 클릭 **[!UICONTROL 추가]**.
1. (선택 사항) 표시할 순서대로 섹션을 끌어다 놓습니다.

   상단 섹션은 페이지의 기본 섹션입니다.

   개별 객체에 대해 생성한 섹션은 동일한 유형의 모든 객체에 액세스할 때 표시되며 해당 사용자만 사용할 수 있습니다.

## 오브젝트의 왼쪽 패널에 대시보드 표시

객체 아래에 대시보드를 추가하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [[!UICONTROL 대시보드 추가] Workfront 개체 또는 영역의 왼쪽 패널에서](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) 이 문서에서.

오브젝트 아래의 사용자 정의 섹션에 대시보드를 추가하면 오브젝트가 대시보드에 대한 필터 역할을 합니다. 예를 들어 대시보드에 작업 보고서를 추가하고 대시보드를 프로젝트에 추가하는 경우 프로젝트의 대시보드를 포함하는 사용자 정의 섹션에 보고 있는 프로젝트의 작업만 표시됩니다.

다음 객체는 객체가 표시되는 객체보다 계층 구조가 높은 경우 해당 객체에 대해 필터링됩니다.

* 프로젝트
* 작업
* 문제
* 승인 진행
* 참고
* 문서

객체의 계층 및 상호 종속성에 대한 자세한 내용은 섹션을 참조하십시오 [객체의 상호 의존성 및 계층](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 이 문서에서 [Adobe Workfront의 오브젝트 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 레이아웃 템플릿에서 왼쪽 패널 맞춤화

에 대시보드를 추가할 때 [!DNL Workfront] 예를 들어 사용자만 볼 수 있습니다.

다음 섹션에서 섹션을 사용자 지정할 수 있습니다. [!DNL Workfront] 레이아웃 템플릿에서 여러 사용자와 새 레이아웃을 공유할 수 있습니다. 시스템 또는 그룹 관리자만 레이아웃 템플릿에서 다른 사용자와 공유할 수 있습니다. 레이아웃 템플릿으로 왼쪽 패널 사용자 정의에 대한 자세한 내용은 [레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
