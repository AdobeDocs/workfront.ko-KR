---
product-area: projects
navigation-topic: financials
title: PIM(성능 인덱스 메서드) 설정
description: 프로젝트에 대한 PIM(성능 인덱스 방법)은 Adobe Workfront에서 CPI(비용 성과 인덱스), CSI(비용 일정 성과 인덱스), SPI(Schedule Performance Index) 및 EAC(Estimate At Completion)와 같은 프로젝트 성능 지표를 계산하는 데 사용하는 방법을 제어합니다.
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# PIM(성능 인덱스 메서드) 설정

프로젝트에 대한 PIM(성능 인덱스 방법)은 Adobe Workfront에서 CPI(비용 성과 인덱스), CSI(비용 일정 성과 인덱스), SPI(Schedule Performance Index) 및 EAC(Estimate At Completion)와 같은 프로젝트 성능 지표를 계산하는 데 사용하는 방법을 제어합니다.

Workfront은 다음을 사용하여 이러한 값을 계산합니다.

* 시간
* 비용

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
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>Finance 관리 권한을 사용하여 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## Workfront의 PIM에 대한 고려 사항

* Workfront 관리자 또는 그룹 관리자가 성능 인덱스 메서드(PIM)가 시간 기반 또는 비용 기반이어야 하는지 여부에 대해 기본값을 설정합니다. 성능 지표에 대한 계산은 이 기본값이 설정되는 방식에 따라 변경됩니다. PIM 계산 방법에 대한 기본값을 변경하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 프로젝트 관리자는 프로젝트의 재무 하위 탭에서 개별 프로젝트에 대한 PIM의 설정을 프로젝트 레벨에서 변경할 수도 있습니다. 프로젝트의 재무 하위 탭을 편집하려면 프로젝트에 대한 관리 권한이 있어야 합니다.

## 프로젝트에 대한 PIM(성능 인덱스 메서드) 설정

1. 소유자인 프로젝트로 이동합니다.

   >[!IMPORTANT]
   >
   >다음 단계를 수행하려면 프로젝트에 대한 권한 관리 가 필요합니다. 또한 프로젝트 소유자만 프로젝트의 재무 영역을 변경해야 합니다.

1. 클릭 **프로젝트 세부 사항** 왼쪽 패널에서 **재무** 영역.
1. 에서 값을 두 번 클릭합니다. **성능 인덱스 메서드** 편집할 필드입니다.
1. 의 다음 옵션 중에서 선택합니다 **성능 인덱스 메서드** 필드:

   | 시간 기반 | Workfront에서는 프로젝트의 CPI 및 EAC를 계산하는 데 계획 시간을 사용하고 프로젝트의 EAC는 시간 단위로 표시됩니다. |
   |---|---|
   | 비용 기반 | Workfront은 프로젝트의 CPI 및 EAC를 계산할 때 계획 노무비를 사용하고 EAC는 통화 값으로 표시됩니다. 이 옵션을 선택하는 경우 작업 담당자(작업 역할 또는 사용자)가 비용 비율에 연결되어 있는지 확인합니다. |

   {style=&quot;table-layout:auto&quot;}

1. 클릭 **저장** **변경 사항**.
