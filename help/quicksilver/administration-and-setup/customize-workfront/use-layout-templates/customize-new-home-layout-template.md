---
title: 레이아웃 템플릿을 사용하여 홈 맞춤화
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿을 사용하여 사용자가 Adobe Workfront에서 홈을 열 때 표시되는 내용을 구성할 수 있습니다.
author: Lisa and Courtney
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# 레이아웃 템플릿을 사용하여 홈 맞춤화

{{preview-fast-release-general}}

레이아웃 템플릿을 사용하여 사용자가 홈을 처음 열 때 표시되는 내용을 구성할 수 있습니다.

다음을 구성할 수 있습니다.

* 기본적으로 작업 공간에 표시되는 위젯
* 선택한 배경
* 내 프로젝트, 내 작업 및 내 문제 위젯에 사용할 수 있는 필터 및 그룹과 해당 기본값을 포함한 특정 위젯 설정

>[!IMPORTANT]
>
>최종 사용자는 레이아웃 템플릿이 적용된 후 페이지에서 배경을 변경하고 위젯을 재정렬할 수 있습니다. Workfront 관리자가 포함하는 위젯은 제거할 수 없습니다.
> 
>관리자는 사용자를 위한 새 위젯을 추가할 수 있습니다. 그러나 최종 사용자가 이미 위젯 순서 또는 배경 선택을 맞춤화한 경우 이러한 특정 맞춤화는 변경되지 않습니다.

홈에 대한 자세한 내용은 [홈 시작](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md)을 참조하세요.

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.</p>
        <p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레이아웃 템플릿을 사용하여 홈 맞춤화

레이아웃 템플릿을 사용하여 홈을 사용자 정의하려면 다음을 수행합니다.

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.

1. ![사용자에게 표시되는 항목 사용자 지정](assets/dropdown-arrow.png)에서 아래쪽 화살표 **아래쪽 화살표**&#x200B;를 클릭한 다음 **홈 Workspace**&#x200B;를 클릭합니다.

1. 오른쪽 탭에서 다음 중 하나를 클릭합니다.

   * **디자인 및 레이아웃**: 위젯과 배경을 선택하고 정렬하려면 선택하십시오.
   * **위젯 설정**: 사용 가능한 필터 및 그룹과 같은 개별 위젯에 대한 설정을 관리하려면 선택하세요.

   다음 표에는 각 탭에 대한 세부 사항이 나와 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">디자인 및 레이아웃</td> 
      <td>
      <p>사용자의 작업 영역과 위치에 표시할 위젯을 선택하고 배경을 선택합니다.</p> 
      <p>사용자는 선택한 위젯을 제거할 수 없지만 자유롭게 이동하고 크기를 조정할 수 있습니다. 위젯을 더 추가할 수도 있습니다.</p>
      <p>이 탭은 기본적으로 이 레이아웃 템플릿을 가진 사용자가 경험할 실제 홈 작업 영역의 미리 보기로 작동합니다.</p> 
      <p> 다음 중 하나를 수행합니다. </p>
      <ul><li><a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">홈에서 위젯 추가, 편집 또는 제거</a>에 설명된 단계에 따라 이 탭을 사용자 지정합니다. </li>
      <li>위젯을 선택하고 사용자에게 표시하려는 대로 작업 영역을 정렬합니다.</li>
      <li>배경을 변경하려면 <b>홈 시작</b>에서 <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">백그라운드 사용자 지정</a>의 단계를 따르십시오.</li></p>
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
      <p>개별 위젯에 대한 설정을 변경합니다.</p> 
      <p>

   >[!NOTE]
   >
   >이러한 옵션은 요약 패널까지 확장되지 않습니다. 레이아웃 템플릿의 요약 탭에서 해당 영역을 구성해야 합니다.

   </p>
      <p> 목록에서 왼쪽의 다음 위젯을 선택합니다.</p>
      <ul>
        <li>내 프로젝트</li>
        <li>내 작업</li>
        <li>내 문제</li>
      </ul>
      <p>편집하려는 위젯을 선택한 후 오른쪽에 있는 홈에서 사용할 수 있도록 하려는 <b>필터</b>, <b>열</b> 및 <b>그룹</b>을 선택합니다.</p>
      <p> 다음과 같은 작업을 수행할 수 있습니다.</p>
      <ul>
      <li><p>목록의 옵션 옆에 있는 상자를 선택하여 사용자가 사용할 수 있는 필터, 열 또는 그룹 순서를 지정합니다. 선택하지 않은 옵션은 사용자에게 표시되지 않습니다.</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* 필터, 열 및 그룹 옵션은 레이아웃 템플릿의 목록 사용자 지정 옵션에 연결됩니다. 여기에서 변경한 사항은 해당 설정에도 적용됩니다.
   >* 관리자 열 구성을 홈 페이지에 올바르게 적용하려면 사용자에게 보기에 대해 적어도 만들기 액세스 권한이 있어야 합니다.
   ></p>
   >   <li><p>옵션 위로 마우스를 이동하고 <b>기본값으로 설정</b>을 클릭하여 위젯에 대한 기본 필터 또는 그룹을 설정합니다. 현재 기본값은 오른쪽에 파란색 <b>기본</b> 배지를 표시합니다.</p></li>
   >   <li><p>각 목록 맨 아래에 있는 더하기 기호 버튼을 클릭하여 해당 목록에 옵션을 추가하여 사용 가능한 옵션 목록에 기존 필터, 열 또는 그룹을 추가합니다. 기존 필터, 필드(열의 경우) 또는 그룹만 이 방법으로 추가할 수 있습니다.</p></li>
   >   </ul>
   >   <p>

   >[!NOTE]
   >
   >레이아웃 템플릿을 사용하여 특정 위젯에 대한 기본 필터 또는 그룹화를 설정하는 경우 기존 사용자 환경 설정으로 인해 즉시 적용되지 않을 수 있습니다. 새 필터 또는 그룹화를 즉시 적용하려면 사용자 또는 사용자가 URL 끝에 &quot;/resetUser&quot;를 추가하여 사용자 환경 설정을 재설정해야 할 수 있습니다.

   </p>
      </td> 
      </tr>
      </tbody> 
      </table>

1. <span class="preview">미리 보기 환경에서: 레이아웃 템플릿을 계속 사용자 지정합니다. 언제든지 **적용**&#x200B;을 클릭하여 진행 상황을 저장할 수 있습니다.</span>

   <span class="preview">또는</span>

   <span class="preview">사용자 지정을 마쳤으면 **저장 후 닫기**&#x200B;를 클릭합니다.</span>

1. 프로덕션 환경에서: 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 왼쪽 하단의 **저장**&#x200B;을 클릭합니다.

   >[!IMPORTANT]
   >
   >레이아웃 템플릿의 사용자 정의를 보려면 사용자가 홈 페이지를 새로 고쳐야 합니다.
