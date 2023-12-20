---
product-area: reporting
navigation-topic: text-mode-reporting
title: 그룹화에서 텍스트 모드 편집
description: '참고: 텍스트 모드에서 편집할 때 모든 FVG 문서를 동일하게 설정)'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# 그룹화에서 텍스트 모드 편집

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

텍스트 모드를 사용하여 목록 또는 보고서에서 그룹화를 편집하여 표준 인터페이스에서 사용할 수 없는 필드에 액세스하고 보다 복잡한 그룹화를 만들 수 있습니다.

>[!TIP]
>
>표준 모드에서 가능한 한 많은 그룹화를 작성한 다음 텍스트 모드로 변환하여 편집하는 것이 좋습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스 권한을 편집하여 보고서의 그룹화를 편집합니다.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서의 그룹화를 편집합니다.</p> <p>편집할 그룹화에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

보고서나 목록에서 텍스트 모드 사용을 시작하기 전에 항상 Workfront 텍스트 모드 구문을 잘 알고 있는지 확인하십시오.

자세한 내용은 다음을 참조하십시오.

* [텍스트 모드 개요](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [텍스트 모드 구문 개요](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [사용자 정의 보기, 필터링 및 그룹화 샘플: 문서 인덱스](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 그룹화에서 텍스트 모드 편집

텍스트 모드를 사용하여 그룹화를 편집하는 것은 보고서와 목록에 대해 동일합니다. 보고서 또는 목록에서 그룹화에 액세스하는 방법은 다릅니다.

>[!NOTE]
>
>그룹화는 보고서에서 차트를 만들기 위한 필수 보고 요소입니다. 텍스트 모드 그룹화는 차트에서 지원되지 않습니다. 보고서에 차트를 추가하는 방법에 대한 자세한 내용은 [보고서에 차트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

그룹화 만들기에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 다음 중 하나를 수행하십시오.

   1. 보고서에서 그룹화에 액세스하려면 해당 보고서로 이동한 다음 **보고서 작업** > **편집** > **그룹화** 탭.
   1. 목록에서 그룹화에 액세스하려면 목록으로 이동한 다음 **그룹화** 드롭다운 메뉴를 수정하려는 그룹화 위로 마우스를 가져간 후 **편집** 아이콘 ![](assets/edit-icon.png).

      그룹화 빌더가 열립니다.

1. 클릭 **그룹화 추가** 그룹화를 추가한 다음 을 클릭합니다. **텍스트 모드로 전환** 빌더의 오른쪽 상단 모서리에서 을 클릭합니다.

   >[!TIP]
   >
   표준 인터페이스에서 최대 3개의 그룹화를 추가할 수 있습니다. 텍스트 모드만 사용하여 네 번째 그룹화를 추가할 수 있으며 Workfront에서는 4개 이상의 그룹화 수준을 가질 수 없습니다.

1. 그룹화할 필드의 이름을 입력하십시오.

   목록에 표시되는 필드의 이름을 선택합니다.

1. 클릭 **텍스트 모드로 전환** 빌더의 오른쪽 상단 모서리에서 을 클릭합니다.

   그러면 그룹화가 텍스트 모드로 표시됩니다.

   텍스트 모드에서 그룹화를 편집하면 Workfront이 다음을 추가합니다.

   ```
   textmode=true
   ```

   그룹화에 대한 코드 줄입니다. 이는 텍스트 모드에서 그룹화가 수정되었음을 나타냅니다.

   **예:** 작업 목록을 프로젝트 이름으로 그룹화한 다음 기본 피할당자의 이름으로 그룹화하려면 텍스트 모드에서 그룹화는 다음과 같아야 합니다.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   굵은 선은 필수입니다.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   그룹화의 각 필드에는 해당 필드를 참조하는 여러 줄의 코드가 있습니다.

   아래 표는 텍스트 모드 그룹화의 주요 행에 대한 개요를 제공합니다.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   텍스트 모드 그룹화의 키 라인은 텍스트 모드 뷰를 작성하는 데 필요한 라인과 유사합니다.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>샘플 라인</strong> </th> 
      <th><strong>설명</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>그룹입니다.&lt;number&gt;.</strong> </td> 
      <td> <p>각 코드 줄 앞에는 이 텍스트가 있습니다. 그룹화에서 선택한 동일한 필드를 참조하는 코드 행은 다음과 같이 동일한 번호로 번호가 매겨집니다.</p> 
       <ul> 
        <li>보고서의 첫 번째 그룹화는 그룹 번호가 0입니다. 첫 번째 그룹화를 참조하는 모든 줄은 다음으로 시작합니다. <code>group.0</code>.</li> 
        <li>보고서의 두 번째 그룹화는 그룹 번호가 1입니다. 두 번째 그룹화를 참조하는 모든 줄은 다음으로 시작합니다. <em><code>group.1</code></em>.</li> 
        <li>보고서의 세 번째 그룹화는 그룹 번호가 2입니다. 세 번째 그룹화를 참조하는 모든 줄은 다음으로 시작합니다. <em><code>group.2</code></em>.</li> 
        <li>텍스트 모드에서만 네 번째 그룹화에 대해 그룹 번호 3을 추가할 수 있습니다. 네 번째 그룹화를 참조하는 모든 줄은 다음으로 시작합니다. <em><code>group.3</code></em>.</li> 
       </ul> <p>참고: 4개의 그룹화는 빌더에서 지원되지 않습니다. 텍스트 모드를 사용할 때만 지원됩니다. Workfront은 4개 이상의 그룹화 수준을 지원하지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>데이터베이스에 나타나는 개체 또는 필드의 이름입니다. 개체와 필드가 데이터베이스에 표시되는 방법에 대한 자세한 내용은 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API 탐색기</a>.</p> <p>다음과 같은 시나리오가 있습니다.</p> 
       <ol> 
        <li value="1"> <p> 표시되는 필드 이름이 단일 명사가 아닌 구문인 경우 <code>valuefield</code>. 예를 들어 작업의 계획된 시작 일자의 경우 코드는 다음과 같습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>사용자 지정 필드를 표시하려면 <code>valuefield</code> 값은 인터페이스에 표시된 실제 필드 이름입니다. 예를 들어 "추가 정보"라는 사용자 정의 필드의 경우 코드는 다음과 같습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>를 사용하여 다른 객체와 관련된 객체별로 그룹화하려는 경우 <code>valuefield</code> 코드 행 개체 이름과 특성은 콜론으로 구분됩니다.</p> <p>예를 들어, 작업 목록에 대해 Portfolio 이름별로 그룹화할 때 valuefield 라인의 값은 다음과 같습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>이는 보고서(작업) 객체에서 다음 관련 객체(프로젝트)에 액세스할 수 있음을 나타냅니다. 여기에서 프로젝트(포트폴리오)에서 다음 관련 객체에 액세스한 다음 포트폴리오 이름(이름)에 액세스할 수 있습니다.</p> </li> 
       </ol> <p>개체가 서로 연결되는 방법에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">객체의 상호 의존성 및 계층</a> 위치: <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront의 오브젝트 이해</a>.</p> <p>주: 표준 인터페이스에서 유효하지 않은 텍스트 모드의 필드를 선택하고 표준 인터페이스로 전환하면 그룹화가 삭제됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>이 줄은 을 표시하는 데 사용되는 형식을 나타냅니다. <code>valuefield</code>. 다음 <code>valueformat</code> 개체나 필드가 텍스트, 숫자, 백분율 또는 날짜로 표시되는지 여부를 식별합니다.</p> <p>다음을 사용하는 것이 좋습니다. <code>HTML</code> 에 대한 <code>valueformat</code>, 특히 을 사용할 때 <code>valueexpression</code>를 사용하여 정보를 가장 정확하게 표시할 수 있습니다.</p> <p>이 라인의 추가 값에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">텍스트 모드에서 조건부 서식 사용</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>이 줄을 추가하여 바꿀 수 있습니다. <code>valuefield</code>를 사용하여 여러 필드 간의 계산으로 목록을 그룹화하십시오.</p> <p>다음을 동봉해야 합니다. <code>valuefield</code> 에서 사용할 때마다 중괄호로 묶인 개체의 수를 <code>valueexpression</code>.</p> <p>다음과 같은 시나리오가 있습니다.</p> 
       <ol> 
        <li value="1"> <p>대문자로 그룹화의 이름을 표시하려면 다음을 사용합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>다음 <code>valuefield</code> API 탐색기에 나타나는 대로 개체의 철자가 지정됩니다.</p> </li> 
        <li value="2">여러 을(를) 추가하려면 <code>valuefields</code> ...로 묶어서 <code>valueexpression </code>line, 마침표로 구분해야 합니다.<p>예를 들어 작업 목록에서 포트폴리오의 이름을 대문자로 표시하려면 다음에서 다음 코드를 사용합니다 <code>valueexpression</code> 줄:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>에서 사용자 정의 필드를 사용하려면 <code>valueexpression</code> 줄 필드 이름 앞에 다음 기한까지 와야 합니다. <code>DE:</code> 사용자 정의 필드임을 나타냅니다. 필드 이름의 철자는 인터페이스에 나타나는 대로 입력됩니다.</p><p>중요 사항: <span>일부 사용자에 대한 권한이 제한된 사용자 정의 양식 섹션에 배치된 사용자 정의 필드를 사용하는 경우 <code>valueexpression </code>보고서에서 이 계산을 볼 때 가 비어 있습니다. 사용자 정의 양식 섹션의 권한 조정에 대한 자세한 내용은</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 정의 양식 만들기 또는 편집</a></span>.</p><p>예를 들어 사용자 정의 필드에 "개발자 이름"이라는 레이블이 있고 이 필드로 그룹화하여 대문자로 표시하려는 경우 다음을 사용할 수 있습니다 <code>valueexpression</code> 이를 나타내는 방법:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>타이프 어헤드 유형 사용자 정의 필드를 참조할 때 다음 표현식을 사용하여 "개발자 이름"이라는 레이블이 지정된 필드에서 선택한 개체의 이름을 참조합니다.</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>이 줄은 그룹화 레이블을 정의합니다. 이 경우 키를 기반으로 하는 축약값을 사용합니다.</p> <p>그룹화 이름을 수정하려면 이 값을 다음과 같이 변경할 수 있습니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> 에서는 그룹화 이름에 대한 텍스트를 입력할 수 있지만 <code>namekey</code> 을(를) 사용하려면 그룹화 이름을 번역하는 데 사용되는 키를 입력해야 합니다.</p> <p>그룹화 이름을 변경하려면 <code>displayname </code>줄, 없는 경우.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>다음 줄을 추가하여 열 이름을 변경할 수 있습니다. 이 이름은 <code>namekey/name</code> 값:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>이 포함된 모든 줄을 제거하는 것이 좋습니다. <code>name </code>그룹화 이름을 바꿀 때</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 다음 코드 줄 중 하나를 그룹화에 추가하여 그룹화 결과가 확장된 목록에 표시되는지 아니면 축소된 목록에 표시되는지 여부를 나타냅니다. 기본적으로 그룹화가 확장되어 표시됩니다.


   ```
   group.0.iscollapsed=true
   ```

   결과를 축소한 상태로 그룹화를 표시하려면

   ```
   group.0.iscollapsed=false
   ```

   결과를 확장하여 그룹화를 표시하려면

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   * 목록을 볼 때 수동으로 그룹화를 조정하면 Workfront은 로그아웃하기 전까지 수동 기본 설정을 기억합니다. 다시 로그인하면 이 설정에 따라 목록이 표시됩니다.
   * 차트 요소에서 액세스한 후 그룹화 결과는 항상 확장되어 표시됩니다.

1. 클릭 **완료** 변경 사항을 저장하고 그룹화나 보고서를 계속 편집하려면 다음을 수행하십시오.
1. 클릭 **그룹화 저장** 또는 **저장 + 닫기** 보고서를 저장합니다.
