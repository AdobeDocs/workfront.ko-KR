---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 미리 보기 샌드박스 환경에서 보고서 보내기
description: 이 페이지의 정보는 미리 보기 및 사용자 지정 새로 고침 샌드박스 환경에서만 사용할 수 있는 기능을 참조합니다. 이 기능은 프로덕션 환경에서 사용할 수 없습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 미리 보기 샌드박스 환경에서 보고서 보내기

이 페이지의 정보는 미리 보기 및 사용자 지정 새로 고침 샌드박스 환경에서만 사용할 수 있는 기능을 참조합니다. 이 기능은 프로덕션 환경에서 사용할 수 없습니다.

모든 Adobe Workfront 테스트 환경에서 보고서 배달 옵션을 설정할 수 있습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

테스트 환경은 프로덕션 환경에서 최대한 가까운 기능을 하도록 되어 있지만, 일부 기능은 프로덕션 환경과 다릅니다.

테스트 환경에서 보고서를 예약할 수 있지만 전달하는 방식은 프로덕션 환경에서 보고서를 전달하는 방법과 다릅니다.

프로덕션 환경에서 전송할 보고서를 예약하는 방법에 대한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

보고서를 예약하는 위치에 따라 배달 기능이 미리 보기 와 사용자 지정 새로 고침 샌드박스 간에 다릅니다.

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

## 미리 보기 환경에서 보고서 예약

* [미리 보기 환경에서 보고서 예약](#schedule-reports-in-the-preview-environment)

### 미리 보기 환경에서 보고서 예약

미리 보기 환경에서 배달된 보고서가 작성되는지 여부는 미리 보기 환경에서 작성되는지 여부에 따라 다릅니다 **이 테스트 환경에서 전자 메일 받기** 이 활성화되어 있거나 활성화되어 있지 않습니다.

샌드박스 환경에서 전자 메일 활성화에 대한 자세한 내용은 [미리 보기 샌드박스 환경에서 전자 메일 게재 활성화](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

미리 보기 환경에서 배달할 보고서를 예약하는 것은 프로덕션 환경에서 보고서를 예약하는 것과 동일합니다. 보고서 배달 예약에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

미리 보기 환경에서 보고서 배달을 예약할 때 다음 시나리오가 있습니다.

* When **이 테스트 환경에서 전자 메일 받기** 보고서를 받는 사용자에게 이 비활성화되어 있으며, 전송할 보고서를 예약할 때 파일이 생성되지 않습니다.
* When **이 테스트 환경에서 전자 메일 받기** 보고서를 받고 있는 사용자에 대해 이 활성화되어 있으면 전달을 위해 보고서를 예약할 때 생성되는 파일이 사용자의 문서 탭에 추가됩니다.

## 사용자 지정 새로 고침 샌드박스 환경에서 보고서 예약

사용자 지정 새로 고침 샌드박스에서 전달된 보고서가 생성되는지 여부는 이 테스트 환경에서 이메일 수신 설정이 활성화되어 있는지 여부에 따라 다릅니다.

미리 보기 환경에서 전자 메일 사용에 대한 자세한 내용은 섹션을 참조하십시오 [전자 메일 알림 설정을 보고 수정합니다](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) 기사 [고유한 이벤트 알림 활성화 또는 비활성화](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

사용자 지정 새로 고침 샌드박스 환경에서 전달을 위한 보고서를 예약하는 것은 프로덕션 환경에서 보고서를 예약하는 것과 동일합니다. 보고서 배달 예약에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

사용자 지정 새로 고침 샌드박스 환경에서 보고서 배달을 예약할 때 다음 시나리오가 있습니다.

* 보고서를 받고 있는 사용자에 대해 이 테스트 환경에서 전자 메일 받기 가 비활성화되면 전송을 위해 보고서를 예약할 때 파일이 생성되지 않습니다.
* 보고서를 받는 사용자에게 이 테스트 환경에서 이메일 수신 이 활성화되면 보고서는 사용자와 연결된 이메일 주소에 대한 첨부 파일로 이메일로 전송됩니다.

## 외부 사용자에게 통지하는 방법

외부 사용자는 Workfront 테스트 환경에서 전송된 보고서를 받거나 이메일 알림을 받지 않습니다.

외부 사용자는 프로덕션 환경에서 전달되는 경우에만 이메일 보고서를 받게 됩니다.
