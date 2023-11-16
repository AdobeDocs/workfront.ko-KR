---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 사용자 업데이트에 대한 환경 설정 구성
description: 사용자가 오브젝트의 주석을 추가할 때 특정 기능에 액세스하는 기본 설정을 구성할 수 있습니다 [!UICONTROL 업데이트] 영역입니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 3%

---

# 사용자 업데이트에 대한 환경 설정 구성

오브젝트의 주석을 추가할 때 사용자에게 특정 기능에 대한 액세스 권한을 부여하는 기본 설정을 구성할 수 있습니다 [!UICONTROL 업데이트] 영역입니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 [!UICONTROL 시스템 관리자] 액세스 수준이 필요합니다.</p><p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자가 업데이트에 이미지를 추가할 수 있도록 허용

기본적으로 사용자는 업데이트에 이미지를 추가할 수 없습니다. 이 환경 설정을 사용하면 사용자가 업데이트에 이미지를 첨부할 수 있습니다. 환경 설정은 의 모든 영역에 있는 모든 업데이트에 적용됩니다. [!DNL Workfront] 인스턴스.

>[!NOTE]
>
>* 업데이트에 저장된 이미지는 문서 저장 용량 한도에 포함됩니다. 자세한 내용은 [문서 저장 공간 제한 확인](../../../documents/managing-documents/check-document-storage.md).
>* 이미지를 통해 액세스할 수 있습니다. [!UICONTROL 업데이트] 개체에서 사용할 수 있는 탭입니다. [!UICONTROL 문서] 아래 영역 [!UICONTROL 메인 메뉴].
>

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**.
1. 다음 항목 선택 **[!UICONTROL 환경 설정]** 탭.

   ![업데이트 피드에 대한 사용자 환경 설정](assets/updatefeeds-preferences-350x137.png)

1. 다음 항목 선택 **[!UICONTROL 사용자가 업데이트에 이미지를 추가하도록 허용]** 확인란.
1. 선택 **[!UICONTROL 저장]**.

   이 환경 설정을 활성화하면 언제든지 비활성화할 수 있습니다. 업데이트에 이미 게시된 모든 이미지는 [!UICONTROL 업데이트] 개체의 영역입니다.
