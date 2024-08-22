---
title: 문서 통합 비활성화
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: ' [!DNL anAdobe] [!DNL Workfront] 관리자는 Workfront과 서드파티 문서 공급자 간의 연결을 비활성화할 수 있습니다.'
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 1%

---

# 문서 통합 비활성화

[!DNL Adobe] [!DNL Workfront] 관리자는 [!DNL Workfront]과(와) 서드파티 문서 공급자 간의 연결을 비활성화할 수 있습니다.

[!DNL Workfront]과(와) 문서 공급자 간의 연결을 사용하지 않도록 설정하면 문서에 대한 링크가 [!DNL Workfront]에서 사라집니다. 사용자는 연결된 문서를 더 이상 볼 수 없고 [!DNL Workfront] 링크를 통해 문서를 변경할 수 없으며 해당 공급자에 더 많은 문서를 추가할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다. [!DNL Workfront] 관리자에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

+++

## 클라우드 공급자 통합 비활성화

[!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]에 대한 문서 통합을 비활성화하려면:

1. [!DNL Workfront]에 [!DNL Workfront] 관리자로 로그인합니다.

{{step-1-to-setup}}

1. **[!UICONTROL 문서]** > **[!UICONTROL 클라우드 공급자]**&#x200B;를 클릭합니다.

1. [!DNL Workfront]에서 연결을 끊을 클라우드 공급자의 선택을 취소하십시오.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   사용자는 비활성화한 특정 클라우드 공급자에 연결할 수 없으며 더 이상 해당 클라우드 공급자의 문서를 Workfront에 연결할 수 없습니다.

## [!DNL SharePoint] 통합 사용 안 함

1. [!DNL Workfront]에 [!DNL Workfront] 관리자로 로그인합니다.

{{step-1-to-setup}}

1. **[!UICONTROL 문서]**&#x200B;를 확장한 다음 **[!UICONTROL [!DNL SharePoint]통합]**&#x200B;을 클릭합니다.
1. 비활성화할 [!DNL SharePoint] 통합을 선택하십시오.
1. **[!UICONTROL 사용 안 함]**&#x200B;을 클릭합니다.\
   사용자가 사용하지 않도록 설정한 [!DNL SharePoint] 사이트에 연결할 수 없으며 [!DNL SharePoint]에서 [!DNL Workfront](으)로 문서를 더 이상 연결할 수 없습니다.

## 사용자 정의 통합 비활성화

1. [!DNL Workfront]에 관리자로 로그인합니다.

{{step-1-to-setup}}

1. **[!UICONTROL 문서]** > **[!UICONTROL 사용자 지정 통합]**&#x200B;을 클릭합니다.
1. 비활성화하려는 사용자 정의 통합을 선택합니다.
1. **[!UICONTROL 사용 안 함]**&#x200B;을 클릭합니다.

   사용자가 사용하지 않도록 설정한 서드파티 문서 공급자에 연결할 수 없으며 해당 클라우드 공급자의 문서를 [!DNL Workfront]에 더 이상 연결할 수 없습니다.
