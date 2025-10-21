---
product-area: home
navigation-topic: use-the-home-area
title: 내 승인 위젯을 사용하여 승인 관리
description: 내 승인 위젯에는 보류 중, 할당, 위임 및 제출된 모든 승인이 한 곳에 표시됩니다. 여기에서 승인을 필터링 및 구성하고 필요한 경우 결정을 내리고 승인을 위임할 수 있습니다.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 5%

---

# 내 승인 위젯을 사용하여 승인 관리

내 승인 위젯에는 보류 중, 할당, 위임 및 제출된 모든 승인이 한 곳에 표시됩니다. 여기에서 승인을 필터링 및 구성하고 필요한 경우 결정을 내리고 승인을 위임할 수 있습니다.

내 승인 위젯은 다음 Workfront 오브젝트에서 승인을 지원합니다.

* 작업
* 문제
* 프로젝트
* 문서
* 교정쇄
* 레코드 요청 계획
* 타임시트

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p>
   <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>승인과 연관된 객체에 대한 보기 이상의 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>승인과 연관된 오브젝트에 대한 이상 권한 보기</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 내 승인 위젯에서 작업 승인

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 승인** 위젯을 추가합니다.
1. (조건부) **필터** 드롭다운 메뉴를 클릭한 다음 **모두**&#x200B;를 선택하여 귀하에게 할당 및 위임된 승인을 확인합니다.

   >[!NOTE]
   >
   >작업 역할 또는 그룹에 할당된 승인이 홈에 표시되지 않습니다. 팀에 할당된 승인은 각 팀 구성원의 내 승인 위젯에 표시됩니다.


1. 승인 결정을 내릴 품목을 선택합니다.

   ![내 승인 위젯](assets/my-approvals-widget.png)

1. 오른쪽 패널에서 승인 결정을 내릴 때 사용할 수 있는 옵션 중 하나를 클릭합니다. 승인하는 항목의 유형에 따라 페이지의 오른쪽 상단에 다음 옵션이 표시됩니다.

   <table>
   <tr>
      <td>
      <p><strong>액세스</strong></p>
      </td>
      <td>
      <p><strong>작업 항목</strong></p>
      </td>
      <td>
      <p><strong>문서</strong></p>
      </td>
      <td>
      <p><strong>교정쇄</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>부여</li>
      <li>무시</li>
      </ul>
      원하는 경우 <b>액세스 변경</b> 드롭다운 메뉴에서 액세스 수준을 조정할 수 있습니다.
      </td>
      <td>
         <ul>
         <li>승인</li>
         <li>거부</li>
         </ul>
      결정 버튼의 드롭다운 메뉴를 클릭하여 결정과 함께 주석을 남길 수 있습니다.
      </td>
      <td>
   승인자로 할당됨
         <ul>
         <li>승인</li>
         <li>변경 사항과 함께 승인</li>
         <li>작업 필요</li>
         </ul>
   검토자로 할당됨
         <ul>
         <li>내 검토 완료</li>
         </ul>
      이 열의 옵션은 통합 승인에만 적용됩니다. 기존 문서 승인은 작업 항목 승인과 동일하게 표시됩니다. 
      </td>
      <td>
         <ul>
         <li>증명으로 이동</li>
         </ul>
         증명 뷰어에서 결정을 내립니다. 증명 검토에 대한 자세한 내용은 <a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Adobe Workfront 내에서 증명 검토</a>를 참조하십시오.
      </td>
   </tr>
   </table>

결정을 내리면 내 승인 위젯에서 승인이 제거됩니다.