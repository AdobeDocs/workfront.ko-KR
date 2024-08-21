---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 개별 하위 개체 복원
description: 이 문서에서는 30일 이전에 Adobe Workfront 프로덕션 또는 미리보기 환경에서 삭제된 개별 하위 객체를 복구하는 데 도움을 받는 방법을 설명합니다.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# 개별 하위 개체 복원

이 문서에서는 30일 이전에 Adobe Workfront 프로덕션 또는 미리보기 환경에서 삭제된 개별 하위 객체를 복구하는 데 도움을 받는 방법을 설명합니다.

[삭제된 항목 복원](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)에 설명된 대로 Workfront 관리자는 각 Workfront 인스턴스의 프로젝트, 작업, 문제 및 문서를 복원할 수 있습니다. 하지만 Workfront 데이터베이스 팀만 작업, 문제, 문서, 사용자 정의 양식, 시간 및 메모와 같은 개체를 상위 개체와 독립적으로 복원할 수 있습니다.

라이브 환경의 데이터는 미리보기 샌드박스에서 최대 7일 동안 사용할 수 있습니다. 즉, 다음 방법을 사용하여 미리보기 샌드박스 환경에서 독립형 데이터를 내보낼 수 있습니다.

* 킥스타트
* 보고서 작성 및 결과 내보내기

Workfront에서 데이터를 내보내는 방법에 대한 자세한 내용은 [데이터 내보내기](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)를 참조하십시오.

다음과 같은 방법으로 내보낸 데이터를 가져올 수 있습니다.

* 수동으로(내보낸 보고서를 사용하는 경우)
* 일괄적으로, 킥스타트를 사용하는 경우

  킥스타트를 사용하여 Workfront으로 데이터를 가져오는 방법에 대한 자세한 내용은 [킥스타트 템플릿을 사용하여 Adobe Workfront으로 데이터 가져오기](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)를 참조하십시오.

주말 유지 관리 기간 동안 미리보기 샌드박스 환경이 새로워졌습니다.

미리 보기 샌드박스 환경의 유지 관리 기간에 대한 자세한 내용은 [Adobe 상태 사이트](https://status.adobe.com)를 참조하십시오.

>[!IMPORTANT]
>
>문서는 이러한 복원 방법에 대한 예외입니다. 미리보기 환경에서 수동으로 다운로드하여 프로덕션 환경에 다시 업로드할 수 있습니다. 문서를 일괄적으로 다운로드하고 업로드하려면 Workfront에서 데이터 복원을 요청해야 합니다.

## 데이터 복원에 필요한 정보

삭제된 개체를 데이터베이스 팀에서 복원해야 한다고 판단했으면 해당 개체에 대해 가지고 있는 만큼 많은 정보를 수집합니다. 데이터베이스 관리자가 객체를 찾아 복원을 시작하려면 다음 정보가 필요합니다.

* 개체 이름
* 오브젝트 유형 (작업, 문제, 프로젝트 등)
* 예상 삭제 날짜 및 시간
* 개체 GUID(가능한 경우)

  개체의 GUID를 찾을 때 다음 정보를 참조하십시오.

   * GUID는 개체(할당 대상, 댓글 등)와 상호 작용하여 트리거된 전자 메일 알림을 참조하여 찾을 수 있습니다.
   * URL 끝에 있는 GUID의 예: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

이 정보를 수집했거나 지원이 필요한 경우 844-306-HELP(4357)로 고객 지원 팀에 문의하거나 온라인으로 티켓을 제출하십시오.

## 데이터 복원 프로세스

1. 고객 지원 팀이 귀하의 정보를 받으면 고객 지원 팀으로 에스컬레이션합니다.
1. 고객 지원 팀이 데이터베이스 팀에 연락합니다.
1. 데이터베이스 팀이 복원 중인 데이터를 검토할 수 있게 되면 ETA에 대한 보다 정확한 예상 값을 제공할 수 있습니다. 복원은 일반적으로 3일이 걸리지만 복원 중인 데이터의 유형 및 볼륨에 따라 더 오래 걸릴 수 있습니다.
1. 데이터베이스 팀은 복원된 데이터를 검토할 수 있는 미리보기 샌드박스 환경으로 정보를 복원합니다. 고객 지원 팀에서 미리보기 샌드박스에서 데이터를 찾을 수 있는 시기를 알려드립니다.
1. 샌드박스에서 복원이 만족스러우면 고객 지원 팀에 알려주면 데이터베이스 팀에 연락하여 운영 환경에 데이터를 복원할 수 있음을 알립니다.
1. 요청이 종료되기 전에 복원된 데이터를 검토할 수 있습니다.
