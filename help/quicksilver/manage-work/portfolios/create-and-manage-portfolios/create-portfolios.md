---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 포트폴리오 만들기
description: Portfolio은 동일한 리소스, 예산 및 일정에 대해 경쟁하는 프로젝트 모음입니다. Portfolio의 프로젝트는 동일한 리소스 풀을 사용하고 동일한 스코어카드에 대해 측정할 만큼 충분히 유사합니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# 포트폴리오 만들기

Portfolio은 동일한 리소스, 예산 및 일정에 대해 경쟁하는 프로젝트 모음입니다. Portfolio의 프로젝트는 동일한 리소스 풀을 사용하고 동일한 스코어카드에 대해 측정할 만큼 충분히 유사합니다.

Portfolio을 사용하여 동일한 제품 라인, 사업부, 부서, 회사 또는 기타 업무 단위에 속하는 프로젝트를 그룹화할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Business] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>[!UICONTROL Edit] Portfolio 액세스</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>포트폴리오를 만들면 기본적으로 포트폴리오에 대한 관리 권한이 있습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 포트폴리오 만들기

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **[!UICONTROL Portfolio]**.
1. 클릭 **[!UICONTROL 새 Portfolio]**.
1. 바꾸기 **[!UICONTROL 제목 없는 Portfolio]** 포트폴리오에 사용할 이름으로 지정합니다.

   이름은 최대 255자를 포함할 수 있습니다.

1. (선택 사항) 아래의 이름을 클릭합니다 **[!UICONTROL Portfolio 관리자]** 페이지 상단의 헤더에서 포트폴리오의 다른 관리자를 할당합니다.

   ![](assets/portfolio-manager-name-350x51.jpg)

   포트폴리오 작성자는 기본적으로 포트폴리오 관리자로 지정됩니다.

1. 클릭 **[!UICONTROL Portfolio 세부 사항]** 왼쪽 패널에 표시됩니다.
1. 에서 **[!UICONTROL 개요]** 영역, 다음 정보 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Portfolio에 대한 설명을 입력하여 고유한 사항을 나타냅니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio 관리자]</td> 
      <td> <p>포트폴리오 관리자로 나타낼 사용자 이름을 입력하고 목록에 표시될 때 선택합니다. [!UICONTROL Portfolio 소유자]와 동일합니다. 포트폴리오 프로젝트에 정의된 작업을 감독하고 비즈니스 사례를 승인할 수 있는 사람입니다.</p> <p>중요 사항: 사용자를 [!UICONTROL Portfolio 관리자]로 지정하면 포트폴리오의 포트폴리오, 프로그램 및 프로젝트에 대한 [!UICONTROL 관리] 권한을 자동으로 가져옵니다. </p> <p>팁: 페이지 맨 위의 헤더에서 [!UICONTROL Portfolio 관리자]를 업데이트할 수도 있습니다.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">그룹 </td> 
      <td> <p>그룹이 포트폴리오를 소유하거나 이를 완료할 책임이 있는 경우 단일 그룹의 이름을 추가합니다. </p> <p>마우스로 가리키고 [!UICONTROL 정보] 아이콘을 클릭하여 올바른 그룹을 선택할 수 있습니다 <img src="assets/info-icon.png"> 옆에 표시됩니다. 그룹 위에 있는 그룹 계층 및 해당 관리자와 같은 그룹에 대한 정보를 나열하는 도구 설명이 표시됩니다.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) **[!UICONTROL 사용자 지정 양식 추가]** 오른쪽 위 모서리의 상자 [!UICONTROL Portfolio 세부 사항] 페이지를 클릭하여 포트폴리오의 사용자 지정 양식을 선택하고 사용자 지정 필드를 업데이트합니다.

   >[!TIP]
   >
   >포트폴리오 사용자 정의 양식을 포트폴리오에 첨부하려면 먼저 이미 만든 포트폴리오 사용자 정의 양식이 있어야 합니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.
1. (선택 사항) **[!UICONTROL 프로그램]** 왼쪽 패널에서 **[!UICONTROL 프로그램 추가]** 포트폴리오에 프로그램을 추가하려면

   프로그램 만들기에 대한 자세한 내용은 [프로그램 만들기](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (선택 사항) **[!UICONTROL 프로젝트]** 왼쪽 패널에서 **[!UICONTROL 프로젝트 추가]** 프로젝트에 프로젝트를 추가하려면 다음을 수행하십시오.

   Portfolio에 프로젝트 추가에 대한 자세한 내용은 [포트폴리오에 프로젝트 추가](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
