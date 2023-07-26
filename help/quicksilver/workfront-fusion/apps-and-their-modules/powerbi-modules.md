---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Power BI 모듈
description: Adobe Workfront Fusion에는 Adobe Workfront 라이센스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2398'
ht-degree: 0%

---

# [!DNL Power BI] 모듈

[!DNL Power BI] 는 관련자들에게 데이터를 시각화하고 제시할 수 있는 애플리케이션입니다. 다양한 소스에서 데이터를 가져올 수 있습니다.

>[!NOTE]
>
>[!DNL Workfront Fusion] 은(는) 데이터 소스가 아닙니다. While [!DNL Workfront Fusion] 는 데이터를 저장하지 않으며, 데이터 소스를 만들고 사용할 수 있습니다.


## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

&#42;&#42;다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] 모듈 및 해당 필드

를 구성할 때 [!DNL Power BI], [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이러한 필드와 함께 앱이나 서비스의 액세스 수준과 같은 요소에 따라 추가 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [Adobe Workfront Fusion의 한 모듈에서 다른 모듈로 정보 매핑](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 대시보드

#### [!UICONTROL 목록 대시보드]

이 검색 모듈은 대시보드 목록을 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>
        <p>나열할 대시보드를 소유한 그룹의 ID를 선택하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 목록 대시보드 타일]

이 검색 모듈은 대시보드 타일 목록을 검색합니다.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 대시보드 ID 입력]</td>
    <td>
      <p>옵션을 선택하거나 매핑하여 타일을 나열할 대시보드를 선택합니다.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 대시보드 ID]</td>
    <td>
      <p>나열할 타일이 포함된 대시보드의 ID를 입력하거나 매핑합니다.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
    <td>나열할 타일이 포함된 대시보드를 소유한 그룹의 ID를 선택하거나 매핑합니다.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 제한]  </td>
    <td>
      <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 대시보드 가져오기]

이 작업 모듈은 지정된 대시보드의 메타데이터를 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 대시보드 ID 입력]</td>
      <td>
        <p>옵션을 선택하거나 매핑하여 메타데이터를 검색할 대시보드를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 대시보드 ID]</td>
      <td>
        <p>메타데이터를 검색할 대시보드의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>메타데이터를 검색할 대시보드를 소유한 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 대시보드 타일 가져오기]

이 작업 모듈은 지정된 대시보드 타일의 메타데이터를 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 대시보드 ID 입력]</td>
      <td>
        <p>옵션을 선택하거나 매핑하여 검색할 대시보드 세부 정보를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 대시보드 ID]</td>
      <td>
        <p>세부 정보를 검색할 대시보드의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 타일 ID]</td>
      <td>의 ID 입력 또는 매핑 [!DNL Power BI] 세부 정보를 검색할 타일입니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>검색할 타일을 소유한 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 대시보드 만들기]

이 작업 모듈은 새 대시보드를 만듭니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>대시보드의 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>새 대시보드를 소유할 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

### 보고서

#### [!UICONTROL 목록 보고서]

이 검색 모듈은 보고서 목록을 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>
        <p>나열할 보고서를 소유하는 그룹의 ID를 선택하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 보고서 가져오기]

이 작업 모듈은 지정된 보고서의 메타데이터를 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID 입력]</td>
      <td>
        <p>옵션을 선택하거나 매핑하여 메타데이터를 검색할 보고서를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID]</td>
      <td>
        <p>메타데이터를 검색할 보고서의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>메타데이터를 검색할 보고서를 소유한 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 보고서 복사]

이 작업 모듈은 기존 보고서를 복사합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID 입력]</td>
      <td>
        <p>옵션을 선택하거나 매핑하여 복사할 보고서를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID]</td>
      <td>
        <p>복사할 보고서의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>복사할 보고서를 소유한 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 새로 복사된 보고서 이름]</td>
      <td>새 보고서의 이름을 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 보고서 삭제]

이 작업 모듈은 보고서를 삭제합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID 입력]</td>
      <td>
        <p>옵션을 선택하거나 매핑하여 삭제할 보고서를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID]</td>
      <td>
        <p>삭제할 보고서의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>삭제할 보고서를 소유한 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

### 데이터 세트

#### [!UICONTROL 데이터 세트 나열]

