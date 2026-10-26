---
title: 사용자 삭제
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 사용자가 조직을 떠나면 Workfront에서 해당 사용자를 제거할 수 있지만 삭제하는 대신 비활성화하는 것이 좋습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 7%
---
# 사용자 삭제

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 Admin Console에 온보딩되지 않은 조직에만 적용됩니다. 조직이 Adobe Admin Console에 온보딩되었으므로 Adobe Admin Console을 통해 이 작업을 수행해야 합니다.
>
>  Adobe Admin Console에서 사용자를 삭제하는 방법에 대한 지침은 [개별적으로 사용자 관리](https://helpx.adobe.com/kr/enterprise/using/manage-users-individually.html) 문서의 &quot;사용자 영구 삭제&quot; 섹션을 참조하거나 Adobe Admin Console 관리자에게 문의하십시오.

사용자가 조직을 떠나면 Adobe Workfront에서 해당 사용자를 제거할 수 있습니다.

사용자 삭제는 Adobe Admin Console을 통해 수행해야 합니다. 자세한 내용은 문서 [개별적으로 사용자 관리](https://helpx.adobe.com/kr/enterprise/using/manage-users-individually.html)의 &quot;사용자를 영구적으로 삭제&quot; 섹션을 참조하거나 Adobe Admin Console 관리자에게 문의하십시오.

>[!IMPORTANT]
>
>시스템에서 사용자를 삭제하면 유지할 사용자와 관련된 정보도 삭제됩니다. 사용자를 삭제하는 대신 비활성화하는 것이 좋습니다. 자세한 내용은 [사용자 비활성화 또는 다시 활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p><p>플랜</p></td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>Adobe Admin Console에서 관리자여야 합니다.</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 삭제 및 비활성화

사용자를 비활성화하면 다음과 같은 일이 발생합니다.

* Workfront Proof 구성 요소가 Workfront 계정과 연결된 경우 Workfront 및 Workfront Proof 모두에 대한 사용자 라이선스를 제거합니다. Workfront Proof에 대한 자세한 내용은 [Workfront Proof: 문서 색인](../../../workfront-proof/workfront-proof.md)을 참조하세요.
* 사용자에게 더 이상 작업을 할당할 수 없습니다.
* 사용자는 더 이상 업데이트에 추가할 수 없습니다.
* 사용자를 더 이상 팀이나 그룹에 추가할 수 없습니다.
* 개체를 더 이상 사용자와 공유할 수 없습니다.
* 다음 개체와의 연관성이 그대로 유지됩니다.

  * 작업, 문제, 프로젝트, 포트폴리오
  * 대시보드

    >[!NOTE]
    >
    >사용자를 비활성화하고 사용자와 연결된 보고서나 대시보드를 더 이상 볼 수 없는 경우 **액세스 권한** 필드로 이 보고서 실행을 업데이트해야 할 수 있습니다.\
    >자세한 내용은 [비활성화된 사용자가 소유한 보고서에 액세스할 수 없는 이유는 무엇입니까?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why)를 참조하십시오. [보고서 FAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 문서의 섹션.

  * 문서
  * 업데이트
  * 시간

* 문서를 체크 아웃한 경우 비활성화하면 문서가 체크 아웃된 상태로 유지됩니다. Workfront 관리자만 다시 체크인할 수 있습니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md)을 참조하십시오.

사용자를 삭제하면 다음과 같은 일이 발생합니다.

* Workfront Proof 구성 요소가 Workfront 계정과 연결된 경우 Workfront 및 Workfront Proof 모두에 대한 사용자 라이선스를 제거합니다. Workfront Proof에 대한 자세한 내용은 [Workfront Proof: 문서 색인](../../../workfront-proof/workfront-proof.md)을 참조하세요.
* 사용자에게 더 이상 작업을 할당할 수 없습니다.
* 사용자는 더 이상 업데이트에 추가할 수 없습니다.
* 사용자를 더 이상 팀이나 그룹에 추가할 수 없습니다.
* 개체를 더 이상 사용자와 공유할 수 없습니다.
* 해당 사용자와 다음 객체의 연관을 삭제합니다.

  * 작업, 문제, 프로젝트, 포트폴리오
  * 대시보드

<!--

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

-->
* 업데이트
* 시간

  >[!NOTE]
  >
  >이러한 오브젝트는 Workfront에 남아 있지만 오브젝트 소유자는 비어 있습니다.

* 사용자가 전역 탐색 막대의 문서 영역 아래에 있는 문서를 업로드한 경우 해당 문서도 삭제됩니다.
* 사용자가 소유한 문서를 체크아웃하고 기본 메뉴에서 액세스할 수 있는 기본 문서 영역에 문서를 업로드하면 문서가 사용자와 함께 삭제됩니다. 문서 체크 아웃에 대한 자세한 내용은 [문서 체크 아웃](../../../documents/managing-documents/check-out-documents.md)을 참조하십시오.

사용자 비활성화에 대한 자세한 내용은 [사용자 비활성화 또는 다시 활성화](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)를 참조하세요.


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
