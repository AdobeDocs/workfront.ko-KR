---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 필터 단추가 페이지 헤더에 표시되지 않습니다
description: 페이지 헤더에 표시되지 않는 필터 단추를 해결하려면 이 문서를 참조하십시오.
feature: Get Started with Workfront
author: Lisa and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# 필터 단추가 페이지 헤더에 표시되지 않습니다

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 라이선스</strong></td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>[!UICONTROL System 관리자]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 문제

다음 필터 단추는 해당 영역에 표시되지 않습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 영역</strong></td> 
   <td><strong>필터 단추</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL 프로젝트 설정]</p> </li> 
     <li> <p>[!UICONTROL Projects I Own]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL 작업표]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL 내 작업표 승인]</span> </p> </li> 
     <li> <p><span>[!UICONTROL 내 작업표]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

의 필터 단추 [!UICONTROL 프로젝트 및 작업표] 해당 필터가 사용자에게 적용된 레이아웃 템플릿에 포함되지 않으므로 영역이 표시되지 않습니다. 다음 [!DNL Workfront] 관리자는 필터가 포함된 레이아웃 템플릿을 할당해야 합니다.

>[!NOTE]
>
>경우에 따라 필터가 [!UICONTROL 목록 컨트롤] 영역 [!UICONTROL 설정]. 다음 [!DNL Workfront] 레이아웃 템플릿에서 이러한 템플릿을 사용할 수 있도록 하려면 관리자가 이 영역의 목록에 이 필드를 포함해야 합니다.

1. 레이아웃 템플릿에 다음 필터가 표시되는지 확인합니다.

   * [!UICONTROL 프로젝트 설정] 및 [!UICONTROL 프로젝트 소유] 에서 [!UICONTROL 프로젝트] 영역
   * [!UICONTROL 내 작업표 승인] 및 [!UICONTROL 내 작업표] 에서 [!UICONTROL 작업표] 영역

   방법은 다음과 같습니다.

   1. 레이아웃 템플릿에 액세스합니다.
   1. 선택 **[!UICONTROL 목록]** 아래에 **[!UICONTROL 사용자에게 표시되는 항목 사용자 지정]**.
   1. 선택 **[!UICONTROL 프로젝트]** 또는 **[!UICONTROL 작업표]** 아래에 **[!UICONTROL 사용자 지정할 목록 선택]**.
   1. 에서 **[!UICONTROL 필터]** 섹션, **[!UICONTROL 프로젝트 설정]**, **[!UICONTROL 프로젝트 소유]** (프로젝트) 및 **[!UICONTROL 내 작업표 승인]** 및 **[!UICONTROL 내 작업표]** (작업표의 경우)를 선택합니다.
   1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. 레이아웃 템플릿을 올바른 사용자, 작업 역할, 팀 또는 그룹에 할당합니다. 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
