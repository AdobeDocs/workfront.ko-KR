---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP 서버 도구
description: Workfront 영역별로 그룹화된 Adobe Workfront MCP 서버를 통해 사용할 수 있는 도구의 참조 목록입니다.
author: Courtney
feature: Get Started with Workfront
source-git-commit: c9177ff889583b086d94214df0320bcd4daff581
workflow-type: tm+mt
source-wordcount: '1578'
ht-degree: 5%

---


# Adobe Workfront MCP 서버 도구

이 문서에서는 [!DNL Adobe Workfront] MCP 서버가 연결된 AI 에이전트 플랫폼에 노출하는 도구를 나열합니다. 플랫폼은 사용자가 Workfront 항목을 검색, 생성, 업데이트 또는 삭제하도록 요청하면 사용자를 대신하여 이러한 도구를 호출합니다.

AI 에이전트 플랫폼을 통해 이러한 도구를 사용하는 방법에 대한 자세한 내용은 [Adobe Workfront MCP 서버 사용](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)을 참조하십시오. 연결 설정 방법에 대한 자세한 내용은 [Adobe Workfront MCP 서버 구성](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)을 참조하십시오.

>[!IMPORTANT]
>
>AI 아젠틱 플랫폼은 Workfront 계정, 액세스 수준 및 오브젝트 권한을 사용하여 Workfront에서 작동합니다. 도구는 Workfront에서 해당 액세스 권한이 있는 경우에만 작동합니다. Adobe은 AI 아젠틱 플랫폼이 Workfront 데이터를 변경했을 때 이에 대한 책임이 없습니다.


## 읽기 및 쓰기 작업

다음 표의 각 도구는 작업 열에서 읽기 또는 쓰기 작업으로 분류됩니다.

* **읽기**: 데이터를 변경하지 않고 Workfront에서 정보를 검색합니다. 예를 들어 프로젝트 찾기, 문서 나열 또는 레코드 세부 정보 가져오기 등이 있습니다.
* **쓰기**: Workfront 데이터를 만들거나 업데이트하거나 삭제합니다. 예: 프로젝트 생성, 레코드 업데이트 또는 보기 삭제

Workfront 관리자는 시스템 환경 설정에서 두 가지 전환을 통해 AI 에이전트 플랫폼에서 사용할 수 있는 도구 범주를 제어합니다.

* **읽기 전용 MCP 도구**(기본적으로 활성화됨)
* **MCP 도구 작성**(기본적으로 사용 안 함)

AI 아젠틱 플랫폼이 Workfront 항목을 찾을 수 있지만 생성, 업데이트 또는 삭제할 수 없는 경우 Workfront 관리자에게 쓰기 작업을 활성화하도록 요청하십시오. 자세한 내용은 *Adobe Workfront MCP 서버 구성*&#x200B;의 [관리 필수 구성 요소](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#admin-prerequisites)를 참조하십시오.

## 승인 도구

### 문서

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 이름별 문서 버전 찾기 | `approvals_find_document_version_by_name` | 파일 이름별로 문서의 현재 버전 ID를 조회합니다. 부분 일치를 지원합니다. | 읽기 |
| 버전 ID로 문서 가져오기 | `approvals_get_document_by_version_id` | 알려진 문서 버전 ID에 대한 문서 세부 정보(이름, 크기, 업로드 날짜, 업로더)를 가져옵니다. | 읽기 |
| 프로젝트별 문서 가져오기 | `approvals_get_documents_by_project` | 각 문서의 현재 버전 ID를 사용하여 Workfront 프로젝트 내의 문서를 나열합니다. | 읽기 |
| 문서 범위 해결 | `approvals_resolve_document_scope` | 프로젝트 또는 폴더를 포함된 문서 버전 ID 목록으로 확장합니다. 프로젝트, 폴더 및 이름별 폴더 범위를 지원합니다. | 읽기 |

