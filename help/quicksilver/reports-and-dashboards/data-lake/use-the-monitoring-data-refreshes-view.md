---
product-area: reports and dashboards
navigation-topic: data-connect
title: Data Connect에서 데이터 새로 고침 모니터링 보기 사용
description: Workfront 관리자는 Data Connect를 사용하여 최근 새로 고치는 동안 데이터 레이크 날짜에 수행된 최근 업데이트에 대한 세부 레코드에 액세스할 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: 230d1a30-2af9-4d2c-9ec1-34c3d4c080d4
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# Data Connect에서 데이터 새로 고침 모니터링 보기 사용

데이터 새로 고침 모니터링 보기에는 최근 새로 고침 도중 데이터 레이크 날짜에 수행된 최근 업데이트가 표시됩니다. 이 보기의 데이터는 데이터 로드가 성공적으로 완료될 때마다 업데이트됩니다.

데이터 양이 많고 집계의 복잡성으로 인해 데이터 새로 고침 모니터링 보기에는 지난 2주 내에 업데이트된 개체 보기만 표시됩니다. 이 보기에 특정 레코드 유형이 없는 경우 해당 기간 내에 활동이 없기 때문일 수 있습니다.

>[!NOTE]
>
>이 보기는 새로 고침 활동 내역을 표시하는 일별 내역 또는 이벤트 보기와 달리 애플리케이션 및 새로 고침 활동에서 제공한 데이터의 세부 컬렉션을 표시합니다. 내역 새로 고침 활동 세부 정보를 얻으려면 <code>DL_LOAD_TIMESTAMP를 사용할 수 있습니다.</code> date 객체

## 데이터 새로 고침 보기 열 모니터링

데이터 새로 고침 모니터링 보기 열에는 다음 정보가 포함됩니다.

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
        <td>CALENDAR_날짜 </td>
        <td>일자</td>
        <td>
   OBJ_TYPE 열에 표시된 객체 유형에 대해 마지막으로 성공한 데이터 새로 고침의 날짜입니다. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 OBJ_TYPE 열에 표시된 객체 유형에 대한 최근 데이터 새로 고침 날짜 및 시간입니다.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       OBJ_TYPE 열에 표시된 객체 유형에 대한 두 번째 최근 데이터 새로 고침의 날짜와 시간입니다. </td>
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
        <td>객체 유형에 대한 이전 및 최신 데이터 새로 고침 사이에 캡처된 CREATE 레코드 이벤트 수.  </td>
    </tr>
                <tr>
        <td>업데이트됨</td>
        <td>숫자 </td>
        <td>객체 유형에 대한 이전 및 최신 데이터 새로 고침 사이에 캡처된 UPDATE 레코드 이벤트 수.</td>
    </tr>
                <tr>
        <td>삭제됨</td>
        <td>숫자 </td>
        <td>개체 유형에 대한 이전 및 최신 데이터 새로 고침 사이에 캡처된 DELETE 레코드 이벤트 수입니다. </td>
    </tr>
                <tr>
        <td>합계</td>
        <td>숫자 </td>
        <td>객체 유형에 대한 이전 데이터 새로 고침과 최신 데이터 새로 고침 사이의 총 이벤트 수입니다. 
        <br> 
        <br><b>참고</b>: 새로 고침 간격 내에 같은 레코드를 여러 번 만들고 업데이트할 수 있으므로 CREATE, UPDATE 또는 DELETE 이벤트의 영향을 받은 총 레코드 수와 다릅니다.  </td>
    </tr>
   </table>
