---
title: 21.4 프로젝트 개선 사항
description: 21.4 프로젝트 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 21.4 프로젝트 개선 사항

이 페이지에서는 미리 보기 환경에 대한 21.4 릴리스로 수행된 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2021년 10월 4일이 있는 프로덕션 환경에서 사용할 수 있습니다.

21.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [21.4 릴리스 개요](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 업데이트에 이미지 포함

이제 개체의 업데이트 탭에서 도구 모음에서 이미지 아이콘을 클릭하여 이미지를 추가할 수 있습니다. 이미지를 업데이트 영역으로 끌어다 놓을 수도 있습니다. 이미지 아이콘을 보려면 Workfront 관리자가 이미지 추가를 활성화해야 합니다.

업데이트 및 회신 모두에 이미지를 추가할 수 있습니다. 업데이트의 이미지 축소판은 수신자가 브라우저에서 이미지를 미리 보거나 다운로드할 수 있음을 나타내고, 이메일 및 인앱 알림은 이미지에 업데이트가 연결되어 있음을 나타냅니다.

이전에는 Workfront에서 이미지를 공유할 수 있는 유일한 방법은 개체를 문서로 연결하는 것입니다. 업데이트 탭에 추가된 이미지는 해당 탭에서만 사용할 수 있으며 문서 탭에서는 사용할 수 없습니다.

자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Workfront 사용자가 업데이트에 이미지를 포함하려면 먼저 Adobe Workfront 관리자가 이 기능을 활성화해야 합니다. 자세한 내용은 다음에 설명된 대로 [사용자 업데이트에 대한 환경 설정 구성](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## 스마트 할당에 대한 알고리즘 업데이트

스마트 할당을 만들 때 사용되는 알고리즘을 개선했습니다. 새로운 개선 사항을 통해 Workfront은 로그인한 사용자가 작업 및 문제를 할당할 때 제안하기 위해 30개의 최근 할당을 봅니다. 추천 목록에는 최대 50명의 사용자가 포함될 수 있습니다.

이 개선 사항 전에 Workfront에서는 사용자를 제안할 때 상위 작업 및 해당 할당과 관련된 기타 사용자 속성에 대한 지정을 고려했습니다.

스마트 할당에 대한 자세한 내용은 [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## 템플릿에서 프로젝트를 작성할 때의 새로운 경험

Workfront을 새로운 Workfront 환경과 일관되게 사용하기 위해 Adobe에서는 템플릿에서 프로젝트를 작성할 수 있는 인터페이스를 다시 디자인했습니다. 템플릿을 사용하여 프로젝트를 만드는 기능은 변경되지 않았습니다. 그러나 이러한 새로 다시 디자인된 인터페이스의 일부 개선 사항은 다음과 같습니다.

* 첨부 전에 템플릿 정보 미리 보기
* 프로젝트 작성 프로세스 중에 즐겨찾기 목록에 템플릿 추가

프로젝트 뿐만 아니라 템플릿 영역에서 프로젝트를 만들 때 둘 다 프로젝트를 만들기 위한 인터페이스를 업데이트했습니다.

자세한 내용은 [템플릿을 사용하여 프로젝트 만들기](../../../manage-work/projects/create-projects/create-project-from-template.md).

## 프로젝트에 템플릿을 첨부할 때 새로운 경험

>[!NOTE]
>
>이 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.

Workfront을 새로운 Workfront 환경과 일관되게 사용하기 위해 프로젝트에 템플릿을 첨부하기 위한 인터페이스를 다시 디자인했습니다. 템플릿 첨부 기능은 변경되지 않았습니다. 그러나 다음과 같은 내용을 포함하여 새로 디자인된 인터페이스의 몇 가지 개선 사항이 있습니다.

* 첨부 전에 템플릿 정보 미리 보기
* 첨부 프로세스 중에 즐겨찾기 목록에 템플릿을 추가합니다
* 하나의 연속 페이지에서 템플릿 및 프로젝트 설정을 관리하기 위한 모든 옵션을 봅니다

자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## 작업에 대한 통합 기간 및 기간 단위 값

보다 깔끔하고 간소화된 사용자 경험을 위해 기간 필드의 값을 기간 단위와 병합했습니다. 이 개선 사항 전에 기간 필드 뒤에 별도의 드롭다운 필드에 시간 단위가 표시됩니다.

[작업 세부 정보], [작업 편집] 및 [새 작업] 상자의 [기간] 필드 외에도 이 환경과 일치하도록 다음 필드도 업데이트하고 있습니다.

* 고급 할당을 수행할 때 기간 필드
* 작업을 만들거나 편집할 때 지연 평준화 필드
* 반복 작업을 만들 때 빈도 필드(곧 사용 가능)
* 이전 사용자를 추가할 때 지연 필드(곧 사용 가능)

자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## 프로젝트에서 인라인 문제 추가 비활성화

사용자가 문제 양식을 작성하여 프로젝트에 문제를 추가할 때 정확한 정보를 제공할 수 있도록 하기 위해 프로젝트 또는 해당 작업에 인라인 문제를 추가할 수 있는지 여부를 관리할 수 있는 새 설정을 도입했습니다. 이 설정은 프로젝트 편집 상자의 새 문제 설정 영역에서 기본적으로 활성화됩니다. 비활성화하면 프로젝트의 문제 섹션에 있는 추가 문제 옵션이 표시되므로 사용자가 목록에 문제를 더 이상 추가할 수 없습니다. 사용자는 여전히 문제 섹션의 새 문제 옵션을 사용하거나 프로젝트에 대해 구성된 경우 요청 큐를 사용하여 프로젝트에 문제를 추가할 수 있습니다.

>[!NOTE]
>
>이 설정은 새 Workfront 경험에서만 사용할 수 있습니다. Workfront Classic에서 작업하는 사용자는 새 Workfront 경험에서 작업하는 사용자가 이 설정을 프로젝트에 대해 사용하지 않도록 설정하더라도 프로젝트 또는 해당 작업에 인라인 문제를 추가할 수 있습니다.

자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

## 확인란 및 라디오 단추에 대한 사용자 지정 필드 표시 개선 사항

사용자 지정 양식에서 확인란 및 라디오 단추 옵션을 보고 선택하는 작업이 이제 쉬워졌습니다. 여러 확인란 또는 라디오 단추 옵션이 있는 사용자 지정 필드가 이제 페이지의 여러 열에 표시됩니다. 이전에는 단일 열에 표시되었지만 양식을 채우는 사용자에게 추가 스크롤이 필요합니다.

이는 사용자 지정 양식에서 필드를 배치하는 방법에 따라 다릅니다. 확인란 또는 라디오 단추 필드를 사용하여 동일한 행에 다른 필드를 배치하는 경우 옵션에는 단일 열에 표시할 충분한 수평 공간만 있을 수 있습니다.

사용자 지정 양식 채우기에 대한 자세한 내용은 [사용자 지정 양식 필드에서 정보 편집](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

사용자 지정 양식에서 확인란 또는 라디오 단추 필드를 만드는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 및 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) 기사 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

