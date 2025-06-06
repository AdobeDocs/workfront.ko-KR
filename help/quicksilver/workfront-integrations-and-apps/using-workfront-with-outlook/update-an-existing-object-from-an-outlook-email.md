---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Outlook 이메일에서 기존 개체 업데이트
description: Outlook 전자 메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# [!DNL Outlook] 이메일에서 기존 개체 업데이트

>[!IMPORTANT]
>
>[Microsoft에서 기존 Exchange 온라인 토큰에 대한 지원을 사용하지 않도록 설정하는 중입니다](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens). 이 토큰은 현재 인증을 위해 Workfront Outlook 추가 기능에서 사용됩니다. Microsoft의 이러한 변경 사항은 이미 고객에게 영향을 주기 시작했으며 2025년 10월까지 단계적으로 계속 적용될 예정입니다.
>
>* **Microsoft에서 이 토큰을 완전히 비활성화하면 Microsoft Outlook용 Workfront 통합이 더 이상 작동하지 않습니다.**
>
>이 변경의 일부로 Microsoft은 토큰이 다시 활성화되는 방식을 변경하기로 결정했습니다. **2025년 6월 30일** 이후에는 관리자가 더 이상 토큰을 직접 다시 활성화할 수 없습니다. Microsoft 지원에서만 예외를 허용할 수 있습니다. **2025년 10월 1일부터 모든 테넌트에 대해 레거시 토큰이 꺼집니다. 예외가 부여되지 않습니다.**

[!DNL Outlook] 전자 메일의 정보로 기존 프로젝트, 작업 또는 문제를 업데이트할 수 있습니다.


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

## [!DNL Outlook] 이메일에서 기존 개체 업데이트

1. [!DNL Outlook]에서 [!DNL Adobe Workfront update]에 포함할 정보가 포함된 전자 메일을 선택합니다.
1. 이메일 메시지의 오른쪽 상단에 있는 **[!DNL Workfront]** 아이콘을 클릭하여 Workfront 추가 기능을 표시합니다.\
   [!DNL Workfront] 아이콘에 액세스하려면 전자 메일의 오른쪽 위에 있는 아래쪽 방향 화살표를 클릭해야 할 수 있습니다.

1. **[!UICONTROL Menu]** 아이콘 ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png)을(를) 클릭하여 사용 가능한 [!DNL Workfront] 옵션 목록을 표시합니다.\


1. Workfront에서 **[!UICONTROL 업데이트]**&#x200B;를 클릭합니다.\
   작업으로 저장되기 전에 이메일에서 다음 정보를 업데이트할 수 있습니다.

   * **[!UICONTROL 유형]**: 업데이트할 개체의 유형을 선택하십시오. **[!UICONTROL 프로젝트]**, **[!UICONTROL 작업]** 또는 **[!UICONTROL 문제]**&#x200B;를 선택할 수 있습니다. 선택한 개체는 아래 **[!UICONTROL 이름]** 필드에 표시되는 결과를 결정합니다. 개체 유형을 잘 모를 경우 **[!UICONTROL 모두]**&#x200B;를 선택하여 프로젝트, 작업 및 문제를 동시에 검색하십시오.

   * **[!UICONTROL 이름]**: 업데이트할 프로젝트, 작업 또는 문제의 이름을 입력하세요. 드롭다운 목록에 표시될 때 이름을 클릭합니다.
   * **[!UICONTROL 업데이트]**: 기본적으로 업데이트는 전자 메일 본문과 동일합니다. 원하는 대로 업데이트를 수정할 수 있습니다.\

     이 [!UICONTROL 업데이트]는 Workfront의 업데이트 상태로 표시됩니다.

   * **[!UICONTROL 첨부 파일]**: 전자 메일 첨부 파일은 작업의 [!UICONTROL 문서] 영역에 저장됩니다. 업데이트를 제출하기 전에 첨부 파일을 삭제할 수 있습니다.

1. (선택 사항) **[!UICONTROL 다른 사용자 포함]**&#x200B;을 클릭하고 업데이트에 포함할 사용자 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.\
   이 프로세스를 반복하여 추가 사용자를 포함한 다음 **[!UICONTROL 완료]**&#x200B;를 클릭합니다.\
   기본적으로 회신하려는 사용자는 포함 여부에 관계없이 알림을 받습니다.\

1. (선택 사항) 이 업데이트를 회사 내의 사용자로 제한하려면 **[!UICONTROL 잠금]** 아이콘을 클릭합니다. 업데이트가 잠기면 회사 외부의 사용자가 업데이트를 볼 수 없습니다.

   * **[!UICONTROL 잠금 해제됨]:** 업데이트가 있는 프로젝트, 작업 또는 문제에 대한 액세스 권한이 있는 모든 사용자가 업데이트를 볼 수 있습니다.\

     기본적으로 업데이트는 잠금 해제되어 있습니다.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL 잠김]:** 회사 내의 사용자만 업데이트를 볼 수 있습니다.\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. **[!UICONTROL 업데이트]**&#x200B;를 클릭합니다.
1. (선택 사항) [!UICONTROL Outlook] 내에서 [!DNL Workfront] 통합으로 업데이트된 항목을 보려면 **[!UICONTROL Workfront에서 보기]**&#x200B;를 클릭합니다.