<!--
| List AEM-linked folders* | `approvals_list_aem_linked_folders` | Lists Workfront document folders that are linked to Adobe Experience Manager. | Read |
| Send documents to AEM folder* | `approvals_send_documents_to_aem_folder` | Moves one or more Workfront documents to an AEM-linked folder. | Write |

*You must have a native [!DNL Adobe Experience Manager] integration configured in your Workfront instance to use these tools. For more information, see [Overview of Adobe Experience Manager Assets integrations](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/aem-asset-integrations.md).


*Sending documents to an AEM folder is not yet supported for projects on Adobe cloud storage. Support is expected in a future release.

-->

### 승인 작업 과정

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 승인 워크플로 정보 가져오기 | `approvals_get_approval_info` | 문서 버전에 대한 현재 승인 워크플로(단계, 참가자, 상태)를 반환합니다. | 읽기 |
| 승인 워크플로우 만들기 또는 업데이트 | `approvals_create_or_update_approval_workflow` | 문서 버전에 대한 승인 워크플로 단계를 만들거나 업데이트합니다. 선형 및 병렬(그래프) 스테이지 종속성을 지원합니다. | 쓰기 |
| 템플릿에서 승인 만들기 | `approvals_create_approval_from_template` | 기존 템플릿을 사용하여 문서에 대한 승인 워크플로를 만듭니다. | 쓰기 |
| 승인 단계 삭제 | `approvals_delete_approval_stage` | 승인 워크플로에서 이름 또는 위치별로 단일 단계를 삭제합니다. 시작되지 않은 단계만 삭제할 수 있습니다. | 쓰기 |

<!--
| Add and remove participants for an approval in bulk | `approvals_bulk_update_approval_participants`<br>`approvals__submit_bulk_update_approval_participants` | Adds or removes participants to or from multiple approvals at the same time. Currently, bulk updates can be applied only across a single project. Bulk updates across multiple projects will be available in the near future. | Write |
-->

<!--
| Request document approval | `approvals_request_document_approval` | Opens a guided form for requesting approval on a document version (title, approvers/reviewers, optional due date and message). | Write |
-->

### 알림 메시지

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 참가자에게 미리 알림 보내기 | `approvals_send_reminder_to_participants` | 승인 단계의 특정 참가자에게 미리 알림 이메일을 보냅니다. 시작됨, 완료되지 않음, 잠기지 않음 단계에만 작동합니다. | 쓰기 |
| 결정되지 않은 참가자에게 미리 알림 보내기 | `approvals_send_reminder_to_undecided` | 승인 단계에서 결정되지 않은 모든 참가자(알림, 열림 또는 댓글 달기)에게 미리 알림 이메일을 보냅니다. | 쓰기 |

### 승인 템플릿

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 승인 템플릿 나열 | `approvals_list_templates` | 이 Workfront 인스턴스에서 사용할 수 있는 승인 템플릿을 나열합니다. 작성자, 참가자별 필터링 및 용도별 정렬을 지원합니다. | 읽기 |
| 이름별 템플릿 검색 | `approvals_search_template_by_name` | 이름별로 승인 템플릿을 찾습니다(대/소문자를 구분하지 않는 부분 일치). | 읽기 |
| 승인 템플릿 만들기 | `approvals_create_template` | 선형 또는 그래프 기반의 단계 종속성으로 새 승인 템플릿을 만듭니다. | 쓰기 |
| 승인 템플릿 업데이트 | `approvals_update_template` | 구조화된 수정 사항으로 기존 템플릿을 업데이트합니다(참가자 추가 또는 제거, 단계 이름 변경, 기한 설정 등). | 쓰기 |

