---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Outlook 전자 메일에서  [!DNL Adobe Workfront] 요청 만들기
description: Outlook에서 전자 메일에서  [!DNL Adobe Workfront] 요청을 만들 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# [!UICONTROL Outlook] 전자 메일에서 [!DNL Adobe Workfront] 요청 만들기

>[!IMPORTANT]
>
>[Microsoft에서 기존 Exchange 온라인 토큰에 대한 지원을 사용하지 않도록 설정하는 중입니다](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens). 이 토큰은 현재 인증을 위해 Workfront Outlook 추가 기능에서 사용됩니다. Microsoft의 이러한 변경 사항은 이미 고객에게 영향을 주기 시작했으며 2025년 10월까지 단계적으로 계속 적용될 예정입니다.
>
>* **Microsoft에서 이 토큰을 완전히 비활성화하면 Microsoft Outlook용 Workfront 통합이 더 이상 작동하지 않습니다.**
>
>이 변경의 일부로 Microsoft은 토큰이 다시 활성화되는 방식을 변경하기로 결정했습니다. **2025년 6월 30일** 이후에는 관리자가 더 이상 토큰을 직접 다시 활성화할 수 없습니다. Microsoft 지원에서만 예외를 허용할 수 있습니다. **2025년 10월 1일부터 모든 테넌트에 대해 레거시 토큰이 꺼집니다. 예외가 부여되지 않습니다.**


Outlook의 전자 메일에서 [!DNL Adobe Workfront] 요청을 만들 수 있습니다.

전자 메일을 기반으로 [!DNL Workfront] 요청을 만들 때 기본적으로 전자 메일의 콘텐츠(제목 및 본문 포함)가 요청에 포함됩니다.

>[!NOTE]
>
>공유 [!UICONTROL Outlook] 사서함에서 [!DNL Workfront] 요청을 만들 수 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 전제 조건

이 통합을 사용하려면 [!DNL Workfront] 관리자가 [!DNL Workfront]에서 [!DNL Outlook for Office]을(를) 사용하도록 설정해야 합니다.

## [!DNL Outlook] 이메일에서 요청 만들기

[!DNL Outlook]에서 [!DNL Workfront] 요청을 만들려면:

1. [!DNL Workfront] 요청에 포함할 정보가 포함된 이메일을 선택하십시오.
1. 이메일 메시지의 오른쪽 상단에 있는 **[!DNL Workfront]** 아이콘을 클릭하여 Workfront 추가 기능을 표시합니다.\
   [!DNL Workfront] 아이콘에 액세스하려면 전자 메일의 오른쪽 위에 있는 아래쪽 방향 화살표를 클릭해야 할 수 있습니다.

1. **[!UICONTROL 메뉴]** 아이콘 ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png)을(를) 클릭하여 사용 가능한 [!DNL Workfront] 옵션 목록을 표시합니다.

1. **[!UICONTROL 요청 제출]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 요청 유형 선택]** 필드에서 요청을 제출할 요청 대기열을 선택합니다.

1. 다음 정보를 지정합니다.\
   요청 대기열이 설정된 방법에 따라 사용 가능한 필드가 달라질 수 있습니다. 가능한 필드에 대한 전체 목록 및 설명은 [만들기 및 제출 [!DNL Adobe Workfront] 요청](../../manage-work/requests/create-requests/create-submit-requests.md) 문서를 참조하십시오.

   * **[!UICONTROL 제목]:** 요청에 대한 제목을 지정합니다. 기본적으로 이메일 제목이 사용됩니다.
   * **[!UICONTROL 설명]:** 요청에 대한 설명을 지정합니다. 기본적으로 이메일 본문이 사용됩니다.
   * **[!UICONTROL 문서]:** 요청에 포함할 모든 문서를 첨부합니다. 끌어서 놓거나 **[!UICONTROL 파일 선택]**&#x200B;을 클릭하고 문서를 찾아 선택하여 문서를 첨부할 수 있습니다.\

     기본적으로 이메일에 첨부된 모든 문서는 요청에 포함됩니다.

1. **[!UICONTROL 요청 제출]**&#x200B;을 클릭합니다.\
   지정된 요청 큐의 [!DNL Workfront]에 요청이 제출되었습니다.

1. (선택 사항) [!DNL Outlook]&#x200B;(으)로 돌아가서 원본 전자 메일을 선택합니다.\
   [!DNL Workfront] 추가 기능 패널의 맨 위에서 요청으로 이메일이 Workfront에 추가되었다는 링크가 있는 확인을 확인합니다. 링크에는 전환된 날짜가 포함됩니다.\
