---
product-area: reports and dashboards
navigation-topic: data-connect
title: Data Connect에서 데이터 새로 고침 모니터링 보기 사용
description: Workfront 관리자는 Data Connect를 통해 가장 최근 새로 고침 중에 데이터 레이크 날짜에 수행된 최근 업데이트에 대한 세부 기록에 액세스할 수 있습니다.
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# Data Connect에서 데이터 새로 고침 모니터링 보기 사용

데이터 새로 고침 모니터링 보기에는 가장 최근 새로 고침 중에 데이터 레이크 날짜에 대해 수행된 최근 업데이트가 표시됩니다. 이 보기의 데이터는 데이터 로드가 성공적으로 완료되면 업데이트됩니다.

많은 양의 데이터와 집계의 복잡성으로 인해 데이터 새로 고침 모니터링 보기에는 지난 2주 이내에 업데이트된 개체 보기만 표시됩니다. 이 보기에 특정 레코드 종류가 없는 경우 해당 기간 내의 활동 부족 때문일 수 있습니다.

>[!NOTE]
>
>이 보기는 새로 고침 활동 내역을 표시하는 일별 내역 또는 이벤트 보기와 반대로 응용 프로그램 및 새로 고침 활동에서 제공하는 데이터의 세부 모음을 표시합니다. 내역 새로 고침 활동 세부 정보를 가져오려면 <code>DL_LOAD_TIMESTAMP를 사용합니다</code> date 객체.

## 데이터 새로 고침 모니터링 뷰 열

모니터링 데이터 새로 고침 보기 열에는 다음 정보가 포함되어 있습니다.

<table>
    <tr>
        <td><b>열 이름</b></td>
        <td><b>유형</b></td>
        <td><b>설명</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      데이터 레이크로 전송된 Workfront 레코드와 연결된 개체 유형입니다. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Date</td>
        <td>
   OBJ_TYPE 열에 표시된 객체 유형에 대해 마지막으로 성공한 데이터 새로 고침 날짜입니다. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 OBJ_TYPE 열에 표시되는 객체 유형에 대한 가장 최근 데이터 새로 고침 날짜 및 시간입니다.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       OBJ_TYPE 열에 표시되는 객체 유형에 대한 두 번째 가장 최근 데이터 새로 고침 날짜 및 시간입니다. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>숫자</td>
        <td>
     객체 유형에 대한 마지막 데이터 새로 고침 이후 경과된 시간(분)입니다. </td>
    </tr>
            <tr>
        <td>생성됨 </td>
        <td>숫자 </td>
        <td>객체 유형에 대한 이전 및 최신 데이터 새로 고침 사이에 캡처된 CREATE 레코드 이벤트 수입니다.  </td>
    </tr>
                <tr>
        <td>업데이트됨</td>
        <td>숫자 </td>
        <td>객체 유형에 대한 이전 및 최신 데이터 새로 고침 사이에 캡처된 UPDATE 레코드 이벤트 수입니다.</td>
    </tr>
                <tr>
        <td>삭제됨</td>
        <td>숫자 </td>
        <td>오브젝트 유형에 대한 이전 및 최신 데이터 새로 고침 사이에 캡처된 DELETE 레코드 이벤트 수입니다. </td>
    </tr>
                <tr>
        <td>합계</td>
        <td>숫자 </td>
        <td>객체 유형에 대한 이전 및 최신 데이터 새로 고침 간의 총 이벤트 수 카운트입니다. 
        <br> 
        <br><b>참고</b>: 새로 고침 간격 내에 동일한 레코드가 여러 번 만들어지고 업데이트될 수 있으므로 CREATE, UPDATE 또는 DELETE 이벤트의 영향을 받은 총 레코드 수와 다릅니다.  </td>
    </tr>
   </table>