### 조회 및 사용자

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 현재 사용자 가져오기 | `approvals_get_current_user` | 이름, 사용자 ID, 홈 팀 이름 및 홈 팀 ID를 포함하여 호출하는 사용자의 Workfront ID를 반환합니다. | 읽기 |
| 이름으로 사용자 찾기 | `approvals_find_user_by_name` | 이름으로 Workfront 사용자의 ID를 조회합니다(유사 항목 또는 부분 일치). 이름, ID, 이메일, 제목 및 아바타 URL을 반환합니다. | 읽기 |
| 이름으로 팀 찾기 | `approvals_find_team_by_name` | 이름으로 Workfront 팀의 ID를 조회합니다(유사 항목 또는 부분 일치). | 읽기 |
| 이름으로 프로젝트 찾기 | `approvals_find_project_by_name` | 시스템 전체에서 부분 이름 일치로 Workfront 프로젝트를 조회합니다. | 읽기 |
| 소유자별 프로젝트 가져오기 | `approvals_get_projects_by_owner` | 호출 사용자가 소유자인 Workfront 프로젝트를 나열합니다. | 읽기 |
| Adobe 지역 가져오기 | `approvals_get_adobe_region` | 클라우드 공급자 영역의 Adobe 이름을 반환합니다. | 읽기 |

<!--

## Insights tools

Insights tools retrieve information about Workfront objects.

| Title | Tool name | What it does | Action |
| --- | --- | --- | --- |
| Read documents | `insights_read_docs` | Load the Workfront playbook or domain documentation, such as conditions, status, dates, or field paths. This is the required first step before querying data. | Read |
| Get current user | `insights_get_current_user` | Retrieve your own Workfront identity, including name, ID, and URL. | Read |
| Search fields | `insights_search_fields` | Search for available fields (standard and custom) on projects, tasks, issues, users, portfolios, teams, and so on. | Read |
| Get field paths | `insights_get_field_paths` | Resolve dot-notation field paths for entities, required by the data query tool. | Read |
| Find ID by name | `insights_find_id_by_name` | Look up the ID of any Workfront object by name, such as projects, tasks, users, portfolios, and so on. | Read |
| Find Workfront data | `insights_find_workfront_data` | Find, filter, count, sort, and aggregate Workfront data. This is the main query and report tool. | Read |
| Summarize object | `insights_summarize_object` | Fetch and summarize a single Workfront object by ID. | Read |
| List entities | `insights_list_entities` | List all Workfront object types available to query. | Read |

-->

## 계획 도구

>[!IMPORTANT]
>
>* Workfront Planning에서 MCP를 사용하려면 귀사는 Adobe Workfront Planning이 포함된 Workfront 패키지에 있어야 합니다.

### 작업 영역

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 작업 영역 가져오기 | `planning_get_workspace` | ID 또는 별칭별로 작업 공간의 전체 세부 정보를 검색합니다. | 읽기 |
| 작업 영역 목록 가져오기 | `planning_get_workspace_list` | 커서 기반 페이지 매김 기능이 있는 사용 가능한 모든 작업 영역을 나열합니다. | 읽기 |
| 작업 영역 만들기 | `planning_create_workspace` | 레코드 유형, 필드 및 데이터를 구성하는 빈 작업 영역을 새로 만듭니다. | 쓰기 |
| 템플릿에서 작업 영역 만들기 | `planning_create_workspace_from_template` | 기존 템플릿을 사용하여 미리 채워진 새 작업 공간을 만듭니다. | 쓰기 |
| 작업 영역 업데이트 | `planning_update_workspace` | 작업 영역(이름, 설명, 아이콘, 섹션 또는 소유자)을 부분적으로 업데이트합니다. | 쓰기 |
| 작업 영역 삭제 | `planning_delete_workspace` | 작업 영역과 모든 해당 데이터를 영구적으로 삭제합니다. | 쓰기 |
| 작업 영역을 템플릿으로 변환 | `planning_convert_workspace_to_template` | 기존 작업 영역을 재사용 가능한 템플릿으로 저장합니다(관리자 필요). | 쓰기 |
| 작업 영역 공유 가져오기 | `planning_get_workspace_sharing` | 작업 공간에 대한 현재 공유 및 권한 구성을 반환합니다. | 읽기 |
| 작업 영역 공유 수정 | `planning_modify_workspace_sharing` | 작업 영역에 액세스할 수 있는 사용자와 사용 권한 수준을 업데이트합니다. | 쓰기 |

