---
title: 새 라이선스 플랜에서 비유료 사용자에 대한 자동 업그레이드 옵션 사용 안 함
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 액세스,수준,시스템,관리자,표준,조명,기여자
navigation-topic: access-levels
description: Workfront에 로그인하고 작업하려면 모든 사용자에게 액세스 수준이 있어야 합니다. 액세스 수준을 사용하여 사용자가 특정 Workfront 개체 및 영역을 보고 수행할 수 있는 작업을 제어합니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 1%

---

# 새 라이선스 플랜에서 비유료 사용자에 대한 자동 업그레이드 옵션 사용 안 함

증명 및 문서 결정은 새로운 플랜에 대한 모든 비유료 Workfront 라이선스에 대해 제한됩니다. 사용자가 할당된 결정 수에 도달하면 기본적으로 Light 라이선스로 업그레이드됩니다.

설정 영역에서 자동 업그레이드 옵션을 비활성화할 수 있습니다. 자동 업그레이드 작동 방식에 대한 자세한 내용은 [비유료 사용자에 대한 제한된 문서 및 증명 결정 개요](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)를 참조하십시오.

>[!IMPORTANT]
>
>비활성화되면 할당된 결정 수를 초과하는 비유료 사용자는 자동으로 업그레이드되지 않습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>새 플랜: 표준
   <p>또는</p>
   <p>현재 플랜: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

## 비유료 사용자에 대한 자동 업그레이드 비활성화

{{step-1-to-setup}}

1. 왼쪽 탐색에서 [!UICONTROL **시스템**]&#x200B;을 확장한 다음 [!UICONTROL **기본 설정**]&#x200B;을 클릭합니다.
1. [!UICONTROL **일반 환경 설정**] 섹션에서 [!UICONTROL **액세스 수준 내 자동 업그레이드 사용 안 함**] 상자를 선택합니다.
1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.
