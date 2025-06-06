---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 프로젝트에 Outlook 이메일을 작업 또는 문제로 추가
description: 전자 메일을  [!DNL Adobe Workfront] 작업 또는 문제로 변환할 수 있습니다. 이메일이 전환되면 전환할 때 선택한 프로젝트에 작업 또는 문제가 표시됩니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# 프로젝트에 [!DNL Outlook] 이메일을 작업 또는 문제로 추가

>[!IMPORTANT]
>
>[Microsoft에서 기존 Exchange 온라인 토큰에 대한 지원을 사용하지 않도록 설정하는 중입니다](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens). 이 토큰은 현재 인증을 위해 Workfront Outlook 추가 기능에서 사용됩니다. Microsoft의 이러한 변경 사항은 이미 고객에게 영향을 주기 시작했으며 2025년 10월까지 단계적으로 계속 적용될 예정입니다.
>
>* **Microsoft에서 이 토큰을 완전히 비활성화하면 Microsoft Outlook용 Workfront 통합이 더 이상 작동하지 않습니다.**
>
>이 변경의 일부로 Microsoft은 토큰이 다시 활성화되는 방식을 변경하기로 결정했습니다. **2025년 6월 30일** 이후에는 관리자가 더 이상 토큰을 직접 다시 활성화할 수 없습니다. Microsoft 지원에서만 예외를 허용할 수 있습니다. **2025년 10월 1일부터 모든 테넌트에 대해 레거시 토큰이 꺼집니다. 예외가 부여되지 않습니다.**


이메일을 [!DNL Adobe Workfront]개의 작업 또는 문제로 변환할 수 있습니다. 이메일이 전환되면 전환할 때 선택한 프로젝트에 작업 또는 문제가 표시됩니다.

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

## 프로젝트에 [!DNL Outlook] 전자 메일을 작업 또는 문제로 추가

1. [!DNL Outlook] 내에서 작업 또는 문제로 변환할 전자 메일을 선택하십시오.
1. 이메일 메시지의 오른쪽 상단에 있는 **[!DNL Workfront]** 아이콘을 클릭하여 Workfront 추가 기능을 표시합니다.

   [!DNL Workfront] 아이콘에 액세스하려면 전자 메일의 오른쪽 위에 있는 아래쪽 방향 화살표를 클릭해야 할 수 있습니다.

1. **[!UICONTROL Menu]** 아이콘 ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png)을(를) 클릭하여 사용 가능한 [!DNL Workfront] 옵션 목록을 표시합니다.



1. **[!UICONTROL 작업에 추가]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 프로젝트에 추가]** 필드를 선택합니다.
1. **[!UICONTROL 프로젝트]** 필드에 프로젝트 이름을 입력한 다음 목록에 나타나면 선택하십시오.
1. 선택한 프로젝트에 작업을 추가하려면 **[!UICONTROL 작업]** 라디오 단추를 선택하십시오.

   또는

   선택한 프로젝트에 문제를 추가하려면 **[!UICONTROL 문제]** 라디오 단추를 선택하십시오.

1. (선택 사항) **[!UICONTROL 할당 대상]** 필드에서 이 작업 또는 문제를 할당할 사용자를 지정합니다.

   >[!TIP]
   >
   >여러 사람이 알 수 있도록 하려면 작업 또는 문제를 팀에 할당할 수 있습니다. 팀원이 이메일 알림을 활성화한 경우 팀원에게 할당된 새 작업 또는 문제에 대한 이메일을 받게 됩니다.


1. (선택 사항) **[!UICONTROL 기한]**&#x200B;을(를) 지정합니다. 작업 또는 문제의 [!UICONTROL 계획된 완료 일자]가 됩니다.
1. (선택 사항) 작업 또는 문제로 저장되기 전에 이메일에서 다음 정보를 업데이트합니다 (필수 필드는 별표로 표시됨).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL 작업 또는 문제 이름]</td>
        <td>기본적으로 작업 이름은 이메일 제목과 같습니다. 원하는 대로 작업 이름을 수정할 수 있습니다.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL 설명]</td>
        <td>기본적으로 설명은 이메일 본문과 동일합니다. 원하는 대로 설명을 수정할 수 있습니다.</td>
      </tr>
      <tr>
        <td>[!UICONTROL 첨부 파일]</td>
        <td>모든 전자 메일 첨부 파일은 작업 또는 문제의 [!UICONTROL 문서] 영역에 저장됩니다. 이메일을 작업 또는 문제로 저장하기 전에 첨부 파일을 삭제할 수 있습니다.</td>
      </tr>
   </table>

1. **[!UICONTROL 추가]**&#x200B;를 클릭합니다.

   작업 또는 문제가 지정된 프로젝트에 추가됨

1. (선택 사항) [!DNL Workfront]&#x200B;**의**&#x200B;보기를 클릭하여 [!DNL Workfront] 응용 프로그램 내의 작업을 새 탭에 표시합니다.

1. (선택 사항) [!DNL Outlook]&#x200B;(으)로 돌아가서 변환된 전자 메일을 선택합니다.

   [!DNL Workfront] 추가 기능 패널의 맨 위에서 [!DNL Workfront]에 작업 또는 문제로 이메일이 추가되었다는 링크가 있는 확인을 확인합니다. 링크에는 전환된 날짜가 포함됩니다.