### 레코드 유형

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 레코드 유형 가져오기 | `planning_get_record_type` | 필드 및 보기를 포함하여 레코드 종류의 전체 세부 정보를 가져옵니다. | 읽기 |
| 레코드 유형 만들기 | `planning_create_record_types` | 작업 영역 섹션 내에 하나 이상의 레코드 유형을 만듭니다. | 쓰기 |
| 레코드 유형 업데이트 | `planning_update_record_type` | 레코드 유형의 이름, 설명, 아이콘 또는 색상을 부분적으로 업데이트합니다. | 쓰기 |
| 레코드 유형 삭제 | `planning_delete_record_type` | 레코드 종류 및 해당 레코드, 필드, 보기를 영구적으로 삭제합니다. | 쓰기 |
| 목록 글로벌 레코드 유형 | `planning_list_global_record_types` | 현재 사용자가 볼 수 있는 중앙에서 정의된(전역) 모든 레코드 유형을 나열합니다. | 읽기 |
| 목록 추가 가능한 글로벌 레코드 유형 | `planning_list_addable_global_record_types` | 특정 작업 영역에 추가할 수 있는 글로벌 레코드 유형을 나열합니다. | 읽기 |
| 작업 영역에 글로벌 레코드 유형 추가 | `planning_add_global_record_type_to_workspace` | 글로벌 레코드 유형을 지정된 작업 공간에 연결합니다. | 쓰기 |
| 작업 영역에서 글로벌 레코드 유형 제거 | `planning_remove_global_record_type_from_workspace` | 작업 영역에서 글로벌 레코드 유형의 연결을 해제합니다. 해당 작업 영역에서 모든 레코드를 삭제합니다. | 쓰기 |
| 외부 레코드 작업 영역 가져오기 | `planning_get_external_record_workspaces` | 특정 외부 레코드에 연결된 작업 공간 및 레코드 유형을 찾습니다. | 읽기 |
| 레코드 유형 공유 가져오기 | `planning_get_record_type_sharing` | 특정 레코드 종류에 대한 공유 및 권한을 반환합니다. | 읽기 |
| 레코드 유형 공유 수정 | `planning_modify_record_type_sharing` | 레코드 종류 및 권한 수준에 액세스할 수 있는 사용자를 업데이트합니다. | 쓰기 |

### 레코드

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 레코드 가져오기 | `planning_get_record` | 단일 레코드의 전체 세부 정보를 ID로 검색합니다. | 읽기 |
| 레코드 검색 | `planning_search_records` | 레코드 종류 내의 레코드를 검색하고 필터링합니다. | 읽기 |
| 일괄 레코드 작업 | `planning_bulk_record_actions` | 단일 요청에서 여러 레코드를 생성, 업데이트, 삭제 또는 복원합니다. | 쓰기 |
| 연결 레코드 만들기 | `planning_create_connection_record` | 연결된 외부 시스템(예: Workfront 프로젝트)에 새 레코드를 만듭니다. | 쓰기 |
| 레코드 순서 업데이트 | `planning_update_records_order` | 레코드 유형 내의 레코드 표시 순서를 변경합니다. | 쓰기 |
| 레코드 변경 로그 가져오기 | `planning_get_record_change_log` | 레코드에 대한 필드 수준의 편집 기록을 반환합니다. | 읽기 |
| 레코드 공유 가져오기 | `planning_get_record_sharing` | 특정 레코드에 대한 공유 구성을 반환합니다. | 읽기 |
| 레코드 공유 수정 | `planning_modify_records_sharing` | 하나 이상의 레코드에 액세스할 수 있는 사용자 및 권한 수준을 업데이트합니다. | 쓰기 |

### 필드

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 필드 가져오기 | `planning_get_field` | ID별로 필드에 대한 전체 세부 정보 및 값 스키마를 검색합니다. | 읽기 |
| 필드 만들기 | `planning_create_fields` | 레코드 유형에 하나 이상의 필드(열)를 추가합니다. | 쓰기 |
| 필드 업데이트 | `planning_update_field` | 필드의 이름, 설명, 옵션 또는 구성을 부분적으로 업데이트합니다. | 쓰기 |
| 필드 삭제 | `planning_delete_field` | 레코드 유형에서 필드와 모든 해당 데이터를 영구적으로 제거합니다. | 쓰기 |

