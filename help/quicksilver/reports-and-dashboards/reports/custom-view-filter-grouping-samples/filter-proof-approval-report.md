---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '필터: 이전 증명 버전을 생략하기 위한 증명 승인 보고서'
description: 증명 승인 보고서에서 현재 문서 버전 필터를 사용하여 승인을 기다리는 증명의 현재 버전만 포함할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 필터: 이전 증명 버전을 생략하기 위한 증명 승인 보고서

증명 승인 보고서에서 **현재 문서 버전임** 필터를 사용하여 승인을 기다리는 현재 증명 버전만 포함할 수 있습니다.

이 기능은 여러 버전의 증명을 승인하라는 메시지가 표시되는 경우 유용합니다. 현재 문서 버전 필터로 증명 승인 보고서를 실행하면 보고서에는 승인 대기 중인 각 증명의 현재 버전만 나열되며 더 이상 작업할 필요가 없는 이전 버전은 생략됩니다. 

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>필터 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 증명 승인 보고서를 필터링하여 이전 증명 버전 생략

1. 이미 증명 승인 보고서가 있는 경우 엽니다.

   또는

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   자체 증명 승인 보고서를 만들려면 기본 메뉴 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **보고서** ![](assets/reports-in-main-menu.png)을(를) 클릭합니다. **새 보고서**&#x200B;를 클릭합니다. 표시되는 목록에서 로 스크롤하여 **증명 승인**&#x200B;을 클릭합니다. **저장 + 닫기**&#x200B;를 클릭하고 **보고서 이름**(선택 사항)을 입력한 다음 **보고서 저장**&#x200B;을 클릭합니다.

1. **보고서 작업 > 편집**&#x200B;을 클릭합니다.
1. **필터**&#x200B;를 클릭한 다음 **필터 규칙 추가**&#x200B;를 클릭합니다.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. **승인 증명**&#x200B;을 클릭합니다.
1. 표시되는 목록에서 **현재 문서 버전임**&#x200B;을 클릭합니다.
1. Adobe Workfront의 왼쪽 아래 모서리에서 **저장 + 닫기**&#x200B;를 클릭한 다음 표시되는 상자에서 **보고서 저장**&#x200B;을 클릭합니다.
