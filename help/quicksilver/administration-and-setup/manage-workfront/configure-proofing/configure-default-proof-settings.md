---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 기본 증명 설정 구성
description: 이러한 설정을 사용하면 사용자가 만든 모든 새 증명에 적용되는 기본값을 설정할 수 있습니다. 그러나 사용자는 증명을 만들 때 이러한 설정의 대부분을 무시할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 7%

---

# 기본 증명 설정 구성

이러한 설정을 사용하면 사용자가 만든 모든 새 증명에 적용되는 기본값을 설정할 수 있습니다. 그러나 사용자는 증명을 만들 때 이러한 설정의 대부분을 무시할 수 있습니다.

## 새 증명 기본 설정 구성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정**.
1. 왼쪽 패널에서 **증명** > **증명 설정**.
1. 에서 **새 증명 기본값** 섹션에서 다음 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>수신자</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">로그인 필요</td> 
      <td> <p>검토자는 조직의 계정에서 만든 증명을 볼 수 있으려면 먼저 이메일과 암호를 사용하여 로그인해야 합니다. 사용하도록 설정하면 사용자가 게스트 검토자와 증명을 공유할 수 없습니다.</p> <p><b>중요 사항</b>: 활성화되면 새로 만든 모든 증명에 로그인이 필요합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">새 버전의 원본 증명에서 소유자 복사</td> 
      <td> <p>첫 번째 버전 증명의 소유자는 이러한 버전을 만드는 사람에 관계없이 연속적인 모든 버전의 소유자입니다. 이 설정은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 증명 주석을 삭제할 수 있도록 허용</td> 
      <td>사용자는 자신의 주석을 삭제할 수 있습니다. 이 설정은 기본적으로 활성화되어 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정 시 전자 서명 필요 </td> 
      <td> <p>의사 결정자는 증명에 대해 결정할 때 Workfront 로그인 자격 증명을 입력하라는 메시지가 표시됩니다.</p> <p><b>중요 사항</b>: 사용하도록 설정하면 사용자는 로그인 자격 증명이 없는 게스트 검토자와 증명을 공유할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>마감</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 기한 설정</td> 
      <td> <p>시스템에서 이 마감일을 자동화된 워크플로우가 없는 계정의 모든 새 증명에 적용합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">증명 위험 발생 전에 수신자에게 알림</td> 
      <td>수신자는 위에 지정된 최종 기한에 따라 증명이 위험 수준으로 간주되기 전에 이메일을 통해 알림을 받습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>이메일 알림</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">증명에 추가될 때 수신자에게 알림</td> 
      <td>수신자는 증명에 추가되면 이메일을 통해 알림을 받습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

## 증명 결정 구성

사용자는 증명 결정을 사용하여 검토 후 증명의 상태를 나타낼 수 있습니다.

>[!NOTE]
>
>증명 결정 뒤의 로직은 다양한 수준에 대한 여러 의사 결정이 있는 경우 증명 워크플로우의 전체 상태를 계산하는 데 사용됩니다. 결정 &quot;승인됨&quot; 및 &quot;변경 내용으로 승인됨&quot;은 자동 워크플로우에서 다음 단계를 트리거합니다.

증명 결정을 구성하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정**.
1. 왼쪽 패널에서 **증명** > **증명 설정**.
1. 에서 **결정**&#x200B;섹션에서 다음을 수행할 수 있습니다.

   1. **결정 이름 바꾸기**: 결정 상자 내의 텍스트를 클릭하고 새 결정 레이블을 입력합니다.

      >[!TIP]
      >
      >이름을 바꿀 때 결정에 대한 논리를 유지합니다. 예를 들어, 기본 결정 거부 를 *새 버전이 필요합니다.*, 그러나 (으)로 변경해서는 안 됩니다. *프린터로 보내기*.

      ![](assets/rename-decision-350x109.png)

   1. **결정 순서 재정렬**: 언어 교정 뷰어에 표시할 순서대로 의사 결정 상자를 드래그합니다.

      ![](assets/move-decision-350x110.png)

   1. **결정 숨기기**: 의사 결정 상자 위로 마우스를 가져간 다음 오른쪽 위 모서리에 있는 숨기기 아이콘을 클릭합니다.

      ![](assets/hide-decision-350x109.png)

1. (선택 사항) Workfront 기본값으로 돌아가려면 를 클릭합니다. **기본값 복원**.
1. **저장**&#x200B;을 클릭합니다.
