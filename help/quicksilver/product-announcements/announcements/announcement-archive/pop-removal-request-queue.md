---
content-type: reference
navigation-topic: announcements
title: 요청 대기열에 대한 POP 이메일을 21.1로 대체하는 새로운 Adobe Workfront 관리 시스템
description: 요청 대기열에 대한 POP 이메일 옵션을 새로운 Adobe Workfront 관리 시스템으로 바꾸는 중입니다. 이메일을 통해 요청을 제출할 수는 있지만, 대신 요청 대기열 영역에서 새 Workfront 관리 이메일 주소를 설정해야 합니다.
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 요청 대기열에 대한 POP 이메일을 21.1로 대체하는 새로운 Adobe Workfront 관리 시스템

요청 대기열에 대한 POP 이메일 옵션을 새로운 Adobe Workfront 관리 시스템으로 바꾸는 중입니다. 이메일을 통해 요청을 제출할 수는 있지만, 대신 요청 대기열 영역에서 새 Workfront 관리 이메일 주소를 설정해야 합니다.

## POP 이메일 옵션을 제거하는 이유는 무엇입니까?

POP 기술은 신뢰할 수 없고 안전성이 떨어지는 이메일 옵션입니다. 또한 POP 이메일과 관련된 고객 문제도 다수 볼 수 있습니다. Workfront 관리 시스템을 변경하면 보다 안정적인 경험이 제공됩니다.

## 어떤 조치를 취해야 합니까?

프로덕션 환경에서 POP 이메일로 설정한 각 요청 대기열에 대해 새 이메일 주소를 설정하고 필요에 따라 새 이메일 주소를 배포해야 합니다. 자세한 내용은 [사용자가 요청 대기열 프로젝트에 문제를 이메일로 보낼 수 있도록 설정](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md)을 참조하십시오.

## 전환 계획은 무엇입니까?

2월 초 21.1 릴리스부터 60일 동안 새로운 *@intake.workfront.com* 메일 주소로 사용자를 전환할 수 있습니다. 60일 동안 이전에 사용한 POP 이메일은 계속 작동합니다.

## 미리보기에서 테스트하려면 어떻게 해야 합니까?

미리보기에서 이러한 변경 사항을 테스트하려면 미리보기 환경에서 이메일을 활성화해야 합니다. 이렇게 하려면 [미리 보기 샌드박스 환경에서 전자 메일 배달 활성화](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)의 미리 보기에서 전자 메일 관리 섹션에 있는 지침을 따릅니다.

>[!IMPORTANT]
>
>여기서 설정한 내용은 프로덕션 환경으로 이월되지 않습니다. 기능이 프로덕션에 릴리스된 후 이 프로세스를 다시 수행해야 합니다.
