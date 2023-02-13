---
title: 22.1 요청 개선 사항
description: 22.1 요청 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 22.1 요청 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.1 릴리스로 향상된 모든 요청을 설명합니다. 이러한 개선 사항은 프로덕션 환경에서 사용할 수 있습니다

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022년 1월 17일이 있는 주.

22.1 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.1 릴리스 개요](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 요청을 만들 수 있는 액세스 권한이 없는 사용자에 대한 인터페이스 개선

요청을 사용할 때 사용자의 경험을 향상시키기 위해 로그인한 사용자에게 요청을 만들 수 있는 액세스 권한이 없음을 나타내는 인터페이스 개선 사항을 도입했습니다. 이 개선 사항으로 인해 문제를 만들 수 있는 액세스 권한이 없는 사용자에게 새 요청 단추가 흐리게 표시됩니다. 흐리게 표시된 단추 위로 마우스를 가져가면 Workfront 관리자가 현재 사용자의 요청을 만들기 위해 액세스를 제한했음을 설명하는 도구 설명이 표시됩니다.

이 개선 사항 전에 이러한 사용자에 대한 요청 영역에 새 요청 단추가 표시되지 않았습니다. 요청을 새로 복사하고 제출도 제한됩니다.

요청 만들기에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).

## 요청 복사 및 제출

요청 제출 프로세스를 최적화하기 위해 기존 요청을 복사하고 새 요청으로 제출할 수 있는 새 기능을 도입했습니다. 이 기능은 유사한 요청을 자주 제출할 때 유용합니다. 이 경우 기존 요청을 다시 사용하고 몇 가지 변경한 다음 새 요청으로 제출할 수 있습니다.

이러한 변경 사항으로 다른 사용자가 제출한 요청을 볼 수 있는 사용자도 이러한 요청을 복사하여 새로운 요청으로 제출할 수 있습니다. 요청 큐 프로젝트에서 다음 설정을 업데이트하여 이러한 문제가 발생하지 않도록 할 수 있습니다. 동일한 회사의 사람이 모든 요청에 대해 동일한 권한을 상속합니다.

>[!NOTE]
>
>이 기능을 릴리스하기 전에 큐 항목 없이 요청 큐에 제출된 문제를 복사 및 다시 제출할 수 없습니다.

자세한 내용은 [요청 복사 및 제출](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## 요청 영역의 Submitted 섹션에서 요약 패널 경험이 업데이트되었습니다.

>[!NOTE]
>
>이 기능은 2021년 11월 12일에 미리 보기 환경에서 일시적으로 제거되었습니다. 나중에 다시 추가됩니다.

요약 패널의 가시성과 상호 작용을 개선하기 위해 요청 영역의 제출됨 섹션에서 요약 열기 아이콘에 레이블을 추가했습니다. 이제 레이블이 동적이고 패널이 열려 있는지 여부에 따라 업데이트됩니다.

요청을 먼저 선택하지 않고 요약 패널을 열 때 패널을 열기 전에 사용자에게 항목을 명확히 선택하도록 지시하는 사용자에게 친숙한 이미지가 표시됩니다. 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

이 변경 사항으로 작업, 문제 및 문서에 대한 요약 패널도 업데이트되었습니다. 요약 패널에 대한 자세한 내용은 [요약 개요](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
