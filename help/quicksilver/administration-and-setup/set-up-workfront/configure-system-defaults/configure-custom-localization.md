---
user-type: administrator
product-area: system-administration;setup
title: 사용자 지정 로컬라이제이션 구성
description: 사용자 정의 현지화를 사용하면 다른 언어로 사용자 정의 용어 및 구를 정의할 수 있습니다. 그런 다음 Workfront은 이러한 용어를 브라우저 설정에 설정된 언어로 표시합니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 7%

---

# 사용자 정의 현지화 구성

사용자 정의 현지화를 사용하면 다른 언어로 사용자 정의 용어 및 구를 정의할 수 있습니다. 그런 다음 Workfront에서는 이러한 용어를 사용자의 Adobe Identity Management(IMS) 설정에 있는 언어 세트로 표시합니다.

예를 들어 레이블 &quot;Target Audience&quot;를 설정하여 독일어 단어 &quot;Zielgruppe&quot;로 번역할 수 있습니다. 브라우저의 기본 언어로 선택된 독일어를 사용하는 모든 사용자에게는 영어로 &quot;Target Audience&quot;라는 레이블이 지정된 필드에 대한 레이블로 &quot;Zielgruppe&quot;라는 단어가 표시됩니다.

여러 언어로 번역을 구성할 수 있습니다. 현재 사용 가능한 언어는 다음과 같습니다.

* 중국어(번체)
* 중국어(간체)
* 프랑스어
* 독일어
* 이탈리아어
* 일본어
* 한국어
* 포르투갈어(브라질)
* 스페인어

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>워크플로우 Prime 이상 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>번역을 구성하려면 Workfront 관리자여야 합니다.</p>  </td> 
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 현지화 설정 시 고려 사항

현지화를 구성할 때는 다음 사항을 고려하십시오.

* 여러 언어로 번역하도록 용어를 구성할 수 있습니다.
* 현지화는 사용자 정의 필드 레이블(열 헤더로 사용되는 경우 포함) 및 도구 설명에 적용됩니다.
* 사용자 지정 현지화는 Business Rules에서 생성된 메시지에 적용할 수 있지만 Business Rule에서 활성화해야 합니다.

  자세한 내용은 비즈니스 규칙 만들기 및 편집 문서에서 [비즈니스 규칙에서 현지화 사용](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules)을 참조하십시오.

## 번역 구성

번역은 설정 영역에서 구성됩니다.

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. 설정 영역의 왼쪽 탐색 패널에서 **로컬라이제이션**&#x200B;을 클릭합니다.
1. 새 번역을 추가하려면 **새 행**&#x200B;을 클릭하세요.
1. **영어** 열에 번역할 영어 용어를 입력하십시오.
1. 용어를 번역할 언어의 열에 대상 언어로 용어를 입력합니다.
1. 단어를 추가 언어로 번역하려면 해당 언어 열에 번역을 추가합니다.
1. 언어 열의 순서를 바꾸려면 이동할 열의 헤더를 클릭하고 원하는 위치로 끕니다.
