---
title: 사용자 정의 양식 비활성화 또는 재활성화
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 사용자 정의 양식을 다시 활성화하거나 비활성화할 수 있습니다. 이전 데이터를 유지하는 데 더 이상 사용하지 않는 양식을 삭제하는 것보다 사용자 정의 양식을 비활성화하는 것이 좋습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 사용자 정의 양식 비활성화 또는 재활성화

사용자 정의 양식을 다시 활성화하거나 비활성화할 수 있습니다. 이전 데이터를 유지하는 데 더 이상 사용하지 않는 양식을 삭제하는 것보다 사용자 정의 양식을 비활성화하는 것이 좋습니다.

>[!NOTE]
>
>사용자 정의 양식이 비활성화되었지만 여전히 대기열 주제 또는 요청 대기열 정의에 속하는 경우 새 요청에 첨부됩니다. 요청에서 양식을 사용하지 않으려면 요청 대기열에서 수동으로 제거해야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

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
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p></td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 양식 비활성화

연결된 내역 데이터를 손실하지 않고 더 이상 사용하지 않는 사용자 정의 양식을 비활성화할 수 있습니다. 사용자는 비활성 사용자 정의 양식을 오브젝트에 추가할 수 없지만, 이미 첨부된 오브젝트의 필드에 데이터를 보고 추가할 수 있습니다.

비활성 사용자 정의 양식의 필드도 보기에서 인라인 편집할 수 있습니다. 사용자가 인라인 편집 중에 비활성 사용자 정의 양식의 필드를 추가하면 사용자 정의 양식이 비활성화되더라도 양식이 오브젝트에 자동으로 첨부됩니다.

사용자 정의 양식을 비활성화하려면

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을(를) 선택합니다.
1. **Forms** 영역에서 비활성화할 사용자 정의 양식을 선택합니다.
1. 활성 열에서 **False**&#x200B;를 선택하고 열을 클릭합니다. 양식이 더 이상 활성화되지 않습니다.

## 사용자 정의 양식 다시 활성화

사용자 정의 양식을 다시 활성화하면 이전에 설정했던 대로 유지되며 사용자가 비활성화되지 않은 것처럼 사용자 정의 양식과 상호 작용할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을(를) 선택합니다.
1. **Forms** 영역에서 다시 활성화할 사용자 정의 양식을 선택합니다.
1. 활성 열에서 **True**&#x200B;를 선택하고 열을 클릭합니다. 이제 양식이 활성화됩니다.
