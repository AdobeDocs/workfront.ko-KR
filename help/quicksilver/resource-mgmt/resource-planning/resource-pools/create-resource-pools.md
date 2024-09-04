---
product-area: resource-management
navigation-topic: resource-pools
title: 리소스 풀 만들기
description: 리소스 풀은 Adobe Workfront에서 리소스를 보다 쉽게 관리하는 데 도움이 되는 사용자 컬렉션입니다.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 2%

---

# 리소스 풀 만들기

{{preview-and-fast-release-Q424}}

리소스 풀은 Adobe Workfront에서 리소스를 보다 쉽게 관리하는 데 도움이 되는 사용자 컬렉션입니다. 리소스 풀에 대한 자세한 내용은 [리소스 풀 개요](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td><p>새로 만들기: 모두</p>
       <p>또는</p>
       <p>현재: Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>리소스 풀 관리에 대한 액세스 권한을 포함하는 리소스 관리에 대한 액세스 편집</p> <p>프로젝트, 템플릿 및 사용자에 대한 액세스 편집</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td>리소스 풀을 연결할 프로젝트, 템플릿 및 사용자에 대한 권한을 관리합니다.</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 리소스 풀 만들기 {#create-a-resource-pool}

{{step1-to-resourcing}}

1. 왼쪽 패널에서 **리소스 풀**&#x200B;을 클릭합니다.

   <span class="preview">미리 보기 환경의 샘플 이미지:</span>
   <span class="preview">![리소스 풀](assets/list-of-resource-pools.png)</span>

   프로덕션 환경의 샘플 이미지:
   ![리소스 풀](assets/resource-pools-tab-350x198.png)

1. **새 리소스 풀**&#x200B;을 클릭합니다.
1. 다음을 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>이름</strong></td>
      <td>리소스 풀의 이름입니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>설명</strong></td>
      <td>이 리소스 풀에 대한 간략한 설명입니다. 예를 들어 사용해야 하는 용도를 지정할 수 있습니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>풀 멤버</strong></td>
      <td><p> 리소스 풀에 개별적으로 사용자를 추가합니다.<br>또는 <br>한 번에 많은 사용자를 리소스 풀에 추가합니다. 사용자 또는 사용자 컬렉션과 연결된 다음 엔티티 중 하나를 추가할 수 있습니다.
        <ul>
         <li><strong>팀</strong>: 팀의 모든 구성원이 리소스 풀에 추가됩니다.</li>
         <li><strong>그룹</strong>: 그룹의 모든 구성원이 리소스 풀에 추가됩니다.</li>
         <li><strong>역할</strong>: 해당 역할과 연결된 모든 사용자가 리소스 풀에 추가됩니다.</li>
         <li><strong>회사</strong>: 회사의 모든 사용자가 리소스 풀에 추가됩니다.</li>
        </ul><p>팁: 활성 사용자, 팀, <span>역할,</span> 또는 회사만 추가할 수 있습니다.</p><br>리소스 풀의 모든 사용자를 보려면 대화 상자에서 아래로 스크롤해야 할 수 있습니다.
        <p>참고: 그룹, 팀, 회사의 구성원이 되거나 그룹, 팀, 회사 또는 작업 역할이 리소스 풀에 추가된 후 작업 역할과 연결된 경우 새 멤버가 리소스 풀에 자동으로 추가되지 않습니다. <br>사용자가 추가하려는 팀, 그룹, 회사 및 작업 역할에 속하는 경우, 동시에 사용자는 리소스 풀에 한 번만 추가됩니다.리소스 풀에 추가되어 비활성화된 <br>사용자가 사용자 목록에 희미하게 표시되고 비활성화된 것으로 표시됩니다.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (선택 사항) **실행 취소** 링크를 사용하여 그룹, 팀, 회사 또는 작업 역할을 통해 추가된 사용자를 제거합니다.

   >[!NOTE]
   >
   >리소스 풀에 보유할 수 있는 사용자 수에는 제한이 없습니다. 그러나 그렇지 않으면 리소스 관리가 문제가 될 수 있으므로 리소스 풀에 사용자를 너무 많이 추가하지 않는 것이 좋습니다. 사용자 목록에는 리소스 풀의 처음 2,000명의 사용자만 표시되며 알파벳순으로 표시됩니다.

   <span class="preview">미리 보기 환경의 샘플 이미지:</span>
   <span class="preview">![사용자가 리소스 풀에 추가됨](assets/users-in-resource-pool2.png)</span>

   프로덕션 환경의 샘플 이미지:
   ![사용자가 리소스 풀에 추가됨](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (선택 사항) 사용자를 제거하려면 사용자 이름 오른쪽에 있는 X 아이콘을 클릭합니다. 리소스 풀에서 사용자를 제거하는 방법에 대한 자세한 내용은 [리소스 풀에서 사용자 제거](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md)를 참조하십시오.
1. (선택 사항) **검색** 옵션을 사용하여 리소스 풀에서 사용자를 찾습니다.
1. Click **Create**.
