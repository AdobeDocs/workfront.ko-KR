---
title: 레이아웃 템플릿을 사용하여 사용자 인터페이스 용어 사용자 지정
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 관리자는 레이아웃 템플릿을 사용하여 Workfront 전체에 표시되는 일부 객체의 레이블을 조직에서 사용하는 용어와 일치하도록 변경할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# 레이아웃 템플릿을 사용하여 사용자 인터페이스 용어 사용자 지정

Adobe Workfront 관리자는 레이아웃 템플릿을 사용하여 Workfront 전체에 표시되는 일부 객체의 레이블을 조직에서 사용하는 용어와 일치하도록 변경할 수 있습니다.

용어를 변경한 레이아웃 템플릿을 저장한 다음 Workfront에서 로그아웃한 다음 다시 로그인하면 변경한 레이블이 Workfront의 대부분의 영역에 표시됩니다.

* 메인 메뉴
* 기본 메뉴에서 액세스한 모든 영역
* 모든 탭
* 모든 메뉴
* Report Builder 및 보고 요소(보기, 필터 및 그룹화)
* 저장 단추
* 내보낸 파일
* 이메일
* 모바일 앱

>[!NOTE]
>
>* Outlook 추가 기능 영역에 사용자 지정된 레이블이 표시되지 않습니다.
>* 레이블을 사용자 지정할 때 문법 및 기타 문제가 발생할 수 있습니다. 예를 들어 &quot;문제&quot;를 &quot;요청&quot;으로 변경하는 경우 UI에 &quot;요청&quot;이라는 구문이 표시되는 위치가 있을 수 있습니다. 자세한 내용은 [개체 이름 사용자 지정에 대한 의미](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) 기사 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 해당 그룹을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 인터페이스 용어 사용자 지정

1. 에 설명된 대로 레이아웃 템플릿 작업을 시작합니다. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 클릭 **용어 설정** 페이지의 오른쪽 위 모서리 근처에 있습니다.
1. 다음 중 하나를 수행합니다.

   * Workfront에서 제공하는 대체 용어를 사용하려면 아래쪽 화살표를 클릭합니다  ![](assets/dropdown-arrow.png) 레이블 옆에 있는 드롭다운 목록에서 원하는 대체 레이블을 클릭합니다.

      >[!NOTE]
      >
      >드롭다운 목록에 제공된 대체 레이블은 비영어 언어용으로 현지화된 Workfront 버전에서 지원됩니다.

   * 객체에 대해 표시되는 레이블에 대해 고유한 사용자 지정 대체 요소를 제공하려면 **사용자 지정 이름 설정** 레이블 오른쪽에 있는 다음 **단일** 및 **복수** 사용자 지정 용어의 형식입니다. 을(를) 클릭합니다 **재설정** 마음을 바꾸시면

      다음 개체 이름을 사용자 지정할 수 있습니다.

      <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront 개체</p></td>
        <td>
          <p>포트폴리오</p>
          <p>프로그램</p>
          <p>프로젝트</p>
          <p>작업</p>
          <p>문제</p>
          <p>목표</p>
          <p>결과</p>
          <p>활동</p>
         </ul></td>
        <td><p>이러한 객체에 대한 자세한 내용은 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront의 개체 이해</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront 목표 개체</p></td>
        <td>
         <ul>
          <p>목표</p>
          <p>결과</p>
          <p>활동</p>
         </ul></td>
        <td><p>이러한 개체에는 추가 라이센스가 필요합니다. 자세한 내용은 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront 목표 개요</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront 시나리오 플래너 객체</p></td>
        <td>
         <ul>
          <p>이니셔티브</p>
          <p>시나리오</p>
          <p>플랜 </p>
         </ul></td>
        <td><p>이러한 개체에는 추가 라이센스가 필요합니다. 자세한 내용은 <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">시나리오 플래너 시작</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. 완료되면 를 클릭합니다 **완료**.

   >[!TIP]
   >
   >완료 를 클릭한 후(그리고 레이아웃 템플릿을 저장한 후에도) 항상 용어 설정 설정으로 돌아가서 사용자 지정 용어 옆에 있는 재설정 을 클릭하여 기본 상태로 돌아갈 수 있습니다.

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 완료한 경우 을 누릅니다 **저장**.

1. 용어 변경 내용을 보려면 다음을 수행하십시오.

   1. Workfront에서 로그아웃한 후 다시 로그인합니다.
   1. Workfront 환경에 대해 열려 있는 모든 브라우저 탭을 닫습니다.

   >[!IMPORTANT]
   >
   >용어를 변경하기 전에 레이아웃 템플릿을 사용한 사용자에게도 필요합니다.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
