---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 미리보기 샌드박스 환경에서 보고서 보내기
description: 이 페이지의 정보는 미리보기 및 사용자 지정 새로 고침 샌드박스 환경에서만 사용할 수 있는 기능을 참조합니다. 이 기능은 프로덕션 환경에서는 사용할 수 없습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# 미리보기 샌드박스 환경에서 보고서 보내기

<!-- Audited: 11/2024 -->

이 페이지의 정보는 미리보기 및 사용자 지정 새로 고침 샌드박스 환경에서만 사용할 수 있는 기능을 참조합니다. 이 기능은 프로덕션 환경에서는 사용할 수 없습니다.

모든 Adobe Workfront 테스트 환경에서 보고서 배달 옵션을 설정할 수 있습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

테스트 환경은 프로덕션 환경에 최대한 근접하게 작동해야 하지만, 일부 기능은 프로덕션 환경과 다릅니다.

테스트 환경에서 보고서를 예약할 수 있지만 보고서 전달 방식은 프로덕션 환경에서 전달되는 방식과 다릅니다.

프로덕션 환경에서 보고서 배달 예약에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하세요.

보고서를 예약하는 위치에 따라 배달 기능이 미리 보기 및 사용자 지정 새로 고침 샌드박스 간에 달라집니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
      <td> 
      <p>신규:</p>
         <ul>
         <li><p>표준</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>플랜</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 미리보기 환경에서 보고서 예약

* [미리보기 환경에서 보고서 예약](#schedule-reports-in-the-preview-environment)

### 미리보기 환경에서 보고서 예약

미리 보기 환경에서 배달된 보고서가 생성되는지 여부는 **이 테스트 환경에서 전자 메일 받기**&#x200B;의 사용 여부에 따라 달라집니다.

샌드박스 환경에서 전자 메일을 사용하는 방법에 대한 자세한 내용은 [미리 보기 샌드박스 환경에서 전자 메일 배달 사용](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)을 참조하십시오.

![샌드박스에서 이메일 수신 옵션](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

미리보기 환경에서 보고서 배달을 예약하는 것은 프로덕션 환경에서 보고서를 예약하는 것과 동일합니다. 보고서 배달 예약에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하세요.

미리보기 환경에서 보고서 배달을 예약할 때 다음과 같은 시나리오가 존재합니다.

* 보고서를 받는 사용자에 대해 **이 테스트 환경에서 전자 메일 수신**&#x200B;을 사용하지 않도록 설정하면 보고서 배달을 예약할 때 파일이 생성되지 않습니다.
* 보고서를 받는 사용자에 대해 **이 테스트 환경에서 전자 메일 수신**&#x200B;을 사용하도록 설정하면 보고서의 배달 일정을 예약할 때 생성되는 파일이 사용자의 문서 탭에 추가됩니다.

## 사용자 지정 새로 고침 샌드박스 환경에서 보고서 예약

배달된 보고서가 사용자 지정 새로 고침 샌드박스에서 생성되는지 여부는 이 테스트 환경에서 이메일 수신 설정의 활성화 여부에 따라 달라집니다.

미리 보기 환경에서 전자 메일을 사용하는 방법에 대한 자세한 내용은 문서 [사용자 전자 메일 알림 수정](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)의 [전자 메일 알림 설정 보기 및 수정](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) 섹션을 참조하십시오.

![샌드박스에서 이메일 수신 옵션](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

사용자 지정 새로 고침 샌드박스 환경에서 보고서 배달을 예약하는 것은 프로덕션 환경에서 보고서를 예약하는 것과 동일합니다. 보고서 배달 예약에 대한 자세한 내용은 [보고서 배달 개요](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하세요.

사용자 지정 새로 고침 샌드박스 환경에서 보고서 배달을 예약할 때 다음과 같은 시나리오가 존재합니다.

* 보고서를 받는 사용자에 대해 이 테스트 환경에서 이메일 수신 이 비활성화되어 있으면 보고서 배달을 예약할 때 파일이 생성되지 않습니다.
* 보고서를 받는 사용자에 대해 이 테스트 환경에서 이메일 수신 이 활성화되면 보고서가 사용자와 연결된 이메일 주소에 대한 첨부 파일로 이메일로 전송됩니다.

## 외부 사용자에게 알리는 방법

외부 사용자는 Workfront 테스트 환경에서 전송된 보고서를 받지 않으며 이메일 알림을 받지 않습니다.

외부 사용자는 프로덕션 환경에서 제공되는 경우에만 이메일 보고서를 받습니다.
