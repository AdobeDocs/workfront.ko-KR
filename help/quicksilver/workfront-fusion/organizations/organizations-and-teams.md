---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion 조직 및 팀
description: Adobe Workfront Fusion의 조직 및 팀 기능을 통해 기업은 Fusion 내의 시나리오 및 기타 기능에 대한 액세스를 제어할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 조직 및 팀

[!DNL Adobe Workfront Fusion]의 조직 및 팀 기능을 통해 기업은 Fusion 내의 시나리오 및 기타 기능에 대한 액세스를 제어할 수 있습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>작업 자동화 및 통합을 위한 Workfront Fusion,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 
     <p>넌 [!DNL Workfront Fusion] 조직의 관리자</p>
     <p>넌 [!DNL Workfront Fusion] 팀 관리자</p>
   </td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

<p>**에 대한 정보 [!DNL Adobe Workfront Fusion] 라이센스 <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 라이선스</a></p>


## 조직

[!DNL Workfront Fusion] 사용자가 조직에 속합니다. 사용자 [!DNL Fusion] 라이센스는 조직에서 사용할 수 있는 활성 시나리오 및 커넥터의 수를 결정합니다.

[!DNL Fusion] 라이센스는 조직에서 사용할 수 있는 활성 시나리오 및 활성 앱의 수를 결정합니다. [!DNL Fusion] 조직 대시보드에 현재 &quot;활성 시나리오&quot; 및 &quot;활성 앱&quot; 카운트를 표시합니다.

