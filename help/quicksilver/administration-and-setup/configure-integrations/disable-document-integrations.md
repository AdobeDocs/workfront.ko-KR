---
title: 문서 통합 사용 안 함
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 로서의 [!DNL anAdobe] [!DNL Workfront] 관리자는 Workfront과 타사 문서 공급자 간의 연결을 비활성화할 수 있습니다.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---

# 문서 통합 사용 안 함

로서의 [!DNL Adobe] [!DNL Workfront] 관리자는 [!DNL Workfront] 및 타사 문서 공급자

다음 사이의 연결을 비활성화하는 경우 [!DNL Workfront] 문서 공급자 및 문서에 대한 링크가 [!DNL Workfront]. 사용자는 연결된 문서를 더 이상 볼 수 없으며 [!DNL Workfront] 링크이며 해당 공급자에 문서를 더 추가할 수 없습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 클라우드 공급자 통합 비활성화

에 대한 문서 통합을 비활성화하려면 [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. 에 로그인합니다. [!DNL Workfront] 로서의 [!DNL Workfront] 관리자
1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 문서]** > **[!UICONTROL 클라우드 공급자]**.

1. 연결을 끊으려는 클라우드 공급자 중 하나를 선택 취소합니다 [!DNL Workfront].
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   사용자가 비활성화한 특정 클라우드 공급자에 연결할 수 없으며, 해당 클라우드 공급자의 문서를 더 이상 Workfront에 연결할 수 없습니다.

## 비활성화 [!DNL SharePoint] 통합

1. 에 로그인합니다. [!DNL Workfront] 로서의 [!DNL Workfront] 관리자
1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 확장 **[!UICONTROL 문서]**&#x200B;를 클릭한 다음 **[!UICONTROL [!DNL SharePoint]통합]**.
1. 을(를) 선택합니다 [!DNL SharePoint] 비활성화할 통합입니다.
1. 클릭 **[!UICONTROL 비활성화]**.\
   사용자가 [!DNL SharePoint] 사이트를 비활성화하여 더 이상 [!DNL SharePoint] to [!DNL Workfront].

## 사용자 지정 통합 비활성화

1. 에 로그인합니다. [!DNL Workfront] 관리자로.
1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 문서]** > **[!UICONTROL 사용자 지정 통합]**.
1. 비활성화할 사용자 지정 통합을 선택합니다.
1. 클릭 **[!UICONTROL 비활성화]**.

   사용자가 비활성화한 타사 문서 공급자에 연결할 수 없으며 해당 클라우드 공급자의 문서를 [!DNL Workfront].
