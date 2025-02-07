---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 사용자 업데이트에 대한 환경 설정 구성
description: 사용자가 개체의 [!UICONTROL 업데이트] 영역에 댓글을 추가할 때 특정 기능에 액세스하는 환경 설정을 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 3%

---

# 사용자 업데이트에 대한 환경 설정 구성

개체의 [!UICONTROL 업데이트] 영역에 주석을 추가할 때 사용자에게 특정 기능에 대한 액세스 권한을 제공하는 환경 설정을 구성할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td><p>시스템 수준에서 이러한 단계를 수행하려면 [!UICONTROL 시스템 관리자] 액세스 수준이 필요합니다.</p><p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p></td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자가 업데이트에 이미지를 추가할 수 있도록 허용

기본적으로 사용자는 업데이트에 이미지를 추가할 수 없습니다. 이 환경 설정을 사용하면 사용자가 업데이트에 이미지를 첨부할 수 있습니다. 환경 설정은 [!DNL Workfront] 인스턴스의 모든 영역에 있는 모든 업데이트에 적용됩니다.

>[!NOTE]
>
>* 업데이트에 저장된 이미지는 문서 저장 용량 한도에 포함됩니다. 자세한 내용은 [문서 저장소 제한 확인](../../../documents/managing-documents/check-document-storage.md)을 참조하세요.
>* 이미지는 개체의 [!UICONTROL 업데이트] 탭을 통해 액세스할 수 있으며 [!UICONTROL 기본 메뉴]의 [!UICONTROL 문서] 영역에서도 사용할 수 있습니다.
>

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![톱니바퀴 설정 아이콘](assets/gear-icon-settings.png)을 클릭합니다.
1. 왼쪽 패널에서 **[!UICONTROL 인터페이스]** > **[!UICONTROL 피드 업데이트]**&#x200B;를 선택합니다.
1. **[!UICONTROL 환경 설정]** 탭을 선택합니다.

   ![업데이트 피드에 대한 사용자 환경 설정](assets/updatefeeds-preferences-350x137.png)

1. **[!UICONTROL 사용자가 업데이트에 이미지를 추가하도록 허용]** 확인란을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

   이 환경 설정을 활성화하면 언제든지 비활성화할 수 있습니다. 업데이트에 이미 게시된 모든 이미지는 개체의 [!UICONTROL 업데이트] 영역에 남아 있습니다.