* [조직 역할](#organization-roles)
* [조직에 사용자 초대](#inviting-users-to-an-organization)

### 조직 역할

사용자에게는 조직에서 다음 역할 중 하나가 있습니다.

* **[!UICONTROL 소유자]**: 소유자에게는 조직에서 사용할 수 있는 모든 권한이 있습니다.
* **[!UICONTROL 관리]**: 관리자 역할을 사용하면 사용자가 조직의 팀 및 사용자를 만들고 관리할 수 있습니다.
* **[!UICONTROL 멤버]**: 구성원이 [!DNL Workfront Fusion] 하지만 조직을 변경할 수 없습니다.
* **[!UICONTROL 회계사]**: 회계사 역할은 사용자가 조직 대시보드에서 라이선스 정보를 볼 수만 있도록 해줍니다.
* **[!UICONTROL 앱 개발자]**: 이 역할의 기능은 현재 사용할 수 없으며, 가까운 시일 내에 사용할 수 있게 됩니다. 지금은 사용자를 이 역할에 할당하지 않는 것이 좋습니다.

### 조직에 사용자 초대

기본적으로 조직 소유자(또는 승인된 사용자)는 다른 사람을 해당 조직에 가입하도록 초대할 수 있습니다.

사용자를 조직에 가입하도록 초대하려면

1. 클릭 **[!UICONTROL 세부 사항 변경]** 화면 오른쪽 상단 모서리에서
1. 선택 **[!UICONTROL 새 사용자 초대]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. 사용자의 이메일 주소와 이름을 입력합니다.
1. 사용자의 역할을 선택합니다. 역할에 대한 자세한 내용은 [조직 역할](#organization-roles) 참조하십시오.
1. (선택 사항) 메모를 추가합니다. 이 메모는 사용자가 받은 초대 메일에 나타납니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

[!DNL Fusion] 은(는) 특정 조직 및 [!UICONTROL 역할 수락] 버튼을 클릭합니다.

![](assets/accept-the-role.png)

수신자가 버튼을 클릭하면 초대를 수락할 수 있는 초대 페이지로 리디렉션됩니다.

초대는 하루 후에 만료됩니다.

>[!NOTE]
>
>사용자가 [!DNL Fusion], [!DNL Fusion] 계정을 자동으로 만들고 임시 암호가 포함된 이메일을 보내어 새 사용자가 로그인하고 암호를 변경할 수 있도록 합니다.

## 팀

팀은 특정 리소스에 대한 액세스를 공유하는 사용자 그룹입니다. 이러한 리소스는 다음과 같습니다.

* 시나리오
* 연결
* Webhooks
* 키
* 데이터 저장소
* 데이터 구조
* 전자 메일 알림 설정

>[!NOTE]
>
>팀은 리소스에 대한 액세스를 제어하므로 경우에 따라 팀에 구성원이 하나만 있는 것이 유용합니다. 예를 들어, 교육 사용자는 개인과의 연결을 만들 수 있습니다 [!DNL Google] 계정. 모든 팀 구성원은 개인 [!DNL Google] 계정이므로 이 경우 사용자가 교육 팀의 유일한 구성원이 되는 것이 좋습니다.

조직에는 필요한 만큼 많은 팀이 있을 수 있으며 사용자는 하나 이상의 팀에 속할 수 있습니다.

사용자는 왼쪽 탐색 패널의 드롭다운 목록에서 해당 팀을 선택할 수 있습니다. 사용자는 자신이 구성원인 팀만 볼 수 있습니다. 팀을 선택하면 사용자가 해당 팀의 리소스에 액세스할 수 있습니다.

* [팀 역할](#team-roles)
* [팀 관리](#team-management)

### 팀 역할

사용자에게는 각 팀에서 다음 역할 중 하나가 있습니다.

* **[!UICONTROL 팀 관리자]**: 다른 팀 역할의 기능 외에도 사용자는 관리자 역할을 사용하여 팀 구성원의 역할을 추가, 제거 또는 변경할 수 있습니다.
* **[!UICONTROL 팀 구성원]**: 팀 구성원 역할을 사용하면 사용자가 시나리오를 만들고 실행할 수 있습니다.
* **[!UICONTROL 팀 모니터링]**: 다음 [!UICONTROL 모니터링] 역할을 사용하면 사용자가 시나리오에 대한 실행 정보에 액세스할 수 있지만 시나리오를 디자인하거나 &quot;활성&quot; 상태를 변경할 수 없습니다.
* **[!UICONTROL 팀 연산자]**: 다음 [!UICONTROL 연산자] 역할을 사용하면 실행 데이터를 보고 시나리오의 &quot;활성&quot; 상태를 변경할 수 있습니다.
* **[!UICONTROL 팀 제한 멤버]**: 이 역할의 기능은 현재 사용할 수 없으며, 가까운 시일 내에 사용할 수 있게 됩니다. 지금은 사용자를 이 역할에 할당하지 않는 것이 좋습니다.

### 팀 관리

* [팀 만들기](#create-a-team)
* [팀 알림 옵션 설정](#set-team-notification-options)

#### 팀 만들기

조직 소유자 및 관리자는 팀을 만들 수 있습니다.

팀을 만들려면 다음을 수행하십시오.

1. 왼쪽 탐색 패널에서 **[!UICONTROL 조직]**
1. 을(를) 선택합니다 **[!UICONTROL 팀]** 탭.
1. 클릭 **[!UICONTROL 새 팀 추가]** 팀 목록 아래에 있습니다.
1. 새 팀의 이름을 입력하고 **추가**.

#### 팀 알림 옵션 설정

전자 메일 알림 옵션은 팀 수준에서 설정됩니다.

1. 왼쪽 탐색 패널에서 **[!UICONTROL 팀]**
1. 을(를) 선택합니다 **[!UICONTROL 알림 옵션]** 탭.
1. 팀이 수신할 알림을 활성화합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL 시나리오 실행의 경고]'</td> 
      <td> <p>시나리오 실행에 경고가 발생하면 이메일을 수신합니다</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시나리오 실행의 오류]</td> 
      <td>시나리오 실행에 오류가 발생하면 이메일을 수신합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Scenario deactivation]</p> </td> 
      <td><p>시나리오가 비활성화되면 이메일을 수신합니다.</p><p><b>참고:</b> 오류로 인해 시나리오가 자동으로 비활성화된 경우에만 시나리오 비활성화에 대한 알림을 받게 됩니다. 수동으로 비활성화된 시나리오에 대한 알림을 받지 않습니다.</p><p>경우에 따라 시나리오가 [!DNL Workfront Fusion] 시나리오가 성능 또는 기타 문제를 야기하므로 엔지니어링 팀. 이러한 경우에서 알림을 받지 않습니다 [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

알림 옵션 변경 사항이 자동으로 저장됩니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->