---
title: 기존 그룹화 편집
description: 기존 그룹화 편집
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 기존 그룹화 편집

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

원래 만들었거나 사용자와 공유된 기존 그룹화를 사용자 지정할 수 있습니다. 그런 다음 새 그룹화로 저장할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> <p>요청 이상 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서에서 그룹화를 편집할 수 있습니다.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에서 그룹화를 편집하려면 보고서에 대한 권한 관리</p> <p>그룹화에 대한 권한 관리 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

그룹화를 편집하려면 먼저 만들어야 합니다.

그룹화 만들기에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)를 참조하십시오.

## 방법 단계

1. 사용자 지정할 그룹화가 포함된 개체 목록으로 이동합니다.
1. **그룹화** 아이콘을 클릭합니다.
1. 사용자 지정할 그룹화를 선택한 다음 **편집** 아이콘을 클릭합니다.

   ![편집 아이콘을 선택합니다.](assets/customizegrouping-nwe-standard-350x291.png)

   그룹화 맞춤화를 위한 인터페이스 빌더가 열립니다.

1. **그룹화 미리 보기** 섹션에서 **그룹화 추가**&#x200B;를 클릭하여 보고서의 정보를 구성하는 방법을 정의합니다. 보고서에서 그룹화가 표시되는 모양에 대한 미리보기가 아래에 표시되어 있습니다.

1. 보고서에서 정보를 구성하는 방법을 나타내는 필드 이름을 입력한 다음 드롭다운 목록에 나타나면 해당 필드 이름을 클릭합니다.
1. (선택 사항 및 조건부) 업데이트된 목록을 볼 때 그룹화 결과를 확장하지 않고 축소하려면 **기본적으로 이 그룹화 축소**&#x200B;를 선택합니다. 이 설정은 기본적으로 비활성화되며 그룹화 결과는 항상 확장된 목록에 표시됩니다.

   업데이트된 목록과 기존 목록에 대한 자세한 내용은 문서 [Adobe Workfront 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)의 &quot;업데이트된 목록과 기존 목록의 차이점&quot; 섹션을 참조하십시오.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* 목록을 볼 때 수동으로 그룹화를 조정하면 Workfront은 로그아웃하기 전까지 수동 기본 설정을 기억합니다. 다시 로그인하면 이 설정에 따라 목록이 표시됩니다.
   >* 차트 요소나 레거시 목록에서 그룹화에 액세스하면 그룹화 결과가 항상 확장되어 표시됩니다. 이러한 경우 이 설정은 무시됩니다.

1. 4, 5, 6단계를 반복하여 추가 그룹화를 정의합니다.\
   정보 구성을 위해 최대 3개의 그룹화를 정의할 수 있습니다. 매트릭스 보고서를 만들어 최대 4개의 그룹화로 정보를 추가로 구성할 수 있습니다. 매트릭스 보고서에 대한 자세한 내용은 [매트릭스 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)를 참조하십시오.

1. 현재 그룹화를 변경 내용으로 바꾸려면 **새 그룹화로 저장**&#x200B;을 클릭하세요.