이 검색 모듈은 데이터 세트 목록을 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>메타데이터를 검색할 보고서를 소유한 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]</td>
      <td>
        <p>각 시나리오 실행 주기 동안 모듈에 [action]으로 지정할 최대 레코드 수를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 데이터 세트 가져오기]

이 작업 모듈은 지정된 데이터 세트의 메타데이터를 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID 입력]</td>
      <td>
        <p>옵션을 선택하거나 매핑하여 메타데이터를 검색할 보고서를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID]</td>
      <td>
        <p>메타데이터를 검색할 데이터 세트의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>메타데이터를 검색할 데이터 세트를 소유하는 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 데이터 세트 만들기]

이 작업 모듈은 새 데이터 세트를 만듭니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>데이터 세트의 이름을 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>새 데이터 세트를 소유할 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 기본 모드]</td>
      <td>
        <p>데이터 세트에 대한 기본 모드 선택 또는 매핑:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: 의 라이브 연결이 있는 데이터 세트 [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As On Prem]</b>: 의 라이브 연결이 있는 데이터 세트 [!DNL On-premise Analysis] 서비스</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: 로 데이터를 푸시하기 위해 프로그래밍 방식으로 액세스할 수 있는 데이터 세트 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: 데이터 스트리밍을 지원하고 데이터를 로 푸시하기 위해 프로그래밍 방식으로 액세스할 수 있는 데이터 세트입니다 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: 데이터 스트리밍을 지원하는 데이터 세트</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 테이블]</td>
      <td>데이터 세트에 테이블을 추가합니다. 필드의 경우 다음을 참조하십시오. <a href="#Table" class="MCXref_0">테이블 필드</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>데이터 소스를 추가합니다. 필드의 경우 다음을 참조하십시오. <a href="#Data" class="MCXref_0">데이터 소스 필드</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>데이터 세트에 대한 의도적인 정책을 선택하거나 매핑합니다.</p>
        <ul>
          <li>
            <p>[!UICONTROL 없음]</p>
          </li>
          <li>
            <p>[!UICONTROL 기본 FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 테이블 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 이름]</td>
      <td>
        <p>  테이블 이름을 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 열]</td>
      <td>
        <p>열을 추가합니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 이름]</b>
            </p>
            <p>열 이름을 입력(매핑)합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 데이터 유형]</b>
            </p>
            <p>데이터 유형 선택 또는 매핑:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL 정수]</p>
              </li>
              <li>
                <p>[!UICONTROL 부울]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL 형식 문자열]</b>
            </p>
            <p>형식 문자열을 입력(매핑)합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 행]</td>
      <td>행 세부 정보를 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 측정값]</td>
      <td>테이블에 대한 측정값을 추가합니다.</td>
    </tr>
  </tbody>
</table>

##### 데이터 소스 필드

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 데이터베이스]  </td>
      <td>
        <p>사용할 데이터베이스를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>사용할 서버의 이름을 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>사용할 URL을 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 데이터 소스 ID]</td>
      <td>
        <p>  데이터 소스의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 데이터 소스 유형]  </td>
      <td>
        <p>데이터 소스 유형을 선택하거나 매핑합니다. 예: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 게이트웨이 ID]  </td>
      <td>사용할 게이트웨이의 ID를 입력하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 데이터 세트 테이블에서 행 추가 또는 삭제]

이 작업 모듈은 지정된 푸시 데이터 세트 테이블의 행을 추가하거나 삭제합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 테이블 입력]</td>
      <td>옵션을 선택하거나 매핑하여 조정할 테이블이 포함된 데이터 세트를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 데이터 세트 ID]</td>
      <td>추가하거나 삭제할 행이 포함된 데이터 세트의 ID를 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 테이블 이름]  </td>
      <td>
        <p>추가하거나 삭제할 행이 포함된 테이블의 이름을 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>데이터 세트를 소유하는 그룹의 ID를 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 작업 선택]</td>
      <td>
        <p>수행할 작업을 선택하거나 매핑합니다.</p>
        <ul>
          <li>
            <p>[!UICONTROL 행 추가]</p>
          </li>
          <li>
            <p>[!UICONTROL 모든 행 삭제]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 행]</td>
      <td>
        <p>행 필드를 추가합니다.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 키]</b>
            </p>
            <p>키 이름을 입력하거나 매핑합니다.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 필드 유형]</b>
            </p>
            <p>필드 유형을 선택하거나 매핑합니다.</p>
            <ul>
              <li>
                <p>부울</p>
              </li>
              <li>
                <p>일자</p>
              </li>
              <li>
                <p>텍스트</p>
              </li>
              <li>
                <p>숫자</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL 값]</p>
            <p>키 값을 입력하거나 매핑합니다.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 데이터 세트 새로 고침]

