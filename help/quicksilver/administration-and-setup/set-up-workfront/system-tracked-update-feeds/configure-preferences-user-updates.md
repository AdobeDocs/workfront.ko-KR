---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 사용자 업데이트에 대한 환경 설정 구성
description: 사용자가 개체의 설명을 추가할 때 특정 기능에 액세스하는 환경 설정을 구성할 수 있습니다 [!UICONTROL 업데이트] 영역.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 3%

---

# 사용자 업데이트에 대한 환경 설정 구성

사용자가 개체의 주석을 추가할 때 특정 기능에 액세스할 수 있도록 환경 설정을 구성할 수 있습니다 [!UICONTROL 업데이트] 영역.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 [!UICONTROL 시스템 관리자] 액세스 수준이 필요합니다.</p><p>그룹에 대해 해당 그룹을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자가 업데이트에 이미지를 추가할 수 있도록 허용

기본적으로 사용자는 업데이트에 이미지를 추가할 수 없습니다. 이 기본 설정을 사용하면 사용자는 업데이트에 이미지를 첨부할 수 있습니다. 기본 설정은 [!DNL Workfront] 인스턴스.

>[!NOTE]
>
>* 업데이트에 저장된 이미지는 문서 저장소 제한에 포함됩니다. 자세한 내용은 [문서 저장소 제한 확인](../../../documents/managing-documents/check-document-storage.md).
>* 이미지는 [!UICONTROL 업데이트] 탭에서 사용할 수 없음 [!UICONTROL 문서] 탭.
>




1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.
1. 을(를) 선택합니다 **[!UICONTROL 기본 설정]** 탭.

   ![업데이트 피드에 대한 사용자 환경 설정](assets/updatefeeds-preferences-350x137.png)

1. 을(를) 선택합니다 **[!UICONTROL 사용자가 업데이트에서 이미지를 추가할 수 있도록 허용]** 확인란을 선택합니다.
1. 선택 **[!UICONTROL 저장]**.

   이 기본 설정이 활성화되면 언제든지 비활성화할 수 있습니다. 업데이트에 이미 게시된 모든 이미지는 [!UICONTROL 업데이트] 영역에 표시됩니다.
