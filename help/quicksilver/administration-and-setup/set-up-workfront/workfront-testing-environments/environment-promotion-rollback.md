---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 환경 프로모션 패키지 롤백
description: 환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 대상 환경에서 설치된 프로모션 패키지를 롤백하는 방법에 대해 알아봅니다.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 환경 프로모션 패키지 롤백



패키지를 설치한 후 롤백할 수 있습니다. 이렇게 하면 대상 환경에서 패키지가 변경한 사항이 제거되고 영향을 받는 오브젝트가 이전 구성으로 복원됩니다.

프로모션 패키지를 설치한 후 24시간 이내에 롤백할 수 있습니다. 24시간이 지나면 해당 설치에 롤백 기능을 더 이상 사용할 수 없습니다.

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

* 환경 프로모션 패키지를 설치해야 롤백할 수 있습니다.

  지침은 [환경 프로모션 패키지 설치](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)를 참조하십시오.


## 특정 패키지 배포를 롤백할 수 있는지 확인

특정 패키지 배포를 롤백할 수 있는지 확인하려면 다음을 고려하십시오.

* 패키지를 설치한 후 24시간 미만이 경과해야 합니다.
* 가장 최근 패키지 배포만 롤백할 수 있습니다.
* 실패한 배포는 롤백할 수 있습니다.
* 롤백을 롤백할 수 없습니다.


## 설치된 환경 프로모션 패키지 롤백

1. 패키지가 설치된 환경으로 이동합니다.
1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 왼쪽 탐색에서 **환경 승격**&#x200B;을 선택합니다.
1. 롤백할 패키지를 선택하고 **배포**&#x200B;를 클릭합니다.
1. 롤백하려는 배포(설치) 위로 마우스를 가져간 다음 해당 배포 줄의 오른쪽에 나타나면 롤백을 클릭합니다.

   또는

   롤백하려는 배포를 클릭한 다음 화면 오른쪽 상단의 **패키지 롤백**&#x200B;을 클릭합니다.

   >[!IMPORTANT]
   >
   >롤백하기 전에 배포가 24시간 이내에 발생했을 수 있습니다. 24시간 이상 된 설치는 롤백할 수 없습니다.

1. (선택 사항) 롤백 미리 보기 영역에서 배포가 롤백될 때 발생하는 변경 사항을 확인합니다.
1. 화면 오른쪽 상단의 **되돌리기**&#x200B;를 클릭합니다.
