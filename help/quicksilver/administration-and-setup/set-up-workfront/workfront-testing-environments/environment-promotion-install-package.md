---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 환경 프로모션 패키지 설치
description: 환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 대상 환경에 환경 프로모션 패키지를 설치하는 방법을 알아봅니다.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: b26f20b13a18c6e727fcf9e267ba9c53e5b566dc
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# 환경 프로모션 패키지 설치

패키지를 만든 후에는 다른 환경에 설치할 수 있습니다.

개체를 복사할 환경에 패키지를 설치해야 합니다 **끝**. 예를 들어 사용자 정의 샌드박스 새로 고침 환경에서 프로젝트를 구성하고 프로덕션 환경으로 승격하는 경우 프로덕션 환경에 패키지를 설치해야 합니다.

>[!IMPORTANT]
>
>환경 프로모션을 위해 오브젝트를 구성하는 동안 사용자 정의 새로 고침 샌드박스를 새로 고치면 해당 구성이 새로 고침에서 손실됩니다. 미해결 환경 프로모션 개체 및 패키지가 모두 성공적으로 프로모션되지 않는 한 사용자 정의 샌드박스 새로 고침을 새로 고치지 않는 것이 좋습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 플랜</strong>
   </td>
   <td> Prime 또는 Ultimate(신규 계획만 해당)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 라이선스</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>액세스 수준 구성
   </td>
   <td>다음이어야 합니다: [!DNL Workfront] 관리자.
   </td>
  </tr>
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 전제 조건

환경 프로모션 패키지를 설치하려면 먼저 만들어야 합니다.

자세한 내용은 [환경 프로모션 패키지 만들기 또는 편집](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## 설치를 위한 패키지 상태

프로덕션 환경에 설치하려면 패키지가 활성 상태여야 합니다.

패키지를 테스트 상태로 이동하고 다른 샌드박스에 설치하여 패키지를 테스트하는 것이 좋습니다.  이 테스트가 성공하고 오류가 없으면 패키지를 활성으로 이동하여 프로덕션 환경에 설치합니다.

패키지 상태를 편집하려면:

1. 에 설명된 대로 패키지를 선택합니다  [기존 패키지 편집 또는 결합](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) 문서 환경 프로모션 패키지 만들기 및 편집
1. 클릭 **패키지 편집**.
1. 클릭 **상태**.
1. 드롭다운 메뉴에서 원하는 상태를 선택합니다.

상태에 대한 자세한 내용은 [환경 프로모션 상태](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) 문서 Workfront 환경 간 객체 이동에 대한 개요

## 패키지 설치

>[!NOTE]
>
>* 패키지를 설치하려면 패키지를 설치할 환경에 로그인해야 합니다. 객체를 복사하는 환경입니다 **끝**.

1. 패키지를 설치할 환경으로 이동합니다.
1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png).
1. 선택 **시스템** 왼쪽 탐색에서 을(를) 선택합니다. **환경 프로모션**.
1. 표시된 목록에서 패키지를 선택합니다.
1. 충돌이 있는 각 개체에 대해 충돌 해결 방법을 선택합니다.

   충돌을 해결하려면 객체 유형 옆에 있는 드롭다운 화살표를 클릭하고 수행할 작업을 선택합니다.

   자세한 내용은 [충돌](#collisions) 이 문서에서
1. 패키지를 새 환경에 배포하려면 **배포** 화면 오른쪽 상단에 있습니다.

## 충돌

충돌은 소스 환경에서 설치 중인 객체 중 하나와 일치하는 설치 대상 환경에서 발견된 객체입니다. 소스 객체의 이름과 ID를 대상 환경의 객체와 비교하여 충돌을 감지합니다. 또한 소스 객체와 이전에 설치된 객체의 기록을 비교하여 충돌을 감지합니다.

충돌이 발생하면 충돌 해결 방법을 선택할 수 있습니다. 충돌은 객체 레벨에서 해결됩니다.

각 객체 유형 옆에 있는 드롭다운을 클릭하여 충돌을 볼 수 있습니다. 충돌은 충돌(Collision) 열에 표시됩니다.

>[!NOTE]
>
>감지된 충돌은 재정의하거나 설치에서 사용할 개체가 아닐 수 있습니다. 감지된 충돌을 확인하여 설치 대상이 올바른지 확인하는 것이 좋습니다.

충돌을 해결하려면 배포 작업 열에서 작업을 선택하거나 이미 표시된 기본 작업을 사용합니다.

* **새 이름으로 만들기**: 대상 환경에서 새 개체를 만듭니다. 객체가 대상 환경에 존재하면 새 이름으로 새 객체를 작성할 수 있습니다. 대상 환경에 없는 경우 새 이름으로 개체를 만들거나 개체가 패키지에 있는 이름으로 개체를 만들 수 있습니다.
* **기존 항목 사용**: 패키지의 개체가 설치되지 않았으며 대상 환경에 이미 있던 개체가 변경되지 않았습니다.
* **덮어쓰기**: 패키지의 개체가 대상 환경의 기존 개체를 대체합니다.

  충돌이 감지되지 않더라도 덮어쓸 오브젝트를 선택할 수도 있습니다.

  덮어쓰기가 상위 및 하위 객체에 미치는 영향에 대한 자세한 내용은 [상위 및 하위 개체 덮어쓰기](#overwriting-parent-and-child-objects) 이 문서에서.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

기본값은 입니다. `Create new` 객체가 대상 환경에 없는 경우 `Use existing` 객체가 대상 환경에 있는 경우 을 클릭하여 기본 매핑으로 되돌릴 수 있습니다. **기본 매핑으로 재설정**.

## 상위 및 하위 개체 덮어쓰기

프로모션 패키지의 일부 오브젝트에 하위 오브젝트가 포함될 수 있습니다. 예를 들어 프로젝트(상위)에는 작업(하위)이 있습니다. 상위 객체를 덮어쓸 때 하위 객체는 다음과 같이 처리됩니다.

* 패키지와 대상 모두에 있는 하위 개체는 패키지와 일치하도록 대상에서 업데이트됩니다.
* 패키지에 있지만 대상이 아닌 하위 개체가 만들어집니다.
* 대상에 존재하지만 패키지가 아닌 하위 개체는 변경되지 않습니다.

이 기능은 다음 상위 및 하위 객체에 영향을 줍니다.

| 상위 오브젝트 | 하위 개체 |
|---|---|
| 프로젝트 | 작업<br>QueueDef(대기열 정의)<br>라우팅 규칙 |
| 템플릿 | TemplateTask<br>QueueDef(대기열 정의)<br>라우팅 규칙 |
| 매개 변수(사용자 정의 양식 필드) | ParameterOption(사용자 정의 양식 필드 옵션) |
| 캘린더 정보 | CalendarSection |
| QueueDef(대기열 정의) | 대기열 주제 그룹<br>대기열 주제 |

