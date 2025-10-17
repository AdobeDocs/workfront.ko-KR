---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트 설치
description: 프로덕션 환경 또는 샌드박스 환경에 블루프린트를 설치할 수 있습니다.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# 블루프린트 설치

<!-- Audited: 5/2025 -->

프로덕션 환경 또는 샌드박스 환경에 블루프린트를 설치할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>Workfront 관리자</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 블루프린트는 어디에서 설치해야 합니까? {#where-should-i-install-a-blueprint}

다음 환경 중 하나에 패키지를 설치할 수 있습니다.

<table style="table-layout:auto">
        <tr>
        <td><strong>프로덕션</strong></td>
        <td>프로덕션은 라이브 환경입니다.</td>
    </tr>
    <tr>
        <td><strong>샌드박스 미리보기</strong></td>
        <td>샌드박스 미리보기는 라이브 환경의 복제본 역할을 하는 테스트 환경이며 Adobe Workfront에서 매주 주말에 새로 고칩니다. 모든 지원 패키지는 샌드박스 미리보기에 액세스할 수 있습니다. 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">샌드박스 환경 미리 보기[!DNL Adobe Workfront]를 참조하십시오.</a></td>
    </tr>
    <tr>
        <td><strong>샌드박스 1 및 2</strong></td>
        <td>사용자 지정 새로 고침 샌드박스는 사용자가 수동으로 새로 고치는 별도의 테스트 환경입니다. 사용자 지정 새로 고침 샌드박스를 얻는 데 추가 비용이 있습니다. 자세한 내용은 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">사용자 지정 새로 고침 샌드박스 환경[!DNL Adobe Workfront]을 참조하십시오.</a></td>
    </tr>
</table>

>[!TIP]
>
>먼저 샌드박스 환경에 블루프린트를 설치하는 것이 좋습니다. 이렇게 하면 라이브 데이터를 변경하지 않고도 블루프린트의 콘텐츠를 테스트하고 조직에 잘 맞는지 확인할 수 있습니다.

>[!NOTE]
>
>특정 블루프린트는 테스트 목적으로 미리보기 환경에서만 설치할 수 있습니다. 프로덕션 환경, 샌드박스 1 또는 샌드박스 2에서 미리보기 전용 콘텐츠에 액세스하는 경우 설치 버튼이 활성화되지 않고 경고 메시지가 표시될 수 있습니다.\
>또한 환경 전환 기능은 미리보기 환경에 있는 경우에도 미리보기 전용 콘텐츠에 액세스할 때 제한됩니다.

## 블루프린트 설치

{{step1-to-blueprints}}

1. 설치할 블루프린트를 찾습니다. 페이지 오른쪽에서 사용 사례, 완성도, 설치 상태 및 유형별로 필터링할 수 있습니다.
1. (선택 사항) 블루프린트의 작동 방식을 알아보려면 **[!UICONTROL 세부 정보]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 설치]**&#x200B;를 클릭합니다.
1. 프로덕션 환경 또는 샌드박스 환경에 설치하도록 선택합니다.\
   자세한 내용은 [블루프린트는 어디에서 설치할 수 있습니까?이 문서의 &#x200B;](#where-should-i-install-a-blueprint) 섹션.
1. **구성** 페이지에서 다음 중 하나를 수행하도록 선택할 수 있습니다.

   * 블루프린트를 그대로 설치합니다. 구성이 필요하지 않은 블루프린트 유형의 경우 이 옵션만 제공됩니다. 구성이 필요한 블루프린트 유형의 경우 선택적으로 지금 블루프린트를 설치하고 나중에 구성할 수 있습니다. **[!UICONTROL 다음으로 설치]**&#x200B;를 클릭합니다.
   * 구성이 필요한 블루프린트에 대해 설치 전에 블루프린트를 구성합니다. 구성을 선택한 다음 **[!UICONTROL 블루프린트 설치]**&#x200B;를 클릭합니다.

     자세한 내용은 [블루프린트 구성](../../administration-and-setup/blueprints/configure-template-package.md)을 참조하세요.

   설치가 완료되고 메시지에 블루프린트와 함께 성공적으로 설치된 특정 개체(예: 역할, 팀 또는 그룹) 및 설치하지 못한 개체의 목록이 표시됩니다.

블루프린트를 설치한 후 블루프린트를 완전히 배포하려면 몇 가지 추가 작업이 필요할 수 있습니다. 자세한 내용은 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md)을 참조하세요.
