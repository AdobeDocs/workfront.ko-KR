---
title: 브랜드 권한에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 Admin Console에서 사용자 그룹을 만들고 GenStudio system manager 제품 프로필을 할당하여 브랜드 권한을 구성할 수 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 4%

---

# 브랜드 권한에 대한 액세스 권한 부여

사용자는 사용자 그룹에 추가되면 Adobe GenStudio 시스템 관리자의 브랜드 만들기, 편집 및 게시 권한이 부여됩니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console 권한</td> 
   <td> <p>Adobe Admin Console에서 시스템 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요구 사항

* Workfront 인스턴스에는 통합 승인이 활성화되어 있어야 합니다.

* 조직에 GenStudio Foundation이 있어야 합니다.
   * Workfront의 컨텐츠 검토자는 자산 검토 및 승인 워크플로에 GenStudio Foundation에서 사용할 수 있는 기능을 제공합니다. 작업을 완료하기 위해 GenStudio Foundation에 직접 액세스할 필요는 없습니다. 콘텐츠 검토자를 통해 GenStudio Foundation 기능에 대한 액세스는 Workfront 계약 조건에 해당됩니다.
* Adobe은 파일에 서명된 Adobe Gen AI 계약이 있어야 합니다.
계약 서명에 대한 자세한 내용은 [Adobe Gen AI 계약 서명](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)을 참조하십시오.

## &#x200B;1. Admin Console에서 브랜드 권한 구성

### 1단계: 사용자 그룹 만들기

Admin Console에서 새 사용자 그룹을 만들어 브랜드 생성 및 편집에 대한 권한을 관리합니다.

### 2단계: 사용자 그룹에 제품 프로필 할당

할당된 프로필과 연결된 자격 부여는 이 그룹의 모든 사용자에게 GenStudio 브랜드 권한(브랜드 만들기, 업데이트 및 삭제)을 부여합니다.

프로파일을 할당하려면:

1. 새로 생성된 사용자 그룹으로 이동합니다.
1. **할당된 제품 프로필** 탭을 클릭합니다.
1. **프로필 할당**&#x200B;을 클릭합니다.
1. 팝업에서 제품 목록에서 **Adobe GenStudio**&#x200B;을(를) 선택한 다음 **적용**&#x200B;을 클릭합니다.
1. **Adobe GenStudio Foundation 편집기** 프로필을 선택하십시오.
1. **적용**&#x200B;을 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.

### 3단계: 사용자 그룹에 사용자 추가

브랜드를 만들고, 편집하고, 게시할 수 있는 권한을 사용자에게 할당하려면 해당 권한을 사용자 그룹에 추가합니다.

>[!NOTE]
>
>4단계에서 설명한 대로 그룹에 사용자를 추가하려면 먼저 사용자를 한 명 이상 추가해야 합니다.

사용자를 추가하려면:

1. **Admin Console** > **사용자** > **사용자 그룹**(으)로 이동합니다.
1. 사용자 그룹을 선택합니다.
1. 사용자 이름 또는 이메일 주소로 사용자를 추가합니다.
1. 기존 사용자에 대해 제안된 일치 항목 중에서 선택합니다.

### 4단계: 브랜드 프로젝트 만들기

프로젝트는 사용자가 브랜드 자산을 저장할 수 있는 저장소 위치를 제공합니다.

프로젝트를 만들려면 다음 작업을 수행하십시오.

1. Admin Console의 **저장소** 탭으로 이동합니다.
1. **프로젝트**&#x200B;를 클릭합니다.
1. **프로젝트 만들기**&#x200B;를 클릭합니다.
1. 팝업에 프로젝트 이름을 입력하십시오. **Adobe GenStudio 브랜드**.

   >[!IMPORTANT]
   >
   >표시된 대로 프로젝트 이름을 정확하게 입력합니다. 공백을 추가하거나 대소문자를 변경하지 마십시오.

1. Click **Create**.

### 5단계: 사용자 그룹을 프로젝트에 초대

사용자 그룹이 에셋에 액세스하고 관리할 수 있도록 브랜드 프로젝트에 추가합니다.

1. **프로젝트에 초대** 팝업에서 만든 사용자 그룹을 추가합니다.
1. **편집 가능** 권한을 선택합니다.
1. **초대**&#x200B;를 클릭합니다.

### 결과

이제 그룹의 사용자는 Workfront 내에서 브랜드 자산을 생성, 편집 및 게시할 수 있는 권한이 있습니다.

## &#x200B;2. Workfront 액세스 수준의 브랜드에 대한 액세스 권한 부여

Workfront 액세스 수준의 브랜드에 개별 사용자에게 액세스 권한을 부여하기 전에 이전 섹션의 모든 단계를 완료해야 합니다.

>[!IMPORTANT]
>
>* Admin Console에서 GenStudio system manager 제품 프로필이 있는 사용자 그룹에 할당된 사용자만 다른 사용자가 액세스 수준 설정에서 활성화된 브랜드에 액세스할 수 있더라도 Workfront에서 브랜드를 만들고 편집하고 게시할 수 있습니다.
>* 브랜드 액세스가 활성화된 액세스 수준에 추가되었지만 Admin Console에서 사용자 그룹에 추가되지 않은 사용자는 브랜드만 볼 수 있습니다.


Workfront 액세스 수준의 브랜드에 대한 액세스 권한을 부여하려면 다음을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **액세스 수준**&#x200B;을 클릭합니다.
1. 편집할 액세스 수준을 찾은 다음 편집 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭하여 편집합니다.

   또는

   새 액세스 수준을 만들려면 **새 액세스 수준**&#x200B;을 클릭하세요. 액세스 수준 만들기에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.
1. **추가 제한 설정**(으)로 스크롤한 다음 **사용자가 브랜드에 액세스할 수 있도록 허용**을 선택합니다.
   ![브랜드 액세스 허용 설정](assets/access-for-brands.png)
1. **저장**&#x200B;을 클릭합니다.

브랜드를 구성했으면 콘텐츠 검토자를 만들어 검토 및 승인 워크플로의 브랜드 지침에 따라 에셋을 검토할 수 있습니다. 자세한 내용은 [AI 공동 작업자 구성](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)을 참조하십시오.
