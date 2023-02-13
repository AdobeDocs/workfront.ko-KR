---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '필터: 증명 승인 보고서에서 이전 증명 버전을 생략합니다.'
description: 증명 승인 보고서에서 현재 문서 버전임 필터를 사용하여 승인을 기다리는 현재 버전의 증명만 포함할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 필터: 증명 승인 보고서에서 이전 증명 버전을 생략합니다.

증명 승인 보고서에서 **현재 문서 버전입니다.** 승인을 기다리는 현재 버전의 교정증만 포함하도록 필터링합니다.

이 기능은 예를 들어, 여러 버전의 증명을 승인하라는 요청을 받은 경우 유용합니다. 현재 문서 버전 필터로 증명 승인 보고서를 실행하면, 보고서는 승인을 기다리는 각 증명의 현재 버전만 나열하고 더 이상 작업할 필요가 없는 이전 버전을 생략합니다. 

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 증명 승인 보고서를 필터링하여 이전 증명 버전을 생략합니다.

1. 이미 증명 승인 보고서가 있는 경우 엽니다.

   또는

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   자체 증명 승인 보고서를 만들려면 주 메뉴를 클릭합니다 ![](assets/main-menu-icon.png)를 클릭한 다음 **보고서** ![](assets/reports-in-main-menu.png). 클릭 **새 보고서**. 표시되는 목록에서 로 스크롤하여 을 클릭합니다. **증명 승인**. 클릭 **저장 + 닫기**, 입력 **보고서 이름** (선택 사항) **보고서 저장**.

1. 클릭 **보고서 작업 > 편집**.
1. 클릭 **필터**&#x200B;를 클릭한 다음 **필터 규칙 추가**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 클릭 **증명 승인**.
1. 목록이 표시되면 **현재 문서 버전입니다.**.
1. 클릭 **저장 + 닫기** Adobe Workfront의 왼쪽 아래에서 **보고서 저장** 이 표시되는 상자에 나타납니다.
