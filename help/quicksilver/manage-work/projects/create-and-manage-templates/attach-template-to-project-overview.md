---
content-type: overview
product-area: templates
keywords: 덮어쓰기,필드,덮어쓰기
navigation-topic: templates-navigation-topic
title: 프로젝트에 템플릿 첨부 개요
description: 기존 프로젝트에 템플릿을 첨부할 경우 템플릿의 정보에 따라 프로젝트의 일부 정보를 수정합니다. 그 프로젝트에 관한 일부 정보는 변함이 없다.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 7%

---

# 프로젝트에 템플릿 첨부 개요

기존 프로젝트에 템플릿을 첨부할 경우 템플릿의 정보에 따라 프로젝트의 일부 정보를 수정합니다. 그 프로젝트에 관한 일부 정보는 변함이 없다.

프로젝트에 템플릿을 첨부하는 방법에 대한 자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)를 참조하십시오.

## 프로젝트에 템플릿을 추가할 때 고려 사항

프로젝트에 템플릿을 추가할 때 다음 사항을 고려하십시오.

* 활성 템플릿만 프로젝트에 첨부할 수 있습니다.
* Adobe Workfront 관리자 또는 그룹 관리자가 프로젝트 환경 설정 영역에서 이 기능을 활성화한 경우에만 프로젝트가 완료, 중단 또는 승인 보류 상태일 때 프로젝트에 템플릿을 첨부할 수 있습니다. 프로젝트 환경 설정 지정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.
* 특정 템플릿 작업이 첨부 프로세스에서 추가되지 않도록 제외하지 않으면 모든 템플릿 작업이 기존 프로젝트에 추가됩니다.
* 대부분의 템플릿 설정이 프로젝트에 추가됩니다. 일부 프로젝트 설정은 유지됩니다. 자세한 내용은 이 문서에서 [템플릿을 첨부할 때의 프로젝트 필드 변경 내용 이해](#understand-changes-to-project-fields-when-attaching-a-template) 섹션을 참조하십시오.

## 템플릿을 첨부할 때 프로젝트 필드의 변경 사항 이해 {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>템플릿을 프로젝트에 첨부하는 것은 템플릿에서 프로젝트를 만드는 것과 다릅니다. 템플릿에서 프로젝트를 만들 때 모든 템플릿 필드가 새 프로젝트로 전송됩니다. 템플릿을 첨부하면 기존 프로젝트 필드 중 일부가 변경되지 않습니다.

템플릿 첨부 프로세스 중에 제외되도록 명시적으로 표시하지 않는 한 일부 템플릿 설정은 프로젝트로 자동 전송됩니다. 제외하도록 표시하면 프로젝트 필드 값이 유지됩니다.

그러나 템플릿을 프로젝트에 첨부하는 과정에서 일부 프로젝트 필드를 관리할 수는 없습니다. 자세한 내용은 [프로젝트에 템플릿 첨부](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)를 참조하십시오.

다음 표에서는 템플릿을 첨부할 때 프로젝트 필드에 발생하는 내용과 기본 동작을 무시하기 위해 첨부 프로세스 중에 관리할 수 있는 필드에 대한 기본값을 설명합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>필드</td> 
   <td>템플릿을 첨부하는 과정에서 기본적으로 수행되는 작업</td> 
   <td>첨부 파일 프로세스의 필드 업데이트 관리 기능 </td> 
  </tr> 
  <tr> 
   <td>설명</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>상태</p> </td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>프로젝트의 필드가 비어 있는 경우 템플릿에서 전송됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>우선순위</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>상태 유형</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>일정 모드</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>계획된 일자</td> 
   <td>추가된 작업에 따라 변경될 수 있음</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>실제 일자</td> 
   <td>추가된 작업에 따라 변경될 수 있음</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>포트폴리오</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로그램</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>그룹</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>회사</td> 
   <td>프로젝트의 필드가 비어 있는 경우 템플릿에서 전송됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>계획된 시간</td> 
   <td>추가된 작업에 따라 변경될 수 있음</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로젝트 소유자</td> 
   <td>프로젝트의 필드가 비어 있는 경우 템플릿에서 전송됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로젝트 스폰서</td> 
   <td>프로젝트의 필드가 비어 있는 경우 템플릿에서 전송됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>리소스 관리자</td> 
   <td>프로젝트의 기존 리소스 관리자 목록에 추가됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>사용자 정의 양식</td> 
   <td>프로젝트에 이미 있는 양식 외에 를 프로젝트에 추가했습니다.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>예산</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>통화</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>계획된 이익</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>실제 이익</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>마일스톤 경로</td> 
   <td>프로젝트의 필드가 비어 있는 경우 템플릿에서 전송됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>완료 모드</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>요약 완료 모드</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>업데이트 유형</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>예약</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>사용자 휴무</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>리소스 레벨링 모드</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>위험(프로젝트 필드)</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>리소스 풀</td> 
   <td>프로젝트의 기존 리소스 풀 목록에 추가됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>시간 유형</td> 
   <td> <p>첨부 파일 프로세스 중에 선택 해제되면 프로젝트의 시간 유형 설정이 변경되지 않습니다. </p> <p>선택하면 템플릿 설정이 프로젝트로 전송됩니다. 프로젝트와 템플릿 모두에서 시간 유형 필터링이 예로 설정된 경우 템플릿의 시간 유형이 프로젝트의 시간 유형에 추가됩니다.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>미리 알림</td> 
   <td> <p>프로젝트에 대한 기존 미리 알림 목록에 추가되었습니다. </p> <p>첨부 프로세스 중에 선택을 취소한 경우 프로젝트 미리 알림은 변경되지 않습니다. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>작업 기본 승인 프로세스</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>작업 기본 사용자 정의 양식</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>작업 노력</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>사용자가 인라인으로 문제를 추가하도록 허용</span> </td> 
   <td><span>프로젝트 정보가 유지됩니다</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>모든 설정</td> 
   <td>템플릿 설정이 프로젝트의 설정을 덮어씁니다.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>작업</td> 
   <td>기존 프로젝트 작업 외에 작업 목록 맨 아래에 추가됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>문서</td> 
   <td>기존 프로젝트 문서에 추가하여 프로젝트에 추가됨</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>위험(프로젝트의 위험 영역에 있는 객체)</td> 
   <td>기존 프로젝트 위험에 추가하여 프로젝트에 추가됨 </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>승인 진행</td> 
   <td>템플릿에서 전송됨</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>청구 요율</td> 
   <td> <p>프로젝트의 기존 청구 요금에 더해 템플릿에서 전송됨. </p> <p>프로젝트와 템플릿 모두에서 동일한 작업 역할에 대해 다른 비율이 있는 경우 프로젝트의 비율은 변경되지 않습니다. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>청구 기록</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>경비</td> 
   <td>템플릿의 기존 비용에 더해 템플릿에서 전송됨</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>재무 정보</td> 
   <td> <p>첨부 프로세스에서 이 옵션을 선택하면 다음 필드가 프로젝트에 전송되거나 추가됩니다. </p> 
    <ul> 
     <li> <p>고정 비용</p> <p>옵션을 선택하면 프로젝트의 업데이트된 고정 비용이 다음 공식을 사용하여 계산됩니다.</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>고정 수입</p> <p>옵션을 선택하면 다음 공식을 사용하여 프로젝트의 업데이트된 고정 수익이 계산됩니다.</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>작업의 비용 유형</p> <p>템플릿에서 전송됨</p> </li> 
     <li> <p>작업에 대한 수익 유형</p> <p>템플릿에서 전송됨</p> </li> 
    </ul> <p>첨부 프로세스 중에 이 필드를 선택 해제하면 다음과 같은 결과가 발생합니다.</p> 
    <ul> 
     <li> <p>프로젝트의 고정 비용 및 고정 수익은 유지됩니다.</p> </li> 
     <li> <p>템플릿에서 추가된 작업의 비용 및 수익 유형이 비용 없음 및 청구 불능으로 설정됩니다</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>시간</td> 
   <td>프로젝트 정보가 보존됨</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>대기열 세부 정보, 주제 그룹, 대기열 주제, 라우팅 규칙</td> 
   <td> <p>템플릿에서 전송됨</p> <p>첨부 파일 프로세스 중에 <strong>큐 속성 및 문제 설정</strong> 옵션을 선택하면 템플릿의 큐 세부 정보가 프로젝트의 세부 정보를 덮어씁니다. 이 경우 템플릿의 라우팅 규칙, 대기열 주제 및 주제 그룹이 프로젝트의 그룹에 추가됩니다. <br>프로젝트가 요청 대기열로 설정되어 있고 프로젝트에 첨부한 템플릿이 요청 대기열로 설정되어 있지 않은 경우 <strong>대기열 속성 및 문제 설정</strong> 상자를 선택한 상태로 두면 프로젝트의 대기열 정보가 제거됩니다. <br><strong>대기열 속성 및 문제 설정</strong> 상자를 선택 취소하면 프로젝트의 모든 대기열 설정 설정이 유지되며 템플릿의 대기열 설정 설정은 첨부되지 않습니다.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>작업 제한</td> 
   <td> <p>템플릿에서 전송됨 </p> <p>첨부 프로세스 중에 선택 해제되면 프로젝트 일정 시작 설정에 따라 작업 제한 조건이 가능한 한 빨리 또는 가능한 한 늦게 설정됩니다. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>작업의 전임 작업</td> 
   <td> <p>템플릿에서 전송됨</p> <p>첨부 파일 프로세스 중에 선택을 취소하면 템플릿 작업 간의 모든 전임 작업 연결이 제거됩니다.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>공유 옵션</td> 
   <td> <p>첨부 파일 프로세스 중에 선택 해제되면 프로젝트 권한은 변경되지 않습니다.</p> <p>첨부 파일 프로세스 중에 선택된 경우 템플릿 권한이 프로젝트에 추가되거나 프로젝트의 권한을 덮어씁니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span>사용자 A에게 프로젝트에 대한 보기 권한이 있지만 템플릿에 대한 관리 권한이 있는 경우 템플릿을 첨부하면 사용자 A가 프로젝트에 대한 관리 액세스 권한을 갖게 됩니다.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>



<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom Forms</b>: Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p> </p>
</div>
-->