이 작업 모듈은 지정된 데이터 세트를 새로 고칩니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 데이터 세트 입력]</td>
      <td>옵션을 선택하거나 매핑하여 새로 고칠 데이터 세트를 선택합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 데이터 세트 ID]</td>
      <td>새로 고침할 데이터 세트의 ID를 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 테이블 이름]  </td>
      <td>
        <p>추가하거나 삭제할 행이 포함된 테이블의 이름을 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>데이터 세트를 소유하는 그룹의 ID를 입력하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 알림 옵션]  </td>
      <td>
        <p>알림 옵션을 선택하거나 매핑합니다.</p>
        <ul>
          <li>
            <p>완료 시 [!UICONTROL Mail]</p>
          </li>
          <li>
            <p>[!UICONTROL 실패 시 메일]</p>
          </li>
          <li>
            <p>[!UICONTROL 알림 없음]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 데이터 세트 삭제]

이 작업 모듈은 데이터 세트를 삭제합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID 입력]</td>
      <td>
        <p>옵션을 선택하거나 매핑하여 삭제할 데이터 세트를 선택합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID]</td>
      <td>
        <p>삭제할 데이터 세트의 ID를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 그룹 ID]  </td>
      <td>삭제하려는 데이터 세트를 소유하는 그룹의 ID를 선택하거나 매핑합니다.</td>
    </tr>
  </tbody>
</table>

### 앱

#### [!UICONTROL 앱 시청]

이 트리거 모듈은 앱이 업데이트될 때 시나리오를 시작합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 목록 앱]

이 검색 모듈은 설치된 모든 앱 목록을 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 앱 보고서 나열]

이 검색 모듈은 지정된 앱에서 모든 보고서 목록을 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앱 ID]</td>
      <td>보고서를 나열할 앱의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 앱 대시보드 나열]

이 검색 모듈은 지정된 앱에서 대시보드 목록을 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앱 ID]</td>
      <td>대시보드를 나열할 앱의 ID를 선택하거나 매핑합니다.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 앱 가져오기]

이 작업 모듈은 지정된 앱의 메타데이터를 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앱 ID]  </td>
      <td>
        <p>검색할 앱의 ID를 선택하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 앱의 보고서 가져오기]

이 작업 모듈은 지정된 앱 보고서의 메타데이터를 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앱 ID]  </td>
      <td>
        <p>검색할 보고서가 포함된 앱의 ID를 선택하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID]</td>
      <td>
        <p>  검색할 보고서의 ID를 선택하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 앱의 대시보드 가져오기]

이 작업 모듈은 지정된 앱 대시보드의 메타데이터를 검색합니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 앱 ID]  </td>
      <td>
        <p>검색할 대시보드가 포함된 앱의 ID를 선택하거나 매핑합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 보고서 ID]</td>
      <td>
        <p>  검색할 대시보드의 ID를 선택하거나 매핑합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

### 기타

#### [!UICONTROL API 호출 만들기]

이 작업 모듈은 [!DNL Power BI] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>연결에 대한 자세한 내용 [!DNL Power BI] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe에 대한 연결 만들기 [!DNL Workfront Fusion] - 기본 지침</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 경로]</p>
      </td>
      <td>
        <p>상대 경로 입력 <code>https://api.powerbi.com</code>. 예: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 메서드]</p>
      </td>
      <td>
        <p>API 호출을 구성하는 데 필요한 [!UICONTROL HTTP] 요청 메서드를 선택합니다. 자세한 내용은 [!UICONTROL HTTP] 요청 메서드를 참조하십시오.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 인증 헤더 및 x-api-key 헤더를 자동으로 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 쿼리 문자열]  </td>
      <td>
        <p>요청 쿼리 문자열을 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
