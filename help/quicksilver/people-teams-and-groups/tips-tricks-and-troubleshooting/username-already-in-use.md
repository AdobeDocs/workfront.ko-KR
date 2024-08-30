---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: 사용자 이름이 이미 사용 중입니다.
description: 사용자 이름이 이미 사용 중이라는 오류가 표시되면 이 팁을 참조 하십시오.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 1%

---

# 사용자 이름이 이미 사용 중입니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 질문

새 사용자를 만들 때 사용자 이름을 이미 사용하고 있다는 [!UICONTROL 죄송합니다] 오류가 표시됩니다. 시스템에 이 이메일이 더 이상 발생하지 않습니다. 표시되는 이유는 무엇입니까?

## 솔루션

현재 [!DNL Adobe Workfront] 인스턴스에서 사용자 이름 또는 전자 메일 주소가 고유하지 않기 때문에 이러한 문제가 발생할 수 있습니다. 사용자는 별도의 인스턴스에서 동일한 사용자 이름 또는 이메일 주소를 가질 수 있습니다. 예를 들어 사용자 A는 [!DNL Workfront] 계정과 연결된 usera@company1.com 및 usera@company2.com 전자 메일 주소를 가질 수 있습니다.

>[!NOTE]
>
>기본 [!DNL Workfront] 관리자가 동일한 클러스터의 별도 Workfront 인스턴스에 있는 경우 동일한 사용자 이름 또는 전자 메일 주소를 가질 수 없습니다.
>
>인스턴스가 서로 다른 클러스터에 있는 경우 기본 관리자는 동일한 사용자 이름 또는 이메일 주소를 가질 수 있습니다. [!UICONTROL 설정] > [!UICONTROL 시스템] > [!UICONTROL 고객 정보]에서 인스턴스가 있는 클러스터를 볼 수 있습니다.

### 사용자 이름이 인스턴스에서 고유한지 확인

현재 [!DNL Workfront] 인스턴스에서 사용자 이름 및 전자 메일 주소가 고유한지 확인합니다.

{{step-1-to-users}}

1. 직원 목록에서 **[!UICONTROL 전자 메일]** 열을 확인하여 중복 전자 메일이 없는지 확인하세요.
1. 보기에 사용자 이름에 대한 열을 추가합니다.

   1. **[!UICONTROL 보기]** 드롭다운 메뉴에서 **[!UICONTROL 보기 사용자 지정]**&#x200B;을 클릭합니다.
   1. **[!UICONTROL 열 추가]**&#x200B;를 클릭합니다.
   1. 검색 필드에 *[!UICONTROL 사용자 이름]*&#x200B;을(를) 입력합니다.
   1. **[!UICONTROL 사용자]** > **[!UICONTROL 사용자 이름]**&#x200B;을 선택합니다.
   1. 보기를 저장합니다.\
      그러면 중복을 찾을 수 있는 사용자 이름을 표시하는 보기가 표시됩니다.

1. 사용자 목록에서 **[!UICONTROL 사용자 이름]** 열을 찾아 중복된 사용자 이름이 없는지 확인합니다.
