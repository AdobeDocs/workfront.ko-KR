---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''오류 메시지: 잘못된 매개 변수: 전환 값'
description: '기존 사용자 지정 양식에서 사용자 지정 필드의 형식을 변경하려고 하면 다음 오류 메시지가 표시됩니다. ''잘못된 매개 변수: 변환 값 ''&lt;..&gt;"'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 1%

---

# 오류 메시지: 잘못된 매개 변수: 전환 값

## 문제

기존 사용자 지정 양식에서 사용자 지정 필드의 형식을 변경하려고 하면 다음 오류 메시지가 표시됩니다. &quot;잘못된 매개 변수: 변환 값 &quot;&lt;..>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 원인

이 메시지는 다음 시나리오에서 발생합니다.

예를 들어, 텍스트 형식의 사용자 지정 필드가 있습니다.  이제 사용자 지정 필드의 형식을 통화로 변경하려고 합니다. Adobe Workfront 인스턴스의 어딘가에 이 필드는 이미 개체에 연결되어 있으며 이 필드에 이미 지정된 정보가 있습니다. 이러한 필드 중 하나 이상에 있는 기존 정보는 이미 텍스트 형식으로 되어 있습니다. 따라서 필드의 형식은 통화로 변경할 수 없습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront 플랜</a>*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">이전 라이센스 개요</a>*</p> </td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>액세스 수준*</strong> </td> 
   <td> <p>액세스 권한 편집:</p> 
    <ul> 
     <li> <p>보고서, 대시보드 및 달력 만들기</p> </li> 
     <li> <p>필터, 보기 및 그룹화 만들기</p> </li> 
    </ul> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 솔루션

다음을 수행합니다.

1. 사용자 지정 Forms과 연결된 이 필드가 있을 수 있는 모든 개체의 보고서를 작성합니다.\
   보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 보고서 보기에서 편집하려는 사용자 지정 필드를 포함시키면 텍스트 값으로 이 필드가 채워지는 개체를 볼 수 있습니다.
1. 텍스트 형식으로 표시되는 개체의 사용자 지정 필드 값을 수정하고 Currency 형식의 값을 제공합니다. 그런 다음 사용자 지정 양식의 형식 필드를 다시 변경하려고 합니다.\
   또는\
   텍스트 형식 정보로 이미 채워진 필드 값이 너무 많은 경우 사용자 지정 양식에 새 사용자 지정 필드를 추가하고 통화 형식으로 지정하십시오.
