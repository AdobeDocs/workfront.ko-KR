---
title: 기존 그룹화 편집
description: 기존 그룹화 편집
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 기존 그룹화 편집

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

원래 만들거나 사용자와 공유된 기존 그룹을 사용자 지정할 수 있습니다. 그런 다음 새 그룹으로 저장할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서의 그룹을 편집합니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서의 그룹을 편집합니다</p> <p>그룹에 대한 권한 관리 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

편집하려면 먼저 그룹을 만들어야 합니다.

그룹 생성에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## 방법 단계

1. 사용자 지정할 그룹이 포함된 객체 목록으로 이동합니다.
1. 을(를) 클릭합니다. **그룹화** 아이콘.
1. 사용자 지정할 그룹을 선택한 다음 **편집** 아이콘.

   ![편집 아이콘을 선택합니다.](assets/customizegrouping-nwe-standard-350x291.png)

   그룹을 사용자 지정하는 인터페이스 빌더가 열립니다.

1. 에서 **그룹화 미리 보기** 섹션을 클릭합니다. **그룹화 추가** 를 입력하여 보고서에 있는 정보를 구성하는 방법을 정의할 수 있습니다. 보고서에서 그룹이 어떻게 보이는지에 대한 미리 보기는 아래에 나와 있습니다.

1. 보고서에서 정보를 구성할 방법을 나타내는 필드의 이름을 입력한 다음 드롭다운 목록에 표시될 때 클릭합니다.
1. (선택 사항 및 조건부) 업데이트된 목록을 볼 때 **기본적으로 이 그룹을 축소합니다.** 그룹화 결과가 확장되지 않고 축소되도록 하려면 이 설정은 기본적으로 비활성화되며 그룹화 결과는 항상 확장된 목록에 표시됩니다.

   업데이트 및 레거시 목록에 대한 자세한 내용은 문서의 &quot;업데이트된 목록과 레거시 목록 간의 차이&quot; 섹션을 참조하십시오 [Adobe Workfront에서 목록 시작](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* 목록을 볼 때 수동으로 그룹화를 조정하면 Workfront은 로그아웃할 때까지 수동 환경 설정을 기억합니다. 다시 로그인하면 이 설정에 따라 목록이 표시됩니다.
   >* 그룹화 결과는 항상 차트 요소 또는 레거시 목록에서 액세스한 후에 확장됩니다. 이러한 경우 이 설정은 무시됩니다.


1. 추가적인 그룹화를 정의하려면 4, 5 및 6단계를 반복합니다.\
   정보를 구성할 최대 3개의 그룹을 정의할 수 있습니다. 매트릭스 보고서를 만들어 최대 4개의 그룹으로 정보를 추가로 구성할 수 있습니다. 매트릭스 보고서에 대한 자세한 내용은 [매트릭스 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. 클릭 **새 그룹으로 저장** 현재 그룹을 변경 내용으로 바꿉니다.