### 보기 횟수

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 보기 가져오기 | `planning_get_view` | ID별 보기의 전체 세부 정보를 반환합니다. | 읽기 |
| 보기 만들기 | `planning_create_view` | 레코드 유형에 대한 새 테이블, 타임라인 또는 달력 보기를 만듭니다. | 쓰기 |
| 보기 업데이트 | `planning_update_view` | 기존 보기의 구성, 필터 또는 정렬을 부분적으로 업데이트합니다. | 쓰기 |
| 보기 삭제 | `planning_delete_view` | 보기를 영구적으로 삭제합니다(레코드는 영향을 받지 않음). | 쓰기 |
| 보기 공유 가져오기 | `planning_get_view_sharing` | 특정 보기에 대한 공유 구성을 반환합니다. | 읽기 |
| 보기 공유 수정 | `planning_modify_view_sharing` | 보기에 액세스할 수 있는 사용자와 사용 권한 수준을 업데이트합니다. | 쓰기 |

### 템플릿

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 템플릿 목록 가져오기 | `planning_get_template_list` | 요약 정보와 함께 사용 가능한 모든 작업 영역 템플릿을 나열합니다. | 읽기 |
| 템플릿 가져오기 | `planning_get_template` | 특정 템플릿의 전체 세부 정보를 ID로 검색합니다. | 읽기 |

### 검색 및 유틸리티

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 리소스 검색 | `planning_search_resources` | 작업 영역, 레코드 유형 및 보기를 이름별로 검색합니다. | 읽기 |
| 공유 데이터 검색 | `planning_search_sharing_data` | 공유 및 권한을 위해 이름별로 사용자, 그룹, 팀, 역할 및 회사를 찾습니다. | 읽기 |
| 사용자 검색 | `planning_search_users` | 페이지 매김이 지원되는 사용자를 검색합니다. | 읽기 |

## 워크플로 도구

워크플로 도구는 AI 아젠틱 플랫폼이 Workfront 개체(프로젝트, 작업, 문제, 시간, 과제, 프로그램, 포트폴리오 등)와 작업하는 데 사용하는 일반적인 목적의 작업입니다.

| 제목 | 도구 이름 | 기능 | 액션 |
| --- | --- | --- | --- |
| 오브젝트 검색 | `workflow_search_any_object` | 유연한 필터 매개 변수, 순서 지정 및 페이지 매김을 사용하여 Workfront 개체를 검색합니다. | 읽기 |
| 개체 만들기 | `workflow_create_any_object` | 프로젝트, 작업, 문제, 시간, 할당, 프로그램 또는 포트폴리오와 같은 새 Workfront 개체를 만듭니다. | 쓰기 |
| 개체 업데이트 | `workflow_update_any_object` | 기존 Workfront 개체의 필드를 업데이트합니다. | 쓰기 |
| 오브젝트 삭제 | `workflow_delete_any_object` | ID별로 Workfront 개체를 삭제합니다. 작업을 수행하기 전에 명시적인 사용자 확인이 필요합니다. | 쓰기 |
| 필드 이름 확인 | `workflow_resolve_field_names_any_object` | 사용자가 제공한 필드 이름이나 레이블을 기본 Workfront API 필드 이름으로 변환하여 AI 에이전트 플랫폼이 정확한 요청을 작성할 수 있도록 합니다. | 읽기 |

## 도구 업데이트 방법

Adobe이 Workfront MCP 서버의 새 버전을 출시하면 AI 에이전트 플랫폼은 업데이트된 도구 세트를 자동으로 사용합니다. 다시 연결하거나 변경할 필요가 없습니다.



## 추가 툴 출시 예정

향후 Workfront MCP 서버에 다음 도구를 추가하기 위해 노력하고 있습니다.

* 댓글
* 보드

