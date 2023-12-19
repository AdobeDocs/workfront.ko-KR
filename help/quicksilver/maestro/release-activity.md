---
title: Adobe Maestro 릴리스 활동
description: 현재 일부 Workfront 고객은 Adobe Maestro를 사용할 수 있습니다. 이 문서를 자주 검토하여 Adobe Maestro에 대해 최근 릴리스된 기능에 대해 알아보십시오.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: bccd29ce284ca247b51971369102b5992061afb0
workflow-type: tm+mt
source-wordcount: '2796'
ht-degree: 0%

---

# Adobe Maestro 릴리스 활동

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro/maestro-overview.md).

이 문서에서는 2023년 5월 22일 Maestro Closed Beta 프로그램 출시 이후 출시된 기능을 나열합니다.

릴리스된 기능은 릴리스 순서대로 나열되며 가장 최근의 기능이 먼저 릴리스됩니다. Maestro Closed Beta 프로그램에 참여하는 고객은 미리보기 및 프로덕션 환경의 모든 기능에 액세스할 수 있습니다.

>[!IMPORTANT]
>
>아래 섹션에서 참조하는 설명서는 기능이 프로덕션에 릴리스된 후 잠시 사용할 수 있습니다.

이 섹션에는 2023년 5월 22일 Maestro Closed Beta 프로그램 출시 후 출시된 기능 및 패치가 나열되어 있습니다.

기능은 매주 릴리스되고 릴리스 순서대로 나열되며, 가장 최근의 기능이 먼저 나열됩니다. Maestro Closed Beta 프로그램에 참여하는 고객은 미리보기 및 프로덕션 환경의 모든 기능에 액세스할 수 있습니다.

<!--
## Week of November 27, 2023

### Maestro permissions for users and groups

Production: November 28, 2023

>[!IMPORTANT]
>
>This functionality is not yet available in Preview.

You can now share a workspace with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit in a Maestro workspace. After you share permissions to a workspace, users have permissions to the record types, records, and fields in that space.

The following are the permissions levels for Maestro workspaces:  

* None: Users cannot access any workspaces in Maestro, even if the Maestro area is shared with them through a layout template. 

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces ones shared with them.  

* Manage: Users can create, edit, and delete record types, records, and fields in workspaces that are shared with them. They cannot create workspaces.  

Only Workfront administrators can create, edit, or delete workspaces and all information associated with them.  

For more information, see [Grant access to Adobe Maestro](../maestro/access/grant-access.md) and [Overview of sharing permissions in Adobe Maestro](../maestro/access/sharing-permissions-overview.md). -->

## 2024년 12월 18일이 있는 주

### 세부 정보 페이지에서 레코드에 대한 주석 추가

모든 고객을 위한 미리보기 및 프로덕션: 2023년 12월 18일

