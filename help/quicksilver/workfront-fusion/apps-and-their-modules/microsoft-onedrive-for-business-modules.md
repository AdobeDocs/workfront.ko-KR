---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 비즈니스용 Microsoft OneDrive 모듈
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1257'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business]개 모듈

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [비즈니스용 Microsoft OneDrive 모듈](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-onedrive-for-business-modules.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Microsoft OneDrive for Business]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요하면 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)을 참조하세요.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
  <td> <p>[!UICONTROL Pro] 이상</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 전제 조건

[!DNL Adobe Workfront Fusion]에 [!DNL Microsoft OneDrive for Business]을(를) 사용하려면 [!DNL Microsoft] 계정이 필요합니다.

[!DNL OneDrive for Business] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 [Adobe에 연결 만들기 [!DNL Workfront Fusion] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)을 참조하세요.



## [!DNL Workfront Fusion]에 [!DNL Microsoft OneDrive for Business] 서비스를 연결하는 중

[!DNL Microsoft OneDrive for Business] 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법에 대한 지침은 [[!UICONTROL Adobe Workfront Fusion에 연결 만들기] - 기본 지침](../../workfront-fusion/connections/connect-to-fusion-general.md)을 참조하십시오.

>[!NOTE]
>
>일부 Microsoft 앱은 개별 사용자 권한에 연결된 동일한 연결을 사용합니다. 따라서 연결을 만들 때 권한 동의 화면에는 현재 애플리케이션에 필요한 새 권한 외에도 이 사용자의 연결에 대해 이전에 부여된 모든 권한이 표시됩니다.
>
>예를 들어 사용자가 Excel 커넥터를 통해 부여된 &quot;테이블 읽기&quot; 권한을 가지고 있는 다음 Outlook 커넥터에서 연결을 만들어 이메일을 읽은 경우 권한 동의 화면에 이미 부여된 &quot;테이블 읽기&quot; 권한과 새로 필요한 &quot;이메일 쓰기&quot; 권한이 모두 표시됩니다.

## [!DNL Microsoft OneDrive for Business]개 모듈 및 해당 필드

[!DNL Microsoft OneDrive for Business] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Microsoft OneDrive for Business] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)

### 트리거

* [[!UICONTROL 파일 보기]](#watch-files)
* [[!UICONTROL 폴더 보기]](#watch-folders)

#### [!UICONTROL 파일 보기]

이 트리거 모듈은 감시되는 폴더에 새 파일이 추가되거나 업데이트될 때 활성화됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 드라이브 ID]</p> </td> 
   <td> <p>보려는 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더]</td> 
   <td> <p> 보려는 폴더를 선택합니다. 시나리오 내에서는 한 폴더만 모니터링할 수 있습니다.</p> <p>팁: 여러 폴더를 추적하려면 각 폴더에 대해 독립적인 시나리오를 만드십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보고 싶습니다]</p> </td> 
   <td> <p>새 파일 및 모든 변경 내용을 볼지 아니면 새 파일만 볼지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 행 수]</td> 
   <td> <p> 한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 보기]

이 트리거 모듈은 새 폴더가 감시 중인 폴더에 추가되면 활성화됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 드라이브 ID]</p> </td> 
   <td> <p>보려는 드라이브를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더]</td> 
   <td> <p> 보려는 폴더를 선택합니다. 시나리오 내에서는 한 폴더만 모니터링할 수 있습니다.</p> <p>팁: 여러 폴더를 추적하려면 각 폴더에 대해 독립적인 시나리오를 만드십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 보고 싶습니다]</p> </td> 
   <td> <p>새 폴더와 모든 변경 사항을 볼 것인지 새 폴더만 볼 것인지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 행 수]</td> 
   <td> <p> 한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 파일 업로드]](#upload-a-file)
* [[!UICONTROL 파일 삭제]](#delete-a-file)
* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 폴더 삭제]](#delete-a-folder)
* [[!UICONTROL 공유 링크 가져오기]](#get-a-sharing-link)

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 이진 또는 텍스트 파일을 지정된 폴더로 업로드합니다

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 업로드할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>드라이브 내의 폴더를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source 파일]</p> </td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 이름이 같은 파일이 있는 경우]</td> 
   <td> <p> 업로드하려는 파일과 이름이 같은 파일이 이미 있는 경우 수행할 작업을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 기존 파일 바꾸기]</li> 
     <li>[!UICONTROL 새 파일 이름 바꾸기]</li> 
     <li>[!UICONTROL 오류와 함께 종료]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 삭제]

이 작업 모듈은 지정된 파일을 휴지통으로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 삭제할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p>삭제할 파일의 ID를 입력합니다. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

이 작업 모듈은 특정 ID로 파일을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 검색할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 ID]</td> 
   <td> <p>검색할 파일의 ID를 입력합니다. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

지정된 상위 폴더 내에 폴더를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL 연결]</strong> </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL 드라이브 ID]</strong> </td> 
   <td> <p>새 폴더를 만들 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL 폴더]</strong> </td> 
   <td> <p>새 폴더를 만들 폴더를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL 폴더 이름]</strong> </td> 
   <td>새 폴더의 이름을 입력하거나 매핑합니다.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 삭제]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 삭제할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더 ID]</td> 
   <td> <p>삭제하려는 폴더의 ID를 입력하거나 매핑합니다. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 공유 링크 가져오기]

이 모듈은 지정된 파일에 대한 액세스 권한을 제공하기 위해 공유할 수 있는 링크를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 만들기 문서에서 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 드라이브 ID]</td> 
   <td> <p>파일을 업로드할 드라이브를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>파일 ID를 사용하여 파일을 선택할지 파일 경로를 사용하여 파일을 선택할지 선택합니다. 표시되는 필드에 파일 ID 또는 경로를 입력합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 권한 유형]</p> </td> 
   <td> <p>링크를 받는 사람에게 읽기/쓰기 권한을 부여할지 아니면 읽기 전용을 부여할지 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 범위]</td> 
   <td> <p> 링크를 가진 모든 사용자가 파일에 액세스할 수 있는지 또는 조직 구성원만 액세스할 수 있는지 여부를 선택합니다.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
