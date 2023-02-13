---
product-area: programs;projects
navigation-topic: create and manage programs
title: 프로그램에 프로젝트 추가
description: 프로젝트를 포트폴리오 내의 프로그램에 추가하여 구성할 수 있습니다. 하나의 프로그램 내에 여러 개의 프로젝트가 있을 수 있지만 하나의 프로그램만 프로젝트에 연결할 수 있습니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1fecc4d1-4c24-495c-98f5-824e13967369
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# 프로그램에 프로젝트 추가

프로젝트를 포트폴리오 내의 프로그램에 추가하여 구성할 수 있습니다. 하나의 프로그램 내에 여러 개의 프로젝트가 있을 수 있지만 하나의 프로그램만 프로젝트에 연결할 수 있습니다.

프로젝트에 프로젝트를 추가하려면 먼저 이 포트폴리오 내에 포트폴리오와 프로그램을 만들어야 합니다.

포트폴리오 만들기에 대한 내용은 [포트폴리오 만들기](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

프로그램 만들기에 대한 내용은 [프로그램 만들기](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!UICONTROL Team] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로그램 이상에 대한 [!UICONTROL 보기] 액세스</p> <p>프로젝트에 대한 [!UICONTROL Edit] 액세스</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>[!UICONTROL View] 프로그램에 대한 권한</p> <p>프로젝트에 대한 [!UICONTROL Manage] 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 기존 프로그램에 프로젝트 추가

1. 프로그램으로 이동합니다.

   클릭 **[!UICONTROL 프로젝트]** 왼쪽 패널에 표시됩니다.

1. 클릭 **[!UICONTROL 새 프로젝트]** 프로젝트를 추가할 방법을 선택합니다.

   >[!TIP]
   >
   >에서 프로젝트 목록을 볼 때는 프로젝트를 추가할 수 없습니다 [!UICONTROL 이정표] 보기.

   다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 기존 프로젝트]</td> 
      <td> <p>이미 생성된 프로젝트를 추가합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 새 프로젝트]</td> 
      <td> <p>처음부터 새 프로젝트를 추가합니다. </p> <p>처음부터 프로젝트를 만드는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">프로젝트 만들기</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 다음에서 프로젝트 가져오기 [!DNL MS Project]] </td> 
      <td> <p>이전에 내보낸 프로젝트를 추가합니다 [!DNL MS Project] 컴퓨터에 저장했습니다. </p> <p>에서 가져온 새 프로젝트를 만드는 방법에 대한 자세한 내용은 [!DNL Microsoft Project]를 참조하십시오. <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">다음에서 프로젝트 가져오기 [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>작업을 시작하기 전에 새 프로젝트가 승인되도록 요청합니다.</p> <p>프로젝트 요청에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-projects/request-project.md">프로젝트 요청</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 템플릿에서 새로 만들기]</td> 
      <td> <p>기존 템플릿을 사용하여 새 프로젝트를 추가합니다. </p> <p>템플릿에서 프로젝트를 만드는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">템플릿을 사용하여 프로젝트 만들기</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) 선택한 경우 **[!UICONTROL 기존 프로젝트]**&#x200B;를 채울 때 다음을 수행합니다.

   1. 에서 **[!UICONTROL 프로젝트 추가]** 대화 상자에서 제공된 필드에 프로젝트 이름을 입력한 다음 목록에 표시될 때 선택합니다. 한 번에 여러 프로젝트를 추가할 수 있습니다.
   1. 클릭 **[!UICONTROL 프로젝트 추가]**.**&#x200B;**&#x200B;프로젝트&#x200B;이 **[!UICONTROL 프로젝트]** 프로그램의 탭이며 이제 프로그램 및 포트폴리오와 연결됩니다. 
