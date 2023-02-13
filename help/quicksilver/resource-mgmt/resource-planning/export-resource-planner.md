---
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 계획자에서 정보 내보내기
description: 리소스 플래너의 모든 보기에서 컴퓨터에 저장된 Excel(.xlsx) 파일로 정보를 내보낼 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# 리소스 계획자에서 정보 내보내기

리소스 플래너의 모든 보기에서 컴퓨터에 저장된 Excel(.xlsx) 파일로 정보를 내보낼 수 있습니다.

>[!IMPORTANT]
>
>표시되는 정보와 Resource Planner에서 내보낼 수 있는 정보는 제한이 있습니다. 이러한 제한 사항에 대한 자세한 내용은 [리소스 계획자 표시 제한 사항](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 사용자 및 리소스 관리에 대한 액세스 보기 이상</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 보기 이상</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 리소스 계획자에서 정보 내보내기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **리소스**. 다음 **계획자** 기본적으로 표시됩니다.

1. 계획자에 대한 뷰를 선택합니다. 다음 옵션 중 하나를 선택할 수 있습니다.

   * 사용자별 보기
   * 프로젝트별 보기
   * 역할별 보기

1. 클릭 **내보내기**.

   내보내기 옵션 대화 상자가 표시됩니다.

   ![](assets/rp-export-options-box-350x421.png)

1. 다음 정보를 지정합니다.\
   **시작 날짜**: 내보내기의 시작 날짜입니다. 내보낸 파일에는 여기서 지정한 일이 포함된 주의 첫 날로 시작하는 할당 및 가용성 정보가 포함되어 있습니다.\
   **기간 수**: 파일에 포함할 기간 수입니다. 기본값은 4마침표입니다.\
   **유형**: 내보낸 파일에 정보를 표시할 기간 유형(주, 월 또는 분기)입니다.\
   내보낼 수 있는 최대 기간은 다음과 같습니다.

   * 52주
   * 36개월
   * 12분기

   **내보낼 선택**: 선택한 뷰에 따라 화면에 나열된 모든 객체 또는 특정 객체에 대한 가용성 및 예산 정보를 익스포트하도록 선택할 수 있습니다.
을(를) 선택하여 다음 정보를 내보낼 수 있습니다.

   * 프로젝트 보기에서 을(를) 선택하여 내보냅니다.

      * 프로젝트
      * 프로젝트 및 역할
      * 모든 항목(기본 옵션임)
   * 사용자 보기에서 다음을 내보내려면 선택합니다.

      * 사용자
      * 사용자 및 프로젝트
      * 모든 항목(기본 옵션임)
   * 역할 보기에서 다음을 내보내려면 선택합니다.

      * 역할
      * 역할 및 프로젝트
      * 모든 항목(기본 옵션임)

   **데이터 서식**: Excel 파일을 표시할 방법에 따라 다음 옵션을 선택합니다.

   * **Raw**: 가용성 및 할당 정보를 Excel 파일에 속한 객체별로 그룹핑하지 않은 상태로 표시하려면 선택합니다. (기본 옵션임)
   * **그룹화됨**: 이 옵션을 선택하면 가용성 및 할당 정보가 속한 객체별로 그룹핑됩니다. 그러면 내보낸 정보가 화면에 표시되는 대로 표시됩니다.

   내보낸 파일에서 정보가 표시되는 방식에 대한 샘플이 [내보내기 옵션] 대화 상자에 표시됩니다.

1. 클릭 **내보내기** 자원 계획자에서 정보를 익스포트하려면\
   저장한 정보만 내보냅니다.

1. (조건부) 역할이나 프로젝트 뷰에서 계획되지 않은 시간 예산책정된 시간을 저장한 경우 **저장 후 계속.**
Excel(.xlsx) 파일이 컴퓨터에 다운로드됩니다.
\
   파일을 다운로드할 준비가 되어 있는 동안에는 Resource Planner에서 내보낼 수 없습니다.\
   (조건부) 많은 양의 데이터를 내보내는 경우 파일을 다운로드할 수 있는 링크가 포함된 이메일을 받게 됩니다.\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (조건부) 내보낸 파일로 이메일을 받으면 을 클릭합니다 **다운로드** 를 클릭하여 파일을 다운로드하십시오.\
   이렇게 하면 파일을 다운로드할 수 있는 Workfront으로 돌아갑니다.\
   다운로드를 완료하려면 Workfront에 로그인해야 합니다.\
   파일이 전달될 때 다운로드하지 않으면 내보내기 시작 후 7일 동안 다운로드 링크가 활성 상태로 유지됩니다.
