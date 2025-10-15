---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 필터 단추가 페이지 헤더에 표시되지 않음
description: 페이지 헤더에 표시되지 않는 필터 단추 문제를 해결하려면 이 문서를 참조하십시오.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 3%

---

# 필터 단추가 페이지 헤더에 표시되지 않음

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table>
  <tr>
   <td>Adobe Workfront 패키지
   </td>
   <td> <p>Prime 또는 Ultimate</p>
    <p>워크플로 얼티밋</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront 라이선스
   </td>
   <td><p>표준</p>
   <p>플랜</p>
   </td>
  </tr>
   <tr>
   <td>액세스 수준 구성
   </td>
   <td>[!DNL Workfront] 관리자여야 합니다.
   </td>
  </tr>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 문제

다음 필터 단추가 해당 영역에 표시되지 않습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 영역</strong></td> 
   <td><strong>필터 단추</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 프로젝트] </p> </td> 
   <td> 
    <ul> 
     <li> <p>내가 진행 중인 [!UICONTROL 프로젝트]</p> </li> 
     <li> <p>내가 소유한 [!UICONTROL 프로젝트]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL 타임시트]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL 내 타임시트 승인]</span> </p> </li> 
     <li> <p><span>[!UICONTROL 내 타임시트]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

해당 필터가 사용자에게 적용된 레이아웃 템플릿에 포함되어 있지 않으므로 [!UICONTROL 프로젝트 및 타임시트] 영역의 필터 단추가 표시되지 않습니다. [!DNL Workfront] 관리자는 필터를 포함하는 레이아웃 템플릿을 할당해야 합니다.

>[!NOTE]
>
>[!UICONTROL 설정]의 [!UICONTROL 목록 컨트롤] 영역에서 필터를 제거하는 경우가 있습니다. [!DNL Workfront] 관리자는 레이아웃 템플릿에서 사용할 수 있도록 이 영역의 목록에 이를 포함해야 합니다.

1. 레이아웃 템플릿에 다음 필터가 표시되는지 확인합니다.

   * [!UICONTROL 프로젝트] 영역에서 [!UICONTROL 내가 진행 중인 프로젝트] 및 [!UICONTROL 내가 소유한 프로젝트]
   * [!UICONTROL 타임시트] 영역의 [!UICONTROL 내 타임시트 승인] 및 [!UICONTROL 내 타임시트]

   방법은 다음과 같습니다.

   1. 레이아웃 템플릿에 액세스합니다.
   1. **[!UICONTROL 사용자에게 표시되는 항목 사용자 지정]**&#x200B;에서 **[!UICONTROL 목록]**&#x200B;을 선택합니다.
   1. **[!UICONTROL 사용자 지정할 목록 선택]**&#x200B;에서 **[!UICONTROL 프로젝트]** 또는 **[!UICONTROL 타임시트]**&#x200B;를 선택합니다.
   1. **[!UICONTROL 필터]** 섹션에서 **[!UICONTROL 내가 진행 중인 프로젝트]**, **[!UICONTROL 내가 소유한 프로젝트]**(프로젝트용) 및 **[!UICONTROL 내 타임시트 승인]** 및 **[!UICONTROL 내 타임시트]**(타임시트용)가 선택되었는지 확인하십시오.
   1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

1. 올바른 사용자, 작업 역할, 팀 또는 그룹에 레이아웃 템플릿을 할당합니다. 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.
