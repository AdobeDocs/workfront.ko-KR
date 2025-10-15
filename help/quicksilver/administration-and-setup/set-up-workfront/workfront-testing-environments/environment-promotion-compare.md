---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 환경 간 개체 비교
description: 여러 환경의 개체를 비교하여 환경 프로모션 패키지에 필요한 개체가 포함되어 있는지 확인할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 085b0f04-5a9c-49b9-86d7-2363731ee067
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# 환경 간 개체 비교

환경 간에 객체를 비교하여 환경 프로모션 패키지에 필요한 객체가 포함되어 있는지 확인할 수 있습니다.

비교할 객체 환경 및 유형을 선택합니다. Workfront은 두 환경에서 선택한 유형의 모든 객체를 비교하고 객체 차이점에 대한 데이터를 제공합니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td>Adobe Workfront 패키지
   </td>
   <td> <p>Prime 또는 Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront 라이선스</strong>
   </td>
   <td> <p>표준</p>&gt;
   </td>
  </tr>
   <tr>
   <td>액세스 수준 구성
   </td>
   <td><p>Workfront 관리자여야 합니다.</p>
   </td>
  </tr>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 전제 조건

환경 간에 개체를 비교하려면 조직이 Adobe Business Platform에 있어야 합니다.

## 개체 비교 생성

1. 객체를 비교할 환경으로 이동합니다.
1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 왼쪽 탐색에서 **시스템**&#x200B;을 선택한 다음 **환경 홍보**&#x200B;를 선택합니다.
1. 화면 오른쪽 상단 근처에 있는 **환경 비교**&#x200B;를 클릭합니다.
1. **Source 환경** 필드에서 패키지를 만들 환경을 선택합니다. **from**&#x200B;에서 개체를 복사하는 환경입니다.
1. **대상 환경** 필드에서 패키지를 설치할 환경을 선택합니다. **to** 개체를 복사하는 환경입니다.
1. **비교할 개체** 영역에서 환경 간에 비교할 개체 유형을 선택합니다.
1. 화면 오른쪽 상단 근처에 있는 **비교 생성**&#x200B;을 클릭합니다.

   비교는 비교되는 객체의 수와 크기에 따라 생성하는 데 시간이 걸릴 수 있습니다.

## 개체 비교 보기

비교 생성이 완료되면 비교가 표시됩니다.

이 목록에는 소스 환경에 있는 선택한 유형의 객체, 대상 환경에서 해당 객체가 누락되었는지 여부 및 두 객체 간에 필드 차이가 있는지 여부가 포함됩니다.

>[!BEGINSHADEBOX]

![비교 예](assets/environment-promotion-comparison.png)

이 예제에서는

* 첫 번째 줄은 대상 환경에 있지만 소스 환경과 다른 개체를 보여 줍니다.
* 두 번째 행은 대상 환경에 있는 객체를 나타내며 소스 환경과 동일합니다.
* 세 번째 줄은 대상 환경에 없는 개체를 보여 줍니다.

>[!ENDSHADEBOX]

특정 객체 차이를 보려면 다음과 같이 하십시오.

1. 해당 개체에 대한 줄에서 돋보기 아이콘 ![비교 아이콘](assets/compare-icon.png)을 클릭합니다.

   해당 오브젝트의 모든 필드가 있는 창이 열립니다. 차이점은 빨간색으로 표시됩니다.

## 개체 비교에서 패키지 만들기

개체 비교에서 직접 패키지를 만들 수 있습니다.

지침은 환경 프로모션 패키지 만들기 또는 편집 문서에서 [개체 비교에서 패키지 만들기](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison)를 참조하십시오.
