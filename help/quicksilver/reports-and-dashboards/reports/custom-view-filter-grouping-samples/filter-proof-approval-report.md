---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '필터: 이전 증명 버전을 생략하기 위한 증명 승인 보고서'
description: 증명 승인 보고서에서 현재 문서 버전 필터를 사용하여 승인을 기다리는 증명의 현재 버전만 포함할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 필터: 이전 증명 버전을 생략하기 위한 증명 승인 보고서

<!--Audited: 10/2024-->

증명 승인 보고서에서 **현재 문서 버전임** 필터를 사용하여 승인을 기다리는 현재 증명 버전만 포함할 수 있습니다.

이 기능은 여러 버전의 증명을 승인하라는 메시지가 표시되는 경우 유용합니다. 현재 문서 버전 필터로 증명 승인 보고서를 실행하면 보고서에는 승인 대기 중인 각 증명의 현재 버전만 나열되며 더 이상 작업할 필요가 없는 이전 버전은 생략됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 증명 승인 보고서를 필터링하여 이전 증명 버전 생략

증명 승인 보고서에 대한 필터를 만들 수 있습니다.

1. 이미 증명 승인 보고서가 있는 경우 엽니다.

   또는

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   증명 승인 보고서를 만들려면 오른쪽 상단의 **기본 메뉴** 아이콘 ![기본 메뉴 아이콘](assets/main-menu-icon.png)을 클릭하거나 왼쪽 상단의 **기본 메뉴** 아이콘 ![기본 메뉴 줄](assets/lines-main-menu.png)을(를) 클릭한 다음 사용 가능한 경우 **보고서** ![보고서 아이콘](assets/reports-in-main-menu.png)을 클릭하십시오.

1. **새 보고서**&#x200B;를 클릭합니다. 객체 유형 목록이 표시됩니다.
1. 목록에서 **증명 승인**을 클릭합니다.
Report Builder가 열립니다.
1. **필터**&#x200B;를 클릭한 다음 **필터 규칙 추가**&#x200B;를 클릭합니다.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. **보고서에 대한 필터 규칙 설정** 상자 내부를 클릭한 다음 목록에서 **증명 승인**&#x200B;을 선택합니다.
1. **증명 승인** 개체 아래의 목록에서 **현재 문서 버전임**&#x200B;을 클릭합니다.
1. 필터 수정자에 대해 같음을 선택한 다음 참을 선택합니다.
1. Adobe Workfront의 왼쪽 아래 모서리에서 **저장 + 닫기**&#x200B;를 클릭한 다음 표시되는 상자에서 **적용**&#x200B;을 클릭합니다.

   증명 승인이 이 필터링 기준과 일치하는 경우 증명 승인 보고서에는 문서의 현재 버전과 연결된 증명만 표시됩니다.
