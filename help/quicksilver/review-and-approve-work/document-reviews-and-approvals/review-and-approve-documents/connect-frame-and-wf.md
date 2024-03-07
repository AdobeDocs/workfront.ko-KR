---
product-area: projects
navigation-topic: approvals
title: Workfront 및 Frame.io 연결
description: Workfront은 검토 및 승인 프로세스에서 Frame.io를 사용하여 원하는 곳에서 사람들을 만나고 있습니다. 프로젝트 관리 및 승인 프로세스는 Workfront에서 관리되며 검토 프로세스는 Frame.io에서 수행됩니다.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 2c1945cdc9f923ea7fdc750f69eeba2a026571ac
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---


# Workfront 및 Frame.io 연결

>[!IMPORTANT]
>
>이 문서의 내용은 특정 계정에만 사용할 수 있는 업데이트된 문서 승인 기능에 적용됩니다. 표준 승인 프로세스에 대한 정보는 다음 목록에 있는 문서를 참조하십시오. [작업 승인](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Workfront은 검토 및 승인 프로세스에서 Frame.io를 사용하여 원하는 곳에서 사람들을 만나고 있습니다. 프로젝트 관리 및 승인 프로세스는 Workfront에서 관리되며 검토 프로세스는 Frame.io에서 완료됩니다. 통합을 성공적으로 설정하려면 다음 섹션을 모두 완료해야 합니다.

* [Workfront 그룹을 Frame.io 팀에 연결](#connect-a-workfront-group-to-a-frameio-team)
* [Workfront 프로젝트 만들기 및 연결된 그룹 추가](#create-a-workfront-project-and-add-a-connected-group)



## 액세스 요구 사항

* 이 문서에 설명된 기능을 사용하려면 조직을 수동으로 온보딩해야 합니다. 자세한 내용은 [Adobe Workfront 및 Frame.io 기본 통합 알파: 개요](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).


## Workfront 그룹을 Frame.io 팀에 연결

이 기능은 5월에 일반 출시될 수 있도록 적극적으로 개선되고 있습니다.

### 전제 조건

* Workfront 그룹에 매핑할 Frame.io 팀을 만듭니다.
* 팀에 대한 API 개발자 토큰을 찾습니다. 자세한 내용은 [개발자 토큰](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) Frame.io 개발자 사이트에서 참조하십시오.

### Workfront 그룹을 Frame.io 팀에 연결

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**.
1. 기존 그룹을 선택하거나 **그룹 만들기**.
1. 왼쪽 패널에서 **Frame.io에 연결**.
   ![](assets/connect-frame-group.png)
1. API 개발자 토큰을 입력합니다.
1. 클릭 **연결 시작**.
1. (조건부) 둘 이상의 Frame.io 계정의 관리자인 경우 사용할 계정을 선택합니다.

## Workfront 프로젝트 만들기 및 연결된 그룹 추가

Workfront 그룹을 Frame.io 팀에 연결한 후에는 연결된 그룹으로 프로젝트를 만들어야 합니다.

### 전제 조건

* 이전 섹션에서 설명한 대로 Frame.io 팀에 연결된 Workfront 그룹이 있어야 합니다.

### Workfront 프로젝트 만들기 및 연결된 그룹 추가

{{step1-to-projects}}

1. 새 프로젝트를 처음부터 만들거나 템플릿을 만듭니다. 프로젝트를 만드는 방법에 대한 자세한 내용은 [프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. 왼쪽 패널에서 찾기 **프로젝트 세부 정보**.

1. 다음 찾기 **그룹** 화면의 오른쪽에 있는 필드를 클릭하고 Default 그룹을 제거합니다.

1. 드롭다운 메뉴에서 원하는 그룹을 찾습니다. Frame.io와 연결된 그룹은 Frame.io 아이콘을 표시합니다.
   ![](assets/add-frame-group.png)

1. 다른 프로젝트 구성을 변경합니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

1. 다음 섹션으로 이동합니다.

### 작업을 추가하고 통합 상태를 활성으로 설정

>[!NOTE]
>
>하위 작업은 현재 연결된 Frame.io 프로젝트에서 지원되지 않습니다.


1. Frame.io에서 채워야 하는 작업을 만듭니다.

1. 필요한 작업을 선택한 다음 **편집**.

1. 다음으로 스크롤 **사용자 지정 Forms** 및 Frame.io 통합 양식을 찾습니다.

   >[!IMPORTANT]
   >
   >이 양식을 표시하려면 연결된 Frame.io 그룹을 프로젝트 세부 정보 영역에 할당해야 합니다. 자세한 내용은 [Workfront 프로젝트 만들기 및 연결된 그룹 추가](#create-a-workfront-project-and-add-a-connected-group) 이 문서에서.


1. 활성화 **이 작업의 통합 상태** 확인란 및 선택 **활성**.
   ![](assets/frame-custom-form.png)

1. 클릭 **변경 내용 저장**. 프로젝트 이름 옆에 Frame.io 아이콘이 표시됩니다.

1. 작업에 사용자 또는 팀을 할당합니다.

   >[!NOTE]
   >
   >작업에 추가된 사용자 또는 팀은 Frame.io 프로젝트에도 추가됩니다.

1. 프로젝트 문서 영역에서 모든 문서 또는 Creative Brief 를 업로드합니다.

프로젝트가 여전히 연결되어 있지 않습니다. 다음 섹션으로 계속 진행하여 통합을 완료해야 합니다.

### Frame.io에서 프로젝트 활성화

1. 다음에서 프로젝트 상태 변경 **계획 수립** 끝 **현재** 또는 현재 사용자 지정 상태입니다. 이렇게 하면 통합이 완료되고 Frame.io의 프로젝트, 작업 및 문서가 생성됩니다.

프로젝트 이름 옆에 있는 Frame.io 아이콘은 통합이 성공했음을 나타내는 보라색으로 바뀝니다. 사용자는 Frame.io 프로젝트에 초대하는 이메일을 받게 됩니다.

>[!IMPORTANT]
>
>프로젝트가 Frame.io에 대해 연결되면 프로젝트 그룹의 변경 사항이 Frame.io에 반영되지 않습니다.