>[!NOTE]
>
>프로덕션 환경에서는 2024년 1월 릴리스에서 다음 기능을 사용할 수 있습니다.
>
>* 댓글 검색
>
>* 이미지 복사 및 붙여넣기
>
>* 이미지 드래그 앤 드롭
>
>자세한 내용은 [2024년 1분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

이제 세부 정보 페이지에서 레코드를 보는 동안 주석을 추가하거나 다른 레코드에 회신하여 개별 레코드에 대해 다른 사용자와 공동 작업을 할 수 있습니다.

Maestro 레코드에 대한 댓글 달기 환경은 Workfront 객체에 대한 새로운 댓글 달기 환경과 일치합니다.

자세한 내용은 [레코드 주석 관리](/help/quicksilver/maestro/records/manage-record-comments.md).

## 2023년 12월 11일 주

### 레코드 유형의 표 보기에서 기본 필드 업데이트

미리보기 및 프로덕션: 2023년 12월 14일

이제 Maestro 테이블 보기의 첫 번째 열에 표시할 필드를 선택할 수 있습니다. 이제 이 필드를 기본 필드라고 합니다.

이 개선 이전에는 레코드의 이름 필드가 항상 테이블 보기의 첫 번째 열에 표시되므로 다른 위치에 배치할 수 없었습니다.

이 개선 사항을 통해 다음 사항에 주목하십시오.

* 이름 열이나 필드는 기본적으로 여전히 테이블의 첫 번째 열입니다.

* 다음 유형의 필드를 기본 필드로 선택하고 첫 번째 열의 이름 필드를 바꿀 수 있습니다.

   * 한 줄 텍스트

   * 숫자

   * 공식

     >[!NOTE]
     >
     >수식 유형 필드는 나중에 릴리스됩니다.

* 테이블 뷰의 기본 필드는 항상 동결되며 다른 필드를 기본 필드로 설정하지 않는 한 이동할 수 없습니다.

* 기본 필드가 아닌 열 헤더에서 기본 필드를 변경할 수 있습니다.

* 레코드 유형의 모든 테이블 보기에는 선택하는 기본 필드가 동일합니다.

자세한 내용은 [테이블 보기 관리](/help/quicksilver/maestro/views/manage-the-table-view.md).


### Maestro 레코드와 Adobe Experience Manager Assets 연결

미리보기 릴리스: 2023년 12월 14일

프로덕션 릴리스: 2023년 12월 15일로 예정됨

>[!IMPORTANT]
>
>Maestro 레코드를 Adobe Experience Manager Assets에 연결하려면 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.
>
>Adobe Admin Console 온보딩에 대한 질문이 있는 경우 [통합 경험 FAQ Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


이제 Maestro 레코드 유형과 Adobe Experience Manager Assets 간 연결을 설정할 수 있습니다.

연결을 설정하면 이 업데이트에서 다음 기능을 사용할 수 있습니다.

* 액세스 권한이 있는 Experience Manager Assets의 특정 저장소에서 Experience Manager 에셋 및 폴더를 Maestro 레코드에 연결할 수 있습니다. 이 프로세스에서 에셋 필드를 마에스트로 필드에 연결할 수 있습니다.

* Maestro 사용자는 연결된 자산의 이름과 Maestro에 있는 연결된 필드의 값을 볼 수 있습니다

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* 연결된 레코드 필드에서 Maestro 레코드의 테이블 보기에서 에셋 이름을 클릭하고 에셋 썸네일과 여러 키 필드가 있는 팝업 창을 볼 수 있습니다. 팝업 창에서 Experience Manager의 에셋 뷰어로 이동하여 에셋에 대한 모든 세부 정보를 볼 수 있습니다.

자세한 내용은 [레코드 유형 연결](/help/quicksilver/maestro/architecture/connect-record-types.md).

## 2023년 12월 4일 주

### 사람 유형 및 연결된 레코드 필드에 대해 마에스트로 표 보기의 한 필드에서 다른 필드로 정보를 복사하여 붙여넣습니다.

미리보기 및 프로덕션: 2023년 12월 5일

이제 Maestro 레코드 유형 표 보기에서 한 필드의 정보를 같은 유형의 다른 필드로 복사하여 붙여넣을 수 있습니다. 이 기능은 이제 다음 유형의 필드에 대해 지원됩니다.

* 사용자
* 연결된 레코드 필드

다음 사항을 고려하십시오.

* 여러 값을 표시하는 필드에 대해 한 필드에서 다른 필드로 필드 값을 복사하여 붙여넣을 수 있습니다.

* 정보를 붙여넣은 필드와 동일한 유형의 마에스트로 필드 이외의 다른 소스에서 정보를 복사할 수 없습니다.

* 레코드의 세부 정보 영역에 표시되는 필드의 필드 값을 복사하여 붙여넣을 수 없습니다.

자세한 내용은 [레코드 편집](../maestro/records/edit-records.md).

연결된 필드에 대한 자세한 내용은 [레코드 유형 연결](../maestro/architecture/connect-record-types.md).

## 2023년 11월 27일 주

### Maestro 표 보기의 한 필드에서 다른 필드로 정보를 복사하여 붙여넣기

미리보기 및 프로덕션: 2023년 11월 28일

이제 Maestro 레코드 유형 표 보기에서 한 필드의 정보를 같은 유형의 다른 필드로 복사하여 붙여넣을 수 있습니다.

다음 사항을 고려하십시오.

* 정보를 붙여넣은 필드와 동일한 유형의 마에스트로 필드 이외의 다른 소스에서 정보를 복사할 수 없습니다.

* 레코드의 세부 정보 영역에 표시되는 필드의 필드 값을 복사하여 붙여넣을 수 없습니다.

* 다음 필드 유형에 대한 필드 값을 복사하여 붙여넣을 수 없습니다.

   * 사용자

   * 시스템 필드

   * 레코드 연결 결과로 생성된 연결된 필드

자세한 내용은 [레코드 편집](../maestro/records/edit-records.md).

## 2023년 11월 6일 주

### 테이블 보기에 대한 그룹화

미리보기 및 프로덕션: 2023년 11월 7일

이제 레코드 유형 페이지의 표 보기에서 레코드를 그룹화할 수 있습니다. Maestro 인터페이스에서 3개의 고유한 필드별로 그룹화할 수 있습니다 <!--checking into this for now: and by four fields when using the API-->.

자세한 내용은 [표 보기 관리](../maestro/views/manage-the-table-view.md).

## 2023년 10월 30일 주

### 레코드를 만들었거나 마지막으로 수정한 사람 또는 날짜를 캡처하는 사용자 및 날짜 필드의 새 필드 유형

미리보기 및 프로덕션: 2023년 10월 30일

Maestro 레코드에 대해 다음 필드 유형을 도입했습니다.

* 제작자:

* 제작 일자

* 마지막 수정자

* 마지막 수정일

이러한 필드 유형에서 생성된 필드의 필드 값은 읽기 전용이며 레코드를 만들거나 마지막으로 수정한 사용자의 이름 또는 레코드를 만들거나 마지막으로 수정한 날짜를 캡처합니다.

자세한 내용은 [필드 만들기](../maestro/fields/create-fields.md).

### Maestro 레코드에서 Workfront 오브젝트 탐색

미리보기 및 프로덕션: 2023년 10월 31일

이제 Maestro의 다음 영역에서 Workfront 개체 페이지를 열 수 있습니다.

* 읽기 전용으로 연결된 Workfront 개체 레코드 테이블 보기

* 읽기 전용 Workfront 개체 레코드 세부 정보 페이지

자세한 내용은 [레코드 연결](../maestro/records/connect-records.md).

### 표 보기에서 탐색 기능이 개선됨

미리보기 및 프로덕션: 2023년 11월 2일

레코드 유형 페이지의 표 보기에서 탐색을 개선했습니다.

다음은 몇 가지 개선 사항입니다.

* 키보드의 tab 키를 사용하여 표의 열과 행을 탐색합니다

* 열 위치에서 새 레코드를 추가합니다. 이 개선 이전에는 첫 번째 열에서만 레코드를 추가할 수 있었습니다.

* Shift 키와 Enter 키 조합을 사용하여 표에 새 레코드(또는 행)를 추가합니다.

자세한 내용은 [레코드 만들기](../maestro/records/connect-records.md).

## 2023년 10월 16일 주

### 새 사람 필드 유형

미리보기 및 프로덕션: 2023년 10월 16일

이제 Maestro 레코드 유형에 사람 유형 필드를 추가할 수 있습니다. 사람 유형 필드를 사용하여 기존 사용자를 레코드와 연결할 수 있습니다. 자세한 내용은 [필드 만들기](../maestro/fields/create-fields.md).

### 단락 필드에 대한 리치 텍스트 형식

미리보기 및 프로덕션: 2023년 10월 16일

단락 유형 필드에 리치 텍스트 형식 컨트롤을 추가했습니다. 레코드 유형의 표 보기 또는 레코드의 세부 정보 페이지에서 서식 있는 텍스트를 사용하여 단락 필드의 서식을 지정할 수 있습니다. 자세한 내용은 [레코드 편집](../maestro/records/edit-records.md).


### 타임라인 보기에 대한 색상 코딩 기록 및 그룹화

미리보기 및 프로덕션: 2023년 10월 19일

이제 타임라인 보기에서 레코드 창과 그룹화에 대해 색상 코드를 지정할 수 있습니다.

다음은 타임라인 보기에서 레코드 막대 및 그룹화에 대해 표시하도록 선택할 수 있는 색상에 대한 옵션입니다.

* 그룹화는 다음 색과 일치할 수 있습니다.

   * 회색(기본값)

   * 그룹화할 필드의 색상

* 막대는 다음 색상과 일치할 수 있습니다.

   * 레코드 유형의 색상

   * 선택하는 필드의 색상

   * 그룹화의 색상

   * 색상 없음(기본값)

특정 필드에 색상을 일치시킬 때는 색상으로 구분된 옵션이 있는 필드만 선택할 수 있습니다.

자세한 내용은 [타임라인 보기 관리](../maestro/views/manage-the-timeline-view.md).

## 2023년 10월 9일 주

### 표 보기에서 검색

미리보기 및 프로덕션: 2023년 10월 9일

이제 키워드를 검색하여 테이블 보기에서 레코드를 빠르게 찾을 수 있습니다. 화면에 표시되는 모든 필드에 키워드와 특수 문자를 사용하여 레코드를 찾을 수 있습니다. 자세한 내용은 [표 보기 관리](../maestro/views/manage-the-table-view.md).

## 2023년 9월 18일 주

### 행 순서 바꾸기

미리보기 및 프로덕션: 2023년 9월 20일

이제 레코드 유형 페이지의 테이블 보기에서 하나 또는 여러 행(또는 레코드)의 순서를 변경할 수 있습니다. 자세한 내용은 [표 보기 관리](../maestro/views/manage-the-table-view.md).

## 2023년 9월 4일 주

### Maestro 기록을 Workfront 회사 및 그룹과 연결

미리보기 및 프로덕션: 2023년 9월 5일

이제 마에스트로 레코드를 Workfront 회사 및 그룹과 연결할 수 있습니다. 먼저 Maestro 레코드 유형과 Workfront 회사 및 그룹 객체 유형 간에 연결을 만들어야 합니다. 그런 다음 선택한 레코드 유형의 단일 마에스트로 레코드를 개별 Workfront 회사 및 그룹에 연결할 수 있습니다.

다음 사항을 고려하십시오.

* 각 작업 영역에 대해 Maestro 레코드 유형과 Workfront 회사 및 그룹 객체 유형 간에 연결을 만들어야 합니다.

* 분류 레코드 유형을 Workfront 객체 유형과 연결할 수 없습니다.

* 여러 Maestro 레코드를 동일한 Workfront 회사 또는 그룹에 연결하고 여러 회사 또는 그룹을 동일한 Maestro 레코드에 연결할 수 있습니다.

* Maestro에서 회사 또는 그룹을 편집할 수 없습니다. Workfront에서 수행된 모든 회사 또는 그룹 변경 사항은 Maestro 연결 레코드를 검토할 때 Maestro에 표시됩니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [레코드 유형 연결](../maestro/architecture/connect-record-types.md)
   * [레코드 연결](../maestro/records/connect-records.md)

### 한 줄 텍스트 필드에 대한 URL 지원

미리보기 및 프로덕션: 2023년 9월 7일

표 보기에서 링크 작업을 수행할 때 가시성을 높이기 위해 한 줄 텍스트 필드에 URL에 대한 지원을 추가했습니다. 에서는 한 줄 텍스트 필드를 업데이트할 때 다른 웹 사이트 또는 외부 드라이브에 대한 URL을 사용하므로 이를 링크로 식별하여 표에서 클릭할 수 있습니다. 이 개선 이전에는 링크가 텍스트로 표시되었습니다.

## 2023년 8월 28일 주

### 테이블 뷰 도구 모음의 필드 가시성 메뉴

미리보기 및 프로덕션: 2023년 8월 31일

지정된 레코드 집합에 올바른 정보를 표시하려면, 특히 레코드 종류의 일부 필드가 아닌 일부 필드를 표시해야 하는 다른 사용자와 보기를 공유하려는 경우, 이제 테이블 보기에서 표시할 필드(또는 열)와 숨길 필드를 선택할 수 있습니다.

필드 열의 각 헤더에서 개별 필드를 숨기거나 표시하거나 테이블 보기 도구 모음의 설정에서 레코드 유형의 모든 필드를 관리할 수 있습니다.

자세한 내용은 [표 보기 관리](../maestro/views/manage-the-table-view.md).

## 2023년 8월 21일 주

### Maestro 레코드를 프로그램 및 포트폴리오에 연결

미리보기 및 프로덕션: 2023년 8월 24일

이제 마에스트로 레코드를 Workfront 프로그램 및 포트폴리오와 연결할 수 있습니다. Maestro 레코드 유형과 연결된 필드를 만드는 프로그램 또는 포트폴리오 간에 연결을 만들어야 합니다. 그런 다음 동일한 작업 공간 내의 다른 모든 레코드 유형의 Maestro 레코드를 동일한 작업 공간에서 읽기 전용 Workfront 프로그램 또는 Workfront Portfolio 레코드 유형을 만드는 특정 프로그램 및 포트폴리오에 연결할 수 있습니다. 다음 사항을 고려하십시오.

* Workfront 커넥터 레코드 유형은 각 작업 공간에 대해 고유합니다.
* 여러 Maestro 레코드를 동일한 Workfront 프로그램 또는 포트폴리오에 연결하고 여러 프로그램 및 포트폴리오를 동일한 Maestro 레코드에 연결할 수 있습니다.
* Maestro에서는 프로그램 및 포트폴리오를 편집할 수 없습니다. Workfront에서 수행한 모든 프로그램 및 포트폴리오 변경 사항은 연결된 레코드를 검토할 때 Maestro에서 볼 수 있습니다.

### 테이블 보기에 대한 새로운 정렬 기능

미리보기 및 프로덕션: 2023년 8월 24일

이제 레코드 유형 페이지의 표 보기에서 레코드를 정렬할 수 있습니다.
이제 다음 기능을 사용할 수 있습니다.

* 동시에 여러 필드를 기준으로 정렬할 수 있는 테이블 수준에서 정렬합니다.
* 한 번에 개별 필드를 기준으로 정렬할 수 있는 열 또는 필드 수준에서 정렬합니다.

### 타임라인 보기의 개선 사항: 그룹화 및 Compact/Standard 보기 스위치의 새로운 모양

미리보기 및 프로덕션: 2023년 8월 24일

타임라인 보기에 다음과 같은 개선 사항이 도입되었습니다.

* 이제 다음 모드로 타임라인 보기를 표시할 수 있습니다.

   * 표준: 레코드를 별도의 라인에 표시합니다.
   * 작게: 날짜가 같은 줄에 교차하지 않는 레코드를 표시합니다.

* 타임라인 보기의 그룹화 선이 포함된 레코드의 타임라인 위에 표시되도록 해당 줄의 모양을 변경했습니다. 이 개선 이전에는 타임라인 전체 길이에 걸쳐 그룹화가 표시되었습니다.

## 2023년 8월 14일 주

### 테이블 보기에서 열 순서 바꾸기

이제 Maestro 테이블 보기에서 열의 순서를 변경할 수 있습니다. 열을 재정렬할 때는 다음 사항을 고려하십시오.

* 이름 필드는 항상 레코드 유형 페이지의 테이블 보기에서 첫 번째 필드입니다

* 이름 필드를 다른 위치로 이동할 수 없습니다.

* 이름 필드가 고정되어 있고 가로 스크롤의 일부가 아닙니다.

### 타임라인 보기를 위한 수평 스크롤

이제 레코드 유형의 타임라인 보기에서 가로로 스크롤할 수 있습니다.

## 2023년 8월 7일 주

### Excel 파일에서 레코드 형식 가져오기

미리보기 및 프로덕션: 2023년 8월 10일

이제 Excel 파일을 가져와서 작업 공간에서 레코드 유형을 만들 수 있습니다. 파일의 시트는 레코드 유형이 되고 파일의 열은 해당 필드가 됩니다.

### 레코드 유형 및 프로젝트 연결 경험 개선

미리보기 및 프로덕션: 2023년 8월 10일

Workfront 프로젝트에 연결을 포함하여 레코드 유형을 연결하는 방법을 개선했습니다. 이 개선 사항의 일부로 테이블 보기에서 레코드 종류에 대한 필드를 추가할 때 다음과 같이 변경되었습니다.

* &quot;새 필드&quot; 탭에서 관계 유형 필드를 제거했습니다.

* 연결할 레코드 또는 개체 유형을 직접 선택할 수 있는 &quot;새 연결&quot; 탭을 추가하여 관계 유형 필드가 필요하지 않게 합니다.

## 2023년 7월 10일 주

### 레코드 유형의 모양 업데이트

미리보기 및 프로덕션: 2023년 7월 13일

이제 레코드 종류에 대해 사용자 지정 아이콘을 선택하고 레코드 종류 아이콘에 대해 사용자 지정 색상을 선택할 수 있습니다.

### 새 확인란 필드 유형

미리보기 및 프로덕션: 2023년 7월 13일

이제 Checkbox 필드 유형을 Maestro 레코드 유형에 추가할 수 있습니다. 확인란 유형 필드를 사용하여 레코드에 단일 확인란 옵션을 추가할 수 있습니다. 이 필드를 사용하여 특정 레코드에 대한 특정 속성이나 상태를 표시할 수 있습니다. 예를 들어 각 레코드의 완료, 승인 또는 기타 모든 이진 속성을 추적하기 위한 플래그로 사용할 수 있습니다.

## 2023년 6월 26일 주

### 표에서 상황별 메뉴의 빠른 활성화

미리보기 및 프로덕션: 2023년 6월 28일

테이블 보기 또는 레코드 유형에서 레코드를 볼 때 레코드 행의 아무 곳이나 마우스 오른쪽 버튼으로 클릭하여 상황별 메뉴를 활성화하는 기능을 활성화했습니다. 이제 레코드 유형의 테이블 보기에서 컨텍스트 메뉴에 액세스할 때 레코드의 세부 정보 페이지에 대한 링크를 빠르게 보거나 삭제하거나 복사할 수 있습니다. 이 기능이 향상되기 전에는 레코드의 이름 열에 있는 자세히 메뉴에서만 상황별 메뉴에 액세스할 수 있었습니다.

## 2023년 6월 19일 주

### 레코드 필드 이름이 고유합니다.

이제 Maestro 레코드 유형의 필드 이름에 고유한 이름이 있어야 한다는 요구 사항을 도입했습니다. 다른 레코드 유형에 속하는 필드는 고유한 이름을 가질 필요가 없습니다.

## 2023년 6월 5일 주

### Maestro 레코드와 Workfront 프로젝트 연결

미리보기 및 프로덕션: 2023년 6월 5일

이제 마에스트로 레코드를 Workfront 프로젝트와 연결할 수 있습니다. Maestro 레코드와 Workfront 프로젝트 간의 연결을 설정하려면 커넥터 Maestro 레코드 유형을 만들어야 합니다. 그런 다음 관계 필드를 사용하여 다른 모든 레코드 유형의 Maestro 레코드를 커넥터 레코드에 연결할 수 있습니다. 다음 사항을 고려하십시오.

* 각 작업 공간에 대해 Workfront에 대한 커넥터 레코드 유형이 있어야 합니다.
* 여러 Maestro 레코드를 동일한 Workfront 프로젝트에 연결하고 여러 프로젝트를 동일한 Maestro 레코드에 연결할 수 있습니다.
* Maestro에서는 프로젝트를 편집할 수 없습니다. Workfront에서 수행된 모든 프로젝트 변경 사항은 연결된 레코드를 검토할 때 Maestro에 표시됩니다.

## 2023년 5월 29일 주

### 타임라인 보기를 만들기 위한 2일 요구 사항

미리보기 및 프로덕션: 2023년 5월 31일

타임라인 보기를 만들려면 레코드 유형과 연결된 날짜 필드가 두 개 이상 있어야 합니다.
