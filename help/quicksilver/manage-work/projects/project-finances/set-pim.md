---
product-area: projects
navigation-topic: financials
title: PIM(성과 지표 메서드) 설정
description: 프로젝트의 PIM(성과 지표 메서드)은 Adobe Workfront이 원가 성과 지수(CPI), 원가 일정 성과 지수(CSI), 일정 성과 지수(SPI) 및 완료 시 추정(EAC)과 같은 프로젝트 성과 지표를 계산하는 데 사용하는 방법을 제어합니다.
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# PIM(성과 지표 메서드) 설정

프로젝트의 PIM(성과 지표 메서드)은 Adobe Workfront이 원가 성과 지수(CPI), 원가 일정 성과 지수(CSI), 일정 성과 지수(SPI) 및 완료 시 추정(EAC)과 같은 프로젝트 성과 지표를 계산하는 데 사용하는 방법을 제어합니다.

Workfront은 다음을 사용하여 이러한 값을 계산합니다.

* 시간
* 비용

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 권한으로 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## Workfront의 PIM에 대한 고려 사항

* PIM(성능 인덱스 메서드)이 시간 기반이어야 하는지 비용 기반이어야 하는지에 대해 Workfront 관리자 또는 그룹 관리자가 기본값을 설정합니다. 성능 지표에 대한 계산은 이 기본값 설정 방법에 따라 변경됩니다. PIM 계산 방법에 대한 기본값을 변경하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.
* 프로젝트 관리자는 프로젝트의 재무 하위 탭에서 개별 프로젝트에 대한 프로젝트 수준의 PIM 설정을 변경할 수도 있습니다. 프로젝트의 재무 하위 탭을 편집하려면 프로젝트에 대한 관리 권한이 있어야 합니다.

## 프로젝트의 PIM(성과 지표 메서드) 설정

1. 자신이 소유자인 프로젝트로 이동합니다.

   >[!IMPORTANT]
   >
   >다음 단계를 수행하려면 프로젝트에 대한 관리 권한이 필요합니다. 또한 프로젝트 소유자만 프로젝트의 재무 영역을 변경하는 것이 좋습니다.

1. 왼쪽 패널에서 **프로젝트 세부 정보**&#x200B;를 클릭한 다음 **재무** 영역으로 이동합니다.
1. **성능 인덱스 메서드** 필드의 값을 두 번 클릭하여 편집합니다.
1. **성능 인덱스 메서드** 필드에서 다음 옵션 중 선택하십시오.

   | 시간 기반 | Workfront은 프로젝트의 CPI와 EAC를 계산할 때 계획된 시간을 사용하며 프로젝트의 EAC가 시간 단위의 숫자로 표시됩니다. |
   |---|---|
   | 비용 기반 | Workfront은 프로젝트의 CPI와 EAC를 계산할 때 계획된 인건비를 사용하며 EAC는 통화 값으로 표시됩니다. 이 옵션을 선택하는 경우 작업 담당자(작업 역할 또는 사용자)가 비용 비율과 연결되어 있는지 확인합니다. |

   {style="table-layout:auto"}

1. **저장** **변경 내용**&#x200B;을 클릭합니다.
