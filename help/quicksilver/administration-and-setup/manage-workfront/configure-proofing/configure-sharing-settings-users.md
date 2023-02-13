---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 사용자에 대한 공유 설정 구성
description: Adobe Workfront 관리자 또는 Workfront 증명 관리자는 증명을 공유할 수 있는 사용자 계정, 사용자가 증명의 모든 버전을 볼 수 있는지 여부, 사용자가 공유 항목에 액세스할 수 있는 시기를 구성할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# 사용자에 대한 공유 설정 구성

Adobe Workfront 관리자 또는 Workfront 증명 관리자는 증명을 공유할 수 있는 사용자 계정, 사용자가 증명의 모든 버전을 볼 수 있는지 여부, 사용자가 공유 항목에 액세스할 수 있는 시기를 구성할 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Premium 또는 선택</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>증명 권한 프로필에서 관리자를 선택해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">사용자의 언어 교정 액세스 구성</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 다른 계정과의 공유 구성

1. Workfront에서 기본 메뉴를 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 교정을 클릭합니다 ![](assets/proofing-in-main-menu.png) Workfront 증명 액세스

1. 클릭 **설정** > **계정 설정**&#x200B;를 클릭한 다음 **설정** 탭.

1. 에서 **공유** 섹션, 오른쪽 **공유 허용**&#x200B;를 클릭합니다. **설정**.

1. 표시되는 드롭다운 목록에서 옵션을 선택하여 누구나 증명을 사용할 수 있도록 할지, 증명을 자신의 계정으로만 공유할 수 있도록 제한할지, 아니면 자신의 계정과 함께 협력하는 파트너 계정으로 제한할 수도 있습니다.
1. 클릭 **저장.**

## 모든 버전의 공유 증명에 대한 가시성 구성

1. Workfront에서 기본 메뉴를 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 교정을 클릭합니다 ![](assets/proofing-in-main-menu.png) Workfront 증명 액세스

1. 클릭 **설정** > **계정 설정**&#x200B;를 클릭한 다음 **설정** 탭.

1. 에서 **공유** 섹션, 오른쪽 **수신자는 모든 버전을 볼 수 있습니다**, 선택 **활성화** 또는 **비활성화** 증명 URL이 활성화되어 있을 때 수신자가 교정 뷰어 내에서 모든 버전의 증명을 볼 수 있도록 허용할지 여부를 나타냅니다.

## 워크플로우 단계 활동을 기반으로 증명 가시성 구성

지정된 스테이지와 연결된 사용자가 자동화된 워크플로우를 통해 증명을 볼 수 있는 시기를 지정할 수 있습니다.

>[!NOTE]
>
>* 이 옵션은 독립 실행형 Workfront 증명 애플리케이션을 사용하는 경우에만 사용할 수 있습니다. Workfront과 통합된 Workfront 증명 인스턴스를 사용하거나 Workfront 내에서 언어 교정 시 사용할 수 없습니다.
>* 사용자는 이 설정에 관계 없이 사용자가 연결된 단계에 들어온 후에만 증명 전자 메일 알림을 받습니다.
>


사용자가 자동화된 워크플로우를 통해 증명을 볼 수 있는 시기를 구성하려면 다음을 수행하십시오.

1. Workfront에서 기본 메뉴를 클릭합니다. ![](assets/main-menu-icon.png)를 클릭한 다음 교정을 클릭합니다 ![](assets/proofing-in-main-menu.png) Workfront 증명 액세스

1. 클릭 **설정** > **계정 설정**&#x200B;를 클릭한 다음 **설정** 탭.

1. 에서 **공유** 섹션, 활성화 또는 비활성화 **단계 활성화 기반의 증명 가시성**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>비활성화됨</strong> (기본값)</td> 
      <td>증명을 만들 때 사용자가 증명을 볼 수 있습니다.<br><p>증명을 위한 워크플로우의 스테이지와 연결된 모든 사용자는 증명을 만든 직후 검색 결과에서 증명을 볼 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>활성화됨</strong> </td> 
      <td> <p>증명이 연결된 단계가 된 후에만 사용자가 증명을 볼 수 있습니다 <strong>활성화됨.</strong></p> <p><b>메모</b>:   
        <ul> 
         <li><em style="font-style: normal;">이 옵션을 활성화하면 기존 증명을 만들 때 볼 수 있는 사용자가 계속 볼 수 있습니다.</em> </li> 
         <li>사용자가 증명 버전에 액세스할 수 있게 되면(사용자와 연관된 스테이지가 활성 상태가 되므로) 사용자는 스테이지가 활성화된 버전만 볼 수 있습니다. 이전 버전이 사용자와 연결된 단계에 도달하지 않으면 사용자는 해당 버전의 증명을 볼 수 없습니다.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
