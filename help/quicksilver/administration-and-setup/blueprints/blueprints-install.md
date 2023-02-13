---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트 설치
description: 프로덕션 환경 또는 샌드박스 환경에 블루프린트를 설치할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 블루프린트 설치

프로덕션 환경 또는 샌드박스 환경에 블루프린트를 설치할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td> 
   <td> <p> 모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 라이선스</strong></td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>[!UICONTROL System 관리자]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 블루프린트는 어디에서 설치해야 합니까? {#where-should-i-install-a-blueprint}

다음 환경에 패키지를 설치할 수 있습니다.

<table style="table-layout:auto">
        <tr>
        <td><strong>프로덕션</strong></td>
        <td>프로덕션은 라이브 환경입니다.</td>
    </tr>
    <tr>
        <td><strong>샌드박스 미리보기</strong></td>
        <td>샌드박스 미리 보기는 라이브 환경의 복제본 역할을 하며 Workfront에서 매주 새로 고침되는 테스트 환경입니다. 모든 지원 패키지는 샌드박스 미리 보기에 액세스할 수 있습니다. 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">다음 [!DNL Adobe Workfront] 샌드박스 환경 미리 보기</a>.</td>
    </tr>
    <tr>
        <td><strong>샌드박스 1 및 2</strong></td>
        <td>사용자 지정 새로 고침 샌드박스는 사용자가 수동으로 새로 고치는 별도의 테스트 환경입니다. 사용자 지정 새로 고침 샌드박스를 얻는 데 추가 비용이 있습니다. 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">다음 [!DNL Adobe Workfront] 사용자 지정 새로 고침 샌드박스 환경</a>.</td>
    </tr>
</table>

>[!TIP]
>
>먼저 샌드박스 환경에 블루프린트를 설치하는 것이 좋습니다. 그렇게 하면 라이브 데이터를 변경하지 않고 블루프린트의 컨텐츠를 테스트하고 조직에 적합한지 확인할 수 있습니다.

>[!NOTE]
>
>특정 블루프린트는 테스트 목적으로 미리 보기 환경에서만 설치할 수 있습니다. 프로덕션 환경, Sandbox 1 또는 Sandbox 2에서 미리 보기 전용 컨텐츠에 액세스하는 경우 설치 버튼이 활성화되지 않으며 경고 메시지가 표시될 수 있습니다.\
>또한 미리 보기 환경에 있는 경우에도 미리 보기 전용 컨텐츠에 액세스할 때 환경 전환 기능이 제한됩니다.

## 블루프린트 설치

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 블루프린트]**.
1. 설치할 블루프린트를 찾습니다. 사용 사례, 완성도 수준, 설치 상태, 오른쪽의 입력 등을 기준으로 필터링할 수 있습니다.
1. (선택 사항) **[!UICONTROL 세부 사항]** 블루프린트 작동 방식을 알아봅니다.
1. 클릭 **[!UICONTROL 설치]**.
1. 프로덕션 환경 또는 샌드박스 환경에 설치하도록 선택합니다.\
   자세한 내용은 [블루프린트는 어디에서 설치해야 합니까?](#where-should-i-install-a-blueprint) 섹션에 자세히 설명되어 있습니다.
1. 설정 [!UICONTROL 구성] 페이지에서 다음 중 하나를 수행하도록 선택할 수 있습니다.

   * 블루프린트를 있는 그대로 설치합니다. 구성이 필요하지 않은 블루프린트 유형의 경우 이 옵션만 제공됩니다. 구성이 필요한 블루프린트 유형의 경우 필요에 따라 블루프린트를 지금 설치하고 나중에 구성하도록 선택할 수 있습니다. 클릭 **[!UICONTROL 그대로 설치]**.
   * 구성이 필요한 블루프린트에 대해 설치 전에 블루프린트를 구성합니다. 구성을 선택하고 **[!UICONTROL 블루프린트 설치]**.\

      자세한 내용은 [블루프린트 구성](../../administration-and-setup/blueprints/configure-template-package.md).
설치가 완료되면 블루프린트와 함께 성공적으로 설치된 특정 개체(예: 역할, 팀 또는 그룹)와 설치하지 못한 개체 목록이 메시지에 표시됩니다.

블루프린트를 설치한 후 완전히 배포하려면 몇 가지 추가 작업이 필요할 수 있습니다. 자세한 내용은 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
