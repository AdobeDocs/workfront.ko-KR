---
title: 이전 요청의 데이터를 사용하여 요청 자동 완성
content-type: reference
description: AI를 사용하여 이전 요청의 데이터를 사용하여 요청 필드를 자동으로 완료할 수 있습니다.
author: Becky
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
source-git-commit: 21039f9ab14529b56935d65e0261dc1ce068918c
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 이전 요청의 데이터를 사용하여 요청 자동 완성

AI를 통해 이전 요청을 기반으로 요청 필드를 자동 완성할 수 있습니다. 요청을 제출하기 전에 이러한 제안을 승인하거나 거부할 수 있습니다.

자동 완성은 이미 입력한 필드를 덮어쓰지 않습니다.

사용자는 액세스 권한이 없는 데이터에 대한 제안을 받지 않습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 기여자 이상</p>
   또는
   <p>현재: 요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p>  </td> 
  </tr> 
   <td role="rowheader">개체 권한</td> 
   <td><p>요청 대기열에 요청을 추가하는 액세스 권한</p> <p>기존 요청에 대한 이상의 권한 보기</p> <p>요청 대기열 설정에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a>를 참조하십시오. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 양식 작성 시 제안 받기

자동 완성 기능은 양식을 작성하는 동안 필드 값을 제안할 수 있습니다. 요청 필드에 값을 입력하면 Workfront은 해당 값을 이전 요청과 비교합니다. 입력한 값이 이전 요청의 유사한 컨텍스트에서 다른 필드 값과 밀접하게 연관되어 있으면 Workfront에서 해당 값을 제안합니다.

예를 들어, 클리닉이 항상 동일한 청구 코드를 사용하는 경우 Workfront에서는 클리닉 이름을 입력할 때 해당 필드에 청구 코드가 있다고 제안할 수 있습니다.

이전 요청을 기반으로 제안을 사용하려면 다음을 수행합니다.

1. 요청 만들기를 시작합니다.

   지침은 [요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)을 참조하세요.

1. 필드 채우기를 시작합니다.

   필드를 입력할 때 다른 필드에 제안이 표시될 수 있습니다.

1. 각 필드 제안에 대해 해당 필드에 대해 **수락** 또는 **거부**&#x200B;을 선택합니다.

   ![제안 수락 또는 거부](assets/accept-reject-suggestion.png)

   또는

   모든 제안을 수락하거나 거부하려면 페이지 맨 위에서 **모두 수락** 또는 **모두 거부**&#x200B;를 선택하십시오.

   >[!NOTE]
   >
   >검토되지 않은 제안은 요청을 제출할 때 자동으로 수락됩니다.
