---
title: 클래식 레이아웃 템플릿 삭제
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 'Classic Workfront 경험의 레이아웃 템플릿은 더 이상 Workfront 인터페이스에서 사용할 수 없지만 여전히 Workfront 데이터에 영향을 줄 수 있습니다. 이로 인해 보고서 또는 대시보드의 레이아웃 템플릿(예: 다음 사용자와 공유)의 영향을 받는 필드에 불일치가 발생할 수 있습니다.'
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 58%

---

# 레이아웃 템플릿에 대한 관리 액세스 권한 부여

Classic Workfront 경험의 레이아웃 템플릿은 더 이상 Workfront 인터페이스에서 사용할 수 없지만 여전히 Workfront 데이터에 영향을 줄 수 있습니다. 이로 인해 보고서 또는 대시보드의 레이아웃 템플릿(예: 다음 사용자와 공유)의 영향을 받는 필드에 불일치가 발생할 수 있습니다.

클래식 레이아웃 템플릿을 삭제하면 이러한 불일치를 해결할 수 있습니다. Workfront 인터페이스에서는 사용할 수 없으므로 은 Workfront API를 사용하여 삭제해야 합니다.

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
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## API 호출을 사용하여 클래식 레이아웃 템플릿 삭제

브라우저의 URL 표시줄에 API 호출을 입력하고 Enter 키를 누를 수 있습니다. 브라우저에 API 응답이 표시됩니다.

>[!NOTE]
>
>전역 및 시스템 레이아웃 템플릿은 삭제할 수 없습니다.

1. Workfront에 로그인.
1. 다음 API 호출을 사용하여 삭제하려는 레이아웃 템플릿을 찾습니다.
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 삭제하려는 레이아웃 템플릿의 ID를 기록해 두십시오.
1. 다음 API 호출을 사용하여 세션 ID를 찾습니다.
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >세션 ID를 누구와도 공유하지 마십시오.

1. 다음 API 호출에 레이아웃 템플릿 ID 및 세션 ID를 삽입합니다.
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 4단계의 API 호출을 브라우저의 URL 표시줄에 붙여넣고 Enter 키를 누릅니다.

   이렇게 되면 레이아웃 템플릿이 삭제됩니다.
