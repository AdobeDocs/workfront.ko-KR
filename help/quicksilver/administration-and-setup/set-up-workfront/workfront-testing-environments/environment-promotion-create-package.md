---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 환경 프로모션 패키지 만들기 또는 편집
description: 환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 다른 환경에 설치할 수 있는 환경 프로모션 패키지를 만드는 방법에 대해 알아봅니다.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 6f5da5ede6bb8c98b26d7d37366670c89ded6c49
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# 환경 프로모션 패키지 만들기 또는 편집

**from** 개체를 복사할 환경에서 패키지를 만들어야 합니다. 예를 들어 사용자 정의 새로 고침 샌드박스 환경에서 프로젝트를 구성하고 프로덕션 환경으로 승격하는 경우 사용자 정의 새로 고침 샌드박스 환경에서 패키지를 생성해야 합니다.

>[!IMPORTANT]
>
>환경 프로모션을 위해 오브젝트를 구성하는 동안 사용자 정의 새로 고침 샌드박스를 새로 고치면 해당 구성이 새로 고침에서 손실됩니다. 미해결 환경 프로모션 개체 및 패키지가 모두 성공적으로 프로모션되지 않는 한 사용자 정의 샌드박스 새로 고침을 새로 고치지 않는 것이 좋습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 계획</strong>
   </td>
   <td> Prime 또는 Ultimate(신규 계획만 해당)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront]개 라이선스</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>액세스 수준 구성
   </td>
   <td>[!DNL Workfront] 관리자여야 합니다.
   </td>
  </tr>
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 패키지 만들기

1. 패키지를 생성할 환경으로 이동합니다. **from**&#x200B;에서 개체를 복사하는 환경입니다.
1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 왼쪽 탐색에서 **시스템**&#x200B;을 선택한 다음 **환경 홍보**&#x200B;를 선택합니다.
1. **패키지 만들기**&#x200B;를 클릭합니다.

   새 프로모션 패키지 페이지가 열립니다.

1. **패키지 이름** 필드에 패키지 이름을 입력합니다.
1. **설명** 필드에 이 패키지에 대한 설명을 입력하십시오.
1. 패키지에 개체를 추가하려면 왼쪽 탐색에서 **개체 추가**&#x200B;를 클릭하고 추가할 개체 유형을 선택하십시오.
1. 목록에서 하나 이상의 객체를 선택하거나 검색 막대에 이름을 입력하고 목록에 표시될 때 객체를 선택합니다. 목록에서 개체를 두 개 이상 선택할 수 있습니다.
1. 선택한 개체를 패키지에 추가하려면 **추가(X 개체)**&#x200B;를 클릭하십시오.

   >[!INFO]
   >
   >**예**
   >
   >프로젝트에 추가할 세 개의 프로젝트를 선택한 경우 단추에 **세 개의 프로젝트 추가**&#x200B;가 표시됩니다.

   추가한 개체는 페이지 오른쪽의 패키지 콘텐츠 영역에 나타납니다.

1. 다른 유형의 객체를 추가하려면 7-9단계를 반복합니다.
1. (선택 사항) 패키지에서 객체를 제거하려면 패키지 컨텐츠 영역의 객체를 마우스로 가리킨 다음 객체 옆에 있는 X를 클릭합니다.
1. 원하는 개체를 패키지에 모두 추가한 후 패키지를 어셈블하지 않고 저장하려면 **저장 및 닫기**&#x200B;를 클릭합니다.

   또는

   패키지를 저장하고 조합하려면 **저장 및 조합**&#x200B;을 클릭하세요.

   >[!NOTE]
   >
   >* 패키지에 5자 이상의 이름과 하나 이상의 개체가 모두 추가된 경우 저장 및 닫기, 저장 및 어셈블 단추를 사용할 수 있습니다.
   >* 테스트 또는 활성과 같이 설치 가능한 상태의 패키지는 어셈블할 수 없습니다.

## 기존 패키지 편집 또는 결합

1. 패키지를 생성할 환경으로 이동합니다. **from**&#x200B;에서 개체를 복사하는 환경입니다.
1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 왼쪽 탐색에서 **시스템**&#x200B;을 선택한 다음 **환경 홍보**&#x200B;를 선택합니다.
1. 표시된 목록에서 패키지를 선택합니다.
1. (조건부) 비활성화된 패키지를 보려면 **중단된 패키지 표시** 옵션을 활성화하십시오.
1. (선택 사항) 모든 개체와 하위 개체를 포함한 내용을 보려면 **내용** 섹션에서 개체 형식 옆에 있는 드롭다운 화살표를 클릭합니다.
1. (선택 사항) 이 패키지의 이전 설치 및 설치 시도를 보려면 **배포**&#x200B;를 클릭하십시오.
1. (선택 사항) 패키지를 편집하려면 화면 오른쪽 상단의 **패키지 편집**&#x200B;을 클릭합니다.
1. 패키지를 설치하려면 화면 오른쪽 상단의 **설치**&#x200B;를 클릭합니다.

   패키지 설치에 대한 지침은 [환경 프로모션 패키지 설치](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)를 참조하십시오.
