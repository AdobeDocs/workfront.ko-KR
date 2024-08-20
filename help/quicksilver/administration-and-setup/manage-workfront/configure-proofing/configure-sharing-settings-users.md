---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 사용자에 대한 공유 설정 구성
description: Adobe Workfront 관리자 또는 Workfront Proof 관리자는 증명을 공유할 수 있는 사용자 계정, 사용자가 모든 버전의 증명을 볼 수 있는지 여부 및 사용자가 공유 항목에 액세스할 수 있는 시기를 구성할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# 사용자에 대한 공유 설정 구성

Adobe Workfront 관리자 또는 Workfront Proof 관리자는 증명을 공유할 수 있는 사용자 계정, 사용자가 모든 버전의 증명을 볼 수 있는지 여부 및 사용자가 공유 항목에 액세스할 수 있는 시기를 구성할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 플랜: Pro 이상</p> <p>또는</p> <p>기존 플랜: Premium 또는 선택</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>증명 권한 프로필에서 관리자를 선택해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">사용자의 증명 액세스 구성</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 다른 계정과의 공유 구성

{{step1-to-proofing}}

1. **설정** > **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.

1. **공유** 섹션에서 **공유 허용** 오른쪽에 있는 **설정**&#x200B;을 클릭합니다.

1. 표시되는 드롭다운 목록에서 옵션을 선택하여 모든 사용자가 증명을 사용할 수 있도록 할지, 자신의 계정으로만 증명 공유를 제한할지, 아니면 자신의 계정 및 협업 중인 파트너 계정으로 증명을 제한할지 여부를 지정합니다.
1. **저장**&#x200B;을 클릭합니다.

## 공유 증명의 모든 버전에 대한 가시성 구성

{{step1-to-proofing}}

1. **설정** > **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.

1. **공유** 섹션에서 **받는 사람이 모든 버전을 볼 수 있음**&#x200B;의 오른쪽에 있는 **활성화** 또는 **비활성화**&#x200B;를 선택하여 증명 URL이 활성화된 경우 받는 사람이 증명 뷰어 내에서 모든 증명 버전을 볼 수 있도록 허용할지 여부를 지정합니다.

## 워크플로우 스테이지 활동을 기반으로 증명 가시성 구성

자동화된 워크플로를 사용하는 증명이 지정된 단계와 연관된 사용자에게 표시되는 시기를 지정할 수 있습니다.

>[!NOTE]
>
>* 이 옵션은 독립형 Workfront Proof 애플리케이션을 사용하는 경우에만 사용할 수 있으며, Workfront과 통합된 Workfront Proof 인스턴스를 사용하거나 Workfront 내에서 증명을 하는 경우에는 사용할 수 없습니다.
>* 사용자는 이 설정에 관계없이 사용자가 연결된 단계로 진입한 후에만 증명에 대한 이메일 알림을 받습니다.
>

자동화된 워크플로가 있는 증명이 사용자에게 표시되는 시기를 구성하려면 다음을 수행합니다.

{{step1-to-proofing}}

1. **설정** > **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.

1. **공유** 섹션에서 **단계 활성화에 따른 증명 표시 기능을 활성화하거나 비활성화합니다**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>사용 안 함</strong>(기본값)</td> 
      <td>증명은 증명을 만들 때 사용자에게 표시됩니다.<br><p>증명 워크플로의 단계와 연결된 모든 사용자는 증명이 생성된 직후 검색 결과에서 증명을 볼 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용</strong> </td> 
      <td> <p>증명은 연결된 단계가 <strong>활성 상태가 된 후에만 사용자에게 표시됩니다.</strong></p> <p><b>참고</b>:   
        <ul> 
         <li><em style="font-style: normal;">이 옵션을 사용하도록 설정하면 기존 증명이 만들어질 때 볼 수 있는 사용자에게 계속 표시됩니다.</em> </li> 
         <li>사용자가 증명 버전에 액세스할 수 있게 되면(사용자와 연결된 단계가 활성화되므로) 해당 단계가 활성화된 버전만 표시됩니다. 이전 버전이 사용자가 연결된 단계에 도달하지 않은 경우 해당 증명 버전을 볼 수 없습니다.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
