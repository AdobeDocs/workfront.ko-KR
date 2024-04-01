---
title: 레이아웃 템플릿을 사용하여 새 홈 맞춤화
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿 을 사용하여 사용자가 새 홈을 열 때 표시되는 내용을 구성할 수 있습니다.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 9de4a3729abe0ea2ee89df0be2974b714e65332a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 1%

---

# 레이아웃 템플릿을 사용하여 새 홈 맞춤화

레이아웃 템플릿 을 사용하여 사용자가 새 홈을 열 때 표시되는 내용을 구성할 수 있습니다.

다음을 구성할 수 있습니다.

* 기본적으로 작업 영역에 표시되는 위젯과 해당 레이아웃이 페이지에 표시됨
* 선택한 배경
* 내 프로젝트, 내 작업 및 내 문제 위젯에 사용할 수 있는 필터 및 그룹과 해당 기본값을 포함한 특정 위젯 설정

>[!IMPORTANT]
>
>이 페이지에 설명된 관리자 레이아웃 템플릿 선택 사항은 개별 사용자의 사용자 정의 선택 사항을 무시합니다.
>
>레이아웃 템플릿에 대한 변경 사항이 저장되면 해당 레이아웃 템플릿의 사용자는 레이아웃 템플릿과 일치하도록 새 홈 페이지를 변경하고 기존 위젯 선택 사항을 페이지 맨 아래로 푸시합니다. 관리자가 선택한 위젯은 사용자가 위치를 변경하고 크기를 조정할 수 있지만 제거할 수 없습니다.

새 홈에 대한 자세한 내용은 [새 홈 시작](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md).

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 레이아웃 템플릿을 사용하여 새 홈 맞춤화

1. 에 설명된 대로 레이아웃 템플릿에서 작업 시작 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. 아래쪽 화살표 클릭 ![](assets/dropdown-arrow.png) 아래에 **사용자에게 표시되는 항목 맞춤화**&#x200B;을 클릭한 다음 을 클릭합니다 **홈 작업 영역**.

1. 오른쪽에 나타나는 탭에서 다음 중 하나를 클릭합니다. **디자인 및 레이아웃** 위젯과 배경을 선택하고 정렬하려면 또는 **위젯 설정** 사용 가능한 필터 및 그룹과 같은 개별 위젯에 대한 설정을 관리합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">디자인 및 레이아웃</td> 
      <td>
      <p>사용자의 작업 영역에 표시될 위젯과 해당 위치를 선택하고 배경을 선택합니다. 사용자는 선택한 위젯을 제거할 수 없지만 자유롭게 이동하고 크기를 조정할 수 있으며 위젯을 추가할 수도 있습니다.</p>
      <p>이 탭은 기본적으로 작은 새 홈 작업 영역으로 작동합니다. 이에 설명된 단계에 따라 사용자 정의할 수 있습니다 <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">새 홈에서 위젯 추가, 편집 또는 제거</a>. 위젯을 선택하고 사용자에게 표시하려는 대로 작업 영역을 정렬합니다.</p>
      <p>배경을 변경하려면 다음 단계를 수행합니다 <b>백그라운드 사용자 정의</b> 위치: <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">새 홈 시작</a>.</p>
      <p>

>[!NOTE]
>
>레이아웃 템플릿에서 이동 또는 크기 조정 위젯만 사용자의 새 홈 페이지가 레이아웃을 업데이트하도록 트리거하지 않습니다. 하지만 위젯을 추가하거나 제거하면 사용자의 페이지에 대한 업데이트가 트리거됩니다.

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">위젯 설정</td> 
      <td>
      <p>개별 위젯에 대한 설정을 변경합니다. 현재는 세 가지 위젯만 지원됩니다.</p>
      <ul>
        <li>내 프로젝트</li>
        <li>내 작업</li>
        <li>내 문제</li>
      </ul>
      <p>편집할 위젯을 선택하면 사용 가능한 옵션이 오른쪽에 표시됩니다. 이러한 옵션은 다음과 같습니다 <b>필터</b>, <b>열</b>, 및 <b>그룹</b>. 다음을 수행할 수 있습니다.</p>
      <ul>
      <li><p><b>사용자가 사용할 수 있는 필터, 열 또는 그룹을 선택하고 순서를 지정합니다.</b></p>
      <p>목록에서 사용자가 사용할 수 있게 하려는 모든 옵션 옆에 있는 상자를 선택합니다. 선택하지 않은 옵션은 사용자에게 표시되지 않습니다. 목록에서 옵션을 끌어다 놓아 순서를 설정합니다.</li></p>
      <p>

>[!IMPORTANT]
>
>관리자 열 구성을 새 홈 페이지에 올바르게 적용하려면 사용자에게 보기에 대한 만들기 액세스 권한이 있어야 합니다.

</p>
      <li><p><b>위젯에 대한 기본 필터 또는 그룹 설정:</b></p>
      <p>옵션을 마우스로 가리키면 해당 옵션을 사용자의 기본값으로 설정할 수 있는 버튼이 표시됩니다. 현재 기본값은 오른쪽에 파란색 기본 배지가 있습니다.</li></p>
      <li><p><b>사용 가능한 옵션 목록에 기존 필터, 열 또는 그룹을 추가합니다.</b></p>
      <p>각 목록의 맨 아래에 있는 더하기 기호 버튼을 클릭하여 해당 목록에 옵션을 추가합니다. 기존 필터, 필드(열의 경우) 또는 그룹만 이 방법으로 추가할 수 있습니다.</p></li>
      </ul>
      <p>

>[!NOTE]
>
>레이아웃 템플릿을 사용하여 특정 위젯에 대한 기본 필터 또는 그룹화를 설정하는 경우 기존 사용자 환경 설정으로 인해 즉시 적용되지 않을 수 있습니다. 새 필터 또는 그룹화를 즉시 적용하려면 사용자 또는 사용자가 URL 끝에 &quot;/resetUser&quot;를 추가하여 사용자 환경 설정을 재설정해야 할 수 있습니다.

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장** 왼쪽 아래에 있습니다.
