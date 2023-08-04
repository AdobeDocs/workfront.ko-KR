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
source-git-commit: 6531f318d9fb34b38a378a28e4d478c428bd1c25
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 조직 및 팀

[!DNL Adobe Workfront Fusion]의 조직 및 팀 기능을 사용하면 기업에서 Fusion 내의 시나리오 및 기타 기능에 대한 액세스를 제어할 수 있습니다.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> 
     <p>다음이어야 합니다: [!DNL Workfront Fusion] 조직의 관리자.</p>
     <p>다음이어야 합니다: [!DNL Workfront Fusion] 팀 관리자.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

<p>**다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 라이선스</a></p>


## 조직

[!DNL Workfront Fusion] 사용자가 조직에 속합니다.

* [조직 역할](#organization-roles)
* [조직에 사용자 초대](#inviting-users-to-an-organization)
* [조직 간 전환](#switch-between-organizations)

### 조직 역할

사용자에게는 조직에서 다음 역할 중 하나가 있습니다.

* **[!UICONTROL 소유자]**: 소유자는 조직에서 사용 가능한 모든 권한을 가지고 있습니다.
* **[!UICONTROL 관리자]**: 관리자 역할을 통해 사용자는 조직의 팀 및 사용자를 만들고 관리할 수 있습니다.
* **[!UICONTROL 멤버]**: 구성원은 다음을 사용할 수 있습니다. [!DNL Workfront Fusion] 그러나 조직을 변경할 수 없습니다.
* **[!UICONTROL 회계사]**: 회계사 역할은 사용자가 조직 대시보드에서 라이선스 정보만 볼 수 있도록 허용합니다.
* **[!UICONTROL 앱 개발자]**: 이 역할의 기능은 현재 사용할 수 없으며 곧 제공될 예정입니다. 지금은 이 역할에 사용자를 할당하지 않는 것이 좋습니다.

### 조직에 사용자 초대

기본적으로 조직 소유자(또는 인증된 사용자)는 다른 사용자를 초대하여 조직에 가입할 수 있습니다.

사용자를 조직에 초대하려면 다음 작업을 수행하십시오.

1. 클릭 **[!UICONTROL 세부 정보 변경]** 화면의 오른쪽 상단에 있습니다.
1. 선택 **[!UICONTROL 새 사용자 초대]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. 사용자의 이메일 주소와 이름을 입력합니다.
1. 사용자의 역할을 선택합니다. 역할에 대한 자세한 내용은 [조직 역할](#organization-roles) 이 문서에서.
1. (선택 사항) 메모를 추가합니다. 이 메모는 사용자가 받는 초대 이메일에 표시됩니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

[!DNL Fusion] 은(는) 특정 조직 및 [!UICONTROL 역할 수락] 단추를 클릭합니다.

![](assets/accept-the-role.png)

수신자가 버튼을 클릭하면 초대를 수락할 수 있는 초대 페이지로 리디렉션됩니다.

초대장이 하루 후에 만료됩니다.

>[!NOTE]
>
>을 처음 사용하는 사용자인 경우 [!DNL Fusion], [!DNL Fusion] 은(는) 자동으로 계정을 만들고 임시 암호가 포함된 이메일을 보내어 새 사용자가 로그인하고 암호를 변경하도록 지시합니다.

### 조직 간 전환

Fusion에서 두 개 이상의 조직에 속해 있을 수 있습니다. 조직 간에 자원이 공유되지 않습니다.

오른쪽 상단에 있는 조직 이름을 클릭하고 드롭다운에서 새 조직을 선택하여 Adobe 통합 경험 내에서 조직을 전환할 수 있습니다. Adobe에서 다른 조직의 멤버인 경우에도 Fusion 계정이 있는 조직만 드롭다운에 표시됩니다.

## 팀

팀은 특정 리소스에 대한 액세스 권한을 공유하는 사용자 그룹입니다. 이러한 리소스에는 다음이 포함될 수 있습니다.

* 시나리오
* 연결
* 웹훅
* 키
* 데이터 저장소
* 데이터 구조
* 이메일 알림 설정

>[!NOTE]
>
>팀이 리소스에 대한 액세스를 제어하므로 팀에는 한 명의 멤버만 있는 것이 유용한 경우도 있습니다. 예를 들어 교육 중인 사용자는 개인에 대한 연결을 만들 수 있습니다 [!DNL Google] 계정. 모든 팀원이 개인에 연결할 수도 있습니다. [!DNL Google] 계정, 따라서 이 경우 사용자가 교육 팀의 유일한 멤버인 것이 좋습니다.

조직에는 필요한 만큼 많은 팀이 있을 수 있으며 사용자는 하나 이상의 팀에 속할 수 있습니다.

사용자는 왼쪽 탐색 패널의 드롭다운 목록에서 팀을 선택할 수 있습니다. 사용자는 자신이 구성원으로 있는 팀만 볼 수 있습니다. 팀을 선택하면 사용자가 해당 팀의 리소스에 액세스할 수 있습니다.

* [팀 역할](#team-roles)
* [팀 관리](#team-management)

### 팀 역할

사용자는 각 팀에서 다음 역할 중 하나를 수행합니다.

* **[!UICONTROL 팀 관리자]**: 관리자 역할을 통해 다른 팀 역할의 기능 외에도 팀 구성원의 역할을 추가, 제거 또는 변경할 수 있습니다.
* **[!UICONTROL 팀원]**: 팀 구성원 역할을 통해 사용자는 시나리오를 만들고 실행할 수 있습니다.
* **[!UICONTROL 팀 모니터링]**: [!UICONTROL 모니터링] 역할을 통해 사용자는 시나리오의 실행 정보에 액세스할 수 있지만 시나리오를 디자인하거나 &quot;활성&quot; 상태를 변경할 수 없습니다.
* **[!UICONTROL 팀 운영자]**: [!UICONTROL 연산자] 역할을 통해 사용자는 실행 데이터를 보고 시나리오의 &quot;활성&quot; 상태를 변경할 수 있습니다.
* **[!UICONTROL 팀 제한된 구성원]**: 이 역할의 기능은 현재 사용할 수 없으며 곧 제공될 예정입니다. 지금은 이 역할에 사용자를 할당하지 않는 것이 좋습니다.

팀 역할에 사용할 수 있는 특정 작업에 대한 자세한 내용은[조직 및 팀 역할](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### 팀 관리

* [팀 만들기](#create-a-team)
* [팀 알림 옵션 설정](#set-team-notification-options)

#### 팀 만들기

조직 소유자 및 관리자는 팀을 만들 수 있습니다.

팀을 만들려면 다음 작업을 수행하십시오.

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 조직]**
1. 다음 항목 선택 **[!UICONTROL 팀]** 탭.
1. 클릭 **[!UICONTROL 새 팀 추가]** 팀 목록 아래에 있습니다.
1. 새 팀의 이름을 입력하고 **추가**.

#### 팀 알림 옵션 설정

이메일 알림 옵션은 팀 수준에서 설정됩니다.

1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL 팀]**
1. 다음 항목 선택 **[!UICONTROL 알림 옵션]** 탭.
1. 팀이 수신할 알림을 활성화합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Warning in scenario run]'</td> 
      <td> <p>시나리오 실행에서 경고가 있을 때 이메일 수신</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시나리오 실행 오류]</td> 
      <td>시나리오 실행에 오류가 있을 때 이메일을 받습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 시나리오 비활성화]</p> </td> 
      <td><p>시나리오가 비활성화되면 이메일을 받습니다.</p><p><b>참고:</b> 오류로 인해 시나리오가 자동으로 비활성화되는 경우에만 시나리오 비활성화에 대한 알림이 표시됩니다. 수동으로 비활성화된 시나리오에 대한 알림은 받지 않습니다.</p><p>경우에 따라 시나리오는 [!DNL Workfront Fusion] 엔지니어링 팀 이유는 시나리오가 성능 또는 기타 문제를 일으키기 때문입니다. 이러한 경우에서 알림을 받지 않습니다. [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

알림 옵션 변경 사항이 자동으로 저장됨

#### 팀 간 전환

Fusion에서 두 개 이상의 팀에 속해 있을 수 있습니다. 팀은 리소스를 공유하지 않으므로 특정 시나리오나 다른 리소스에 액세스하려면 팀을 전환해야 할 수 있습니다.

조직이 통합 경험 Adobe에 없는 경우 왼쪽 탐색에서 팀 이름을 클릭한 다음 드롭다운에서 팀을 선택하여 팀을 전환할 수 있습니다.

팀이 통합 경험 Adobe에 있는 경우 헤더에서 팀 이름을 클릭한 다음 드롭다운에서 팀을 선택하여 새 팀을 선택할 수 있습니다. 이 옵션은 시나리오 페이지 또는 연결 페이지와 같이 특정 팀에 해당되는 모든 페이지에서 사용할 수 있습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->