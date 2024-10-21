---
title: 레이아웃 템플릿을 사용하여 새 홈 맞춤화
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿 을 사용하여 사용자가 홈을 열 때 표시되는 내용을 구성할 수 있습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 0a19683e2311b1acc57423f5cb5a7dd141c8b79c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# 레이아웃 템플릿을 사용하여 홈 맞춤화

레이아웃 템플릿 을 사용하여 사용자가 홈을 처음 열 때 표시되는 내용을 구성할 수 있습니다.

다음을 구성할 수 있습니다.

* 기본적으로 작업 공간에 표시되는 위젯
* 선택한 배경
* 내 프로젝트, 내 작업 및 내 문제 위젯에 사용할 수 있는 필터 및 그룹과 해당 기본값을 포함한 특정 위젯 설정

>[!IMPORTANT]
>
>최종 사용자는 레이아웃 템플릿이 적용된 후 페이지에서 배경을 변경하고 위젯을 재정렬할 수 있습니다. Workfront 관리자가 포함하는 위젯은 제거할 수 없습니다.
> <br>
>관리자는 사용자를 위한 새 위젯을 추가할 수 있습니다. 그러나 최종 사용자가 이미 위젯 순서 또는 배경 선택을 맞춤화한 경우 이러한 특정 맞춤화는 변경되지 않습니다.



홈에 대한 자세한 내용은 [홈 시작](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md)을 참조하세요.

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>새로운 기능: 표준</p>
  <p> 현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레이아웃 템플릿을 사용하여 홈 맞춤화

레이아웃 템플릿을 사용하여 홈을 사용자 정의하려면 다음을 수행합니다.

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.

1. **사용자에게 표시되는 항목 사용자 지정**&#x200B;에서 아래쪽 화살표 ![](assets/dropdown-arrow.png)을(를) 클릭한 다음 **홈 Workspace**&#x200B;을(를) 클릭합니다.

1. 오른쪽에 나타나는 탭에서 **디자인 및 레이아웃**&#x200B;을 클릭하여 위젯과 배경을 선택하고 정렬하거나 **위젯 설정**&#x200B;을 클릭하여 사용 가능한 필터 및 그룹과 같은 개별 위젯에 대한 설정을 관리합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">디자인 및 레이아웃</td> 
      <td>
      <p>사용자의 작업 영역에 표시될 위젯과 해당 위치를 선택하고 배경을 선택합니다. 사용자는 선택한 위젯을 제거할 수 없지만 자유롭게 이동하고 크기를 조정할 수 있으며 위젯을 추가할 수도 있습니다.</p>
      <p>이 탭은 기본적으로 작은 홈 작업 영역으로 작동합니다. 따라서 <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">홈에서 위젯을 추가, 편집 또는 제거</a>하는 단계에 따라 사용자 지정할 수 있습니다. 위젯을 선택하고 사용자에게 표시하려는 대로 작업 영역을 정렬합니다.</p>
      <p>배경을 변경하려면 <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">홈 시작</a>에서 <b>백그라운드 사용자 지정</b>의 단계를 따르십시오.</p>
      <p>

>[!NOTE]
>
>레이아웃 템플릿에서 이동 또는 크기 조정 위젯만 사용자의 홈 페이지가 레이아웃을 업데이트하도록 트리거하지 않습니다. 하지만 위젯을 추가하거나 제거하면 사용자의 페이지에 대한 업데이트가 트리거됩니다.

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
      <p>편집할 위젯을 선택하면 사용 가능한 옵션이 오른쪽에 표시됩니다. 이러한 옵션에는 <b>필터</b>, <b>열</b> 및 <b>그룹</b>이 포함됩니다. 다음을 수행할 수 있습니다.</p>
      <ul>
      <li><p><b>사용자가 사용할 수 있는 필터, 열 또는 그룹을 선택하고 순서를 지정합니다.</b></p>
      <p>목록에서 사용자가 사용할 수 있게 하려는 모든 옵션 옆에 있는 상자를 선택합니다. 이러한 옵션은 요약 패널까지 확장되지 않습니다. 레이아웃 템플릿의 요약 탭에서 해당 영역을 구성해야 합니다. 선택하지 않은 옵션은 사용자에게 표시되지 않습니다. 목록에서 옵션을 끌어다 놓아 순서를 설정합니다.</li></p>
      <p>

>[!IMPORTANT]
>
>* 필터, 열 및 그룹 옵션은 레이아웃 템플릿의 목록 사용자 지정 옵션에 연결됩니다. 여기에서 변경한 사항은 해당 설정에도 적용됩니다.
>* 관리자 열 구성을 홈 페이지에 올바르게 적용하려면 사용자에게 보기에 대해 적어도 만들기 액세스 권한이 있어야 합니다.

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

   사용자 지정을 마쳤으면 왼쪽 하단의 **저장**&#x200B;을 클릭합니다.

>[!IMPORTANT]
>
>레이아웃 템플릿의 사용자 정의를 보려면 홈 페이지를 새로 고쳐야 합니다.
