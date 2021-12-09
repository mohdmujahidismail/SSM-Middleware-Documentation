# getLlpCurrentProfile

## Limited Liability Partnership Request Respond, Data Mapping, and Issues

## Message Reference

<table class="tableizer-table">
  <thead>
    <tr class="tableizer-firstrow">
      <th>Type</th>
      <th>Description</th>
      <th>Mandatory?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>JSON message header</td>
      <td>JSON.Msg.Body.getLlpCurrentProfile.header<br> An information header of the message request.</td>
      <td>YES </td>
    </tr>
    <tr>
      <td>JSON request body</td>
      <td>JSON.Msg.Body.getLlpCurrentProfile.request.param<br> An information of request parameter</td>
      <td>YES</td>
    </tr>
    <tr>
      <td>JSON good response body</td>
      <td>JSON.Msg.Body.getLlpCurrentProfile.response.getLlpCurrentProfileReturn<br> An information of message response</td>
      <td>YES</td>
    </tr>
    <tr>
      <td>Host response body</td>
      <td>JSON.Msg.Body.getLlpCurrentProfileResponse.getLlpCurrentProfileReturn<br> An information of response based on host service</td>
      <td>YES</td>
    </tr>
  </tbody>
</table>

## Request Message Mapping
Refer Request Message mapping in Common Header Format

<table class="tableizer-table">
  <thead>
    <tr class="tableizer-firstrow">
      <th>S/N</th>
      <th>Request Body</th>
      <th>Description </th>
      <th>Type</th>
      <th>Length</th>
      <th>Req?</th>
      <th>Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>&nbsp;</td>
      <td>Customer Id</td>
      <td>An information of customer Id</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>2.</td>
      <td>&nbsp;</td>
      <td>Customer Reference No</td>
      <td>An information of customer reference number </td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>&nbsp;</td>
      <td>Customer Request Date</td>
      <td>An information that customer request date</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>4.</td>
      <td>&nbsp;</td>
      <td>Entity No</td>
      <td>An information of LLP entity number</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td></td>
    </tr>
  </tbody>
</table>

## Sample Request Message
Web Service - REST Request Message

```json
	{
        "header":{
        "customerId":"MBDD",
        "customerReferenceNo":"MBDDtest",
        "customerRequestDate":"2021-09-02T10:00:00Z"
        },
        "request":{
        "entityNo":"LLP0028160-LGN"
   	    }
    }
```

## Response Message mapping (Good Response)
Refer Response Message mapping in Common Header Format.
##### Response mapping Header
<table class="tableizer-table">
  <thead>
    <tr class="tableizer-firstrow">
      <th>S/N</th>
      <th>Response Body (header)</th>
      <th>Description</th>
      <th>Type</th>
      <th>Length</th>
      <th>Req?</th>
      <th>Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>&nbsp;</td>
      <td>Customer Id</td>
      <td>An information of customer identification Id</td>
      <td>String</td>
      <td></td>
      <td rowspan="11"></td>
    </tr>
    <tr>
      <td>2.</td>
      <td>&nbsp;</td>
      <td>Customer Reference No</td>
      <td>An information of customer reference number</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>&nbsp;</td>
      <td>Customer Request Date</td>
      <td>An information that customer request date</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>4.</td>
      <td>&nbsp;</td>
      <td>Request Timestamp</td>
      <td>An information of customer's LLP request timestamp </td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>5.</td>
      <td>&nbsp;</td>
      <td>Response Timestamp</td>
      <td>An information of customer's LLP response timestamp</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>6.</td>
      <td>&nbsp;</td>
      <td>Record Count</td>
      <td>An information of LLP record count within its service</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>7.</td>
      <td>&nbsp;</td>
      <td>Error Code</td>
      <td>An information if LLP details has error</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>8.</td>
      <td>&nbsp;</td>
      <td>Error Message</td>
      <td>An information if LLP's details has error message</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>9.</td>
      <td>&nbsp;</td>
      <td>Host Error Code</td>
      <td>An information if LLP's details has host error code</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>10.</td>
      <td>&nbsp;</td>
      <td>Host Error Message</td>
      <td>An information if LLP's details has host error message</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>11.</td>
      <td>&nbsp;</td>
      <td>Operation Name</td>
      <td>An information if LLP has operation name</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
  </tbody>
</table>

##### Response mapping Body (request)

<table class="tableizer-table">
  <thead>
    <tr class="tableizer-firstrow">
      <th>S/N</th>
      <th>Response Body (request)</th>
      <th>Description </th>
      <th>Type</th>
      <th>Length</th>
      <th>Req?</th>
      <th>Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>&nbsp;</td>
      <td>Entity No</td>
      <td>An information of company entity number</td>
      <td>String</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>2.</td>
      <td>&nbsp;</td>
      <td>Llp Current Profile</td>
      <td>An information of LLP current profile</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>&nbsp;</td>
      <td>Llp Basic Profile</td>
      <td>An information of LLP basic profile</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>4.</td>
      <td>&nbsp;</td>
      <td>Entity Name</td>
      <td>An information of company name</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>5.</td>
      <td>&nbsp;</td>
      <td>Entity No New Format</td>
      <td>An information of new format of company entity number</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>6.</td>
      <td>&nbsp;</td>
      <td>Entity Status</td>
      <td>An information of company status</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>7.</td>
      <td>&nbsp;</td>
      <td>Entity Status Dt</td>
      <td>An information of company status date</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>8.</td>
      <td>&nbsp;</td>
      <td>Entity Status Desc</td>
      <td>An information of company status description</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>9.</td>
      <td>&nbsp;</td>
      <td>Entity Type</td>
      <td>An information of company type</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>10.</td>
      <td>&nbsp;</td>
      <td>Entity Type Desc</td>
      <td>An information of company type description</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>11.</td>
      <td>&nbsp;</td>
      <td>Entity Reg Dt</td>
      <td>An information of company registration date</td>
      <td> String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>12.</td>
      <td>&nbsp;</td>
      <td>Entity Email</td>
      <td>An information of company's email</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>13.</td>
      <td>&nbsp;</td>
      <td>Entity Update Dt</td>
      <td>An information of company update date (backend use)</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>14.</td>
      <td>&nbsp;</td>
      <td>Last Return Dt</td>
      <td>An information of company last return date </td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>15.</td>
      <td>&nbsp;</td>
      <td>Next Return Dt</td>
      <td>An information of company next return date </td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>16.</td>
      <td>&nbsp;</td>
      <td>Due Return Dt</td>
      <td>An information of company due return date</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>17.</td>
      <td>&nbsp;</td>
      <td>Reg Nature Of Biz</td>
      <td>An information of register of identity company business</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>18.</td>
      <td>&nbsp;</td>
      <td>Old Name</td>
      <td>An information of company old name</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>19.</td>
      <td>&nbsp;</td>
      <td>Name Change Dt</td>
      <td>An information of company changing name date</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>20.</td>
      <td>&nbsp;</td>
      <td>Origin</td>
      <td>An information of company origin location</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>21.</td>
      <td>&nbsp;</td>
      <td>Origin Desc</td>
      <td>An information of company origin location description </td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>22.</td>
      <td>&nbsp;</td>
      <td>Llp Conversion</td>
      <td>An information of LLP conversion statement (backend use)</td>
      <td>String</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
  </tbody>
</table>

##### Response mapping Body (reqBizAddress) 

<table class="tableizer-table">
  <thead>
    <tr class="tableizer-firstrow">
      <th>S/N</th>
      <th>Response Body (regBizAddresses)</th>
      <th>Description </th>
      <th>Type</th>
      <th>Length</th>
      <th>Req?</th>
      <th>Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>&nbsp;</td>
      <td>Address 1</td>
      <td>An information of company address</td>
      <td>String</td>
      <td></td>
      <td rowspan="11"></td>
    </tr>
    <tr>
      <td>2.</td>
      <td>&nbsp;</td>
      <td>Address 2</td>
      <td>An information of company address </td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>&nbsp;</td>
      <td>Address 3</td>
      <td>An information of company address</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>4.</td>
      <td>&nbsp;</td>
      <td>Postcode</td>
      <td>An information of company postcode location</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>5.</td>
      <td>&nbsp;</td>
      <td>City</td>
      <td>An information of city of company</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>6.</td>
      <td>&nbsp;</td>
      <td>State</td>
      <td>An information of company state (backend use)</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>7.</td>
      <td>&nbsp;</td>
      <td>State Desc</td>
      <td>An information of company state description</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>8.</td>
      <td>&nbsp;</td>
      <td>Country</td>
      <td>An information of company country (backend use)</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>9.</td>
      <td>&nbsp;</td>
      <td>Country Desc</td>
      <td>An information of company country description print as Malaysia</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>10.</td>
      <td>&nbsp;</td>
      <td>PrincipalInd</td>
      <td>&nbsp;</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <td>11.</td>
      <td>&nbsp;</td>
      <td>PrincipalInd Desc</td>
      <td>&nbsp;</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
  </tbody>
</table>

##### Response mapping Body (bizCodes) 

<table class="tableizer-table">
  <thead>
    <tr class="tableizer-firstrow">
      <th>S/N</th>
      <th>Response Body (bizCodes)</th>
      <th>Description </th>
      <th>Type</th>
      <th>Length</th>
      <th>Req?</th>
      <th>Remarks</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>&nbsp;</td>
      <td>Entity Biz Code</td>
      <td>An information of company business code</td>
      <td>String</td>
      <td></td>
      <td rowspan="2"></td>
    </tr>
    <tr>
      <td>2.</td>
      <td>&nbsp;</td>
      <td>Entity Biz Code Desc</td>
      <td>An information of company business code description</td>
      <td>String</td>
      <td>&nbsp;</td>
    </tr>
  </tbody>
</table>

## Sample Good Response Message 
Web Service - REST Response Message
```json
	   {
          "header":{
          "customerId":null,
          "customerReferenceNo":null,
          "customerRequestDate":null,
          "requestTimestamp":null,
          "responseTimestamp":null,
          "recordCount":null,
          "errorCode":"00",
          "errorMessage":null,
          "hostErrorCode":null,
          "hostErrorMessage":null,
          "operationName":null
        },
           "request":{
              "entityNo":"LLP0028160-LGN"
           },
           "llpCurrentProfile":{
              "llpBasicProfile":{
                 "entityName":"PROPPY CF  PLT",
                 "entityNo":"LLP0028160-LGN",
                 "entityNoNewFormat":"202104001531",
                 "entityStatus":"1",
                 "entityStatusDt":"2021-05-11T14:34:35.000Z",
                 "entityStatusDesc":"EXISTING",
                 "entityType":"1",
                 "entityTypeDesc":"LOCAL REGISTRATION",
                 "entityRegDt":"2021-05-11T14:34:35.000Z",
                 "entityEmail":"",
                 "entityUpdateDt":"2021-09-27T16:52:48.000Z",
                 "lastReturnDt":"",
                 "nextReturnDt":"2022-11-11T00:00:00.000Z",
                 "dueReturnDt":"2022-11-11T00:00:00.000Z",
                 "regNatureOfBiz":null,
                 "oldName":"",
                 "nameChangeDt":"",
                 "origin":"MYS",
                 "originDesc":"MALAYSIA",
                 "llpConversion":null
              },
              "regOfficeAdd":{
                 "address1":"LOT 3.33, 3.40 & 3.41, 3RD FLOOR",
                 "address2":"VIVA SHOPPING MALL",
                 "address3":"NO. 85 JALAN LOKE YEW",
                 "postcode":"55200",
                 "city":"KUALA LUMPUR",
                 "state":"W",
                 "stateDesc":"W.P KUALA LUMPUR",
                 "country":"MYS",
                 "countryDesc":"MALAYSIA",
                 "principalInd":null,
                 "principalIndDesc":null
              },
              "regBizAddresses":[
                 {
                    "address1":"LOT 3.33, 3.40 & 3.41, 3RD FLOOR",
                    "address2":"VIVA SHOPPING MALL",
                    "address3":"NO. 85 JALAN LOKE YEW",
                    "postcode":"55200",
                    "city":"KUALA LUMPUR",
                    "state":"W",
                    "stateDesc":"W.P KUALA LUMPUR",
                    "country":"MYS",
                    "countryDesc":"MALAYSIA",
                    "principalInd":"Y",
                    "principalIndDesc":"YES"
                 }
              ],
              "involvements":[
                 {
                    "involveType":"CO",
                    "involveTypeDesc":"COMPLIANCE OFFICER",
                    "involveName":"CHEN FOCK SIONG",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"750602145665",
                    "involveEffectiveFromDt":"2021-05-11T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"NO 9, JALAN PP 55 SEKS 2",
                       "address2":"TAMAN PENGGIRAN PUTRA",
                       "address3":"BANDAR PUTRA PERMAI",
                       "postcode":"43300",
                       "city":"SERI KEMBANGAN",
                       "state":"B",
                       "stateDesc":"SELANGOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"LEE WILSON",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"720209015023",
                    "involveEffectiveFromDt":"2021-05-11T07:47:59.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"A1-32-1, MYHABITAT",
                       "address2":"NO. 3, JALAN AMAN",
                       "address3":"OFF JALAN TUN RAZAK",
                       "postcode":"55000",
                       "city":"KUALA LUMPUR",
                       "state":"W",
                       "stateDesc":"W.P KUALA LUMPUR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"LEONG EE MUN, SHARON",
                    "involveIdType":"05",
                    "involveIdTypeDesc":"PASSPORT",
                    "involveId":"K2156533P",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"23 JALAN KIA PENG",
                       "address2":"AMPERSAND CONDO UMT C-1-3",
                       "address3":null,
                       "postcode":"50450",
                       "city":"KUALA LUMPUR",
                       "state":"W",
                       "stateDesc":"W.P KUALA LUMPUR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"CHONG NYOK HOON",
                    "involveIdType":"05",
                    "involveIdTypeDesc":"PASSPORT",
                    "involveId":"S7463104E",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"BLK 249 KIM KEAT LINK",
                       "address2":"#06-73 310249",
                       "address3":null,
                       "postcode":null,
                       "city":null,
                       "state":null,
                       "stateDesc":null,
                       "country":"SGP",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"TSUN CHIN ENG",
                    "involveIdType":"05",
                    "involveIdTypeDesc":"PASSPORT",
                    "involveId":"S7977504E",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"547A SEGAR ROAD",
                       "address2":"#14-77 671547",
                       "address3":null,
                       "postcode":null,
                       "city":null,
                       "state":null,
                       "stateDesc":null,
                       "country":"SGP",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"TOH JIA XIN",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"880929045426",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"NO 6 JALAN RIA 1",
                       "address2":"TAMAN RIA",
                       "address3":"KAMPUNG JAWA",
                       "postcode":"85000",
                       "city":"SEGAMAT",
                       "state":"J",
                       "stateDesc":"JOHOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"BOK CHICK SHIM",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"880602566262",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"136 LORONG LASSIM",
                       "address2":"JALAN HAJI ABDULLAH",
                       "address3":null,
                       "postcode":"84000",
                       "city":"MUAR",
                       "state":"J",
                       "stateDesc":"JOHOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"CHEN FOCK SIONG",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"750602145665",
                    "involveEffectiveFromDt":"2021-05-11T07:47:59.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"NO 9, JALAN PP 55 SEKS 2",
                       "address2":"TAMAN PENGGIRAN PUTRA",
                       "address3":"BANDAR PUTRA PERMAI",
                       "postcode":"43300",
                       "city":"SERI KEMBANGAN",
                       "state":"B",
                       "stateDesc":"SELANGOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"CHONG YEE THENG",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"801020015913",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"NO.32 JALAN JASA 54",
                       "address2":"TAMAN MUTIARA RINI",
                       "address3":null,
                       "postcode":"81300",
                       "city":"SKUDAI",
                       "state":"J",
                       "stateDesc":"JOHOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"WILLIAM MAN MAO WAH",
                    "involveIdType":"05",
                    "involveIdTypeDesc":"PASSPORT",
                    "involveId":"538682847",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"C-LG-2 JALAN BAYU 3",
                       "address2":"BUKIT GITA BAYU",
                       "address3":"SERDANG",
                       "postcode":"43300",
                       "city":"SERI KEMBANGAN",
                       "state":"B",
                       "stateDesc":"SELANGOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"SASHEKUMAR A/L MUNIANDY",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"790523085533",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"B-13-11 BLOCK B PERDANA EXCLUSIVE CONDO",
                       "address2":"JALAN PJU 8/1 DAMANSARA PERDANA",
                       "address3":null,
                       "postcode":"47820",
                       "city":"PETALING JAYA",
                       "state":"B",
                       "stateDesc":"SELANGOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"CHOW KEAN WAI",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"760529065317",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"A-3894 LORONG ALOR AKAR 14",
                       "address2":"JALAN ALOR AKAR",
                       "address3":null,
                       "postcode":"25250",
                       "city":"KUANTAN",
                       "state":"C",
                       "stateDesc":"PAHANG",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"FUNG JUI SENG",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"750309017197",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"282-10 LORONG DATO AHMAD",
                       "address2":"JALAN KHALIDI",
                       "address3":null,
                       "postcode":"84000",
                       "city":"MUAR",
                       "state":"J",
                       "stateDesc":"JOHOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"YAP YIK YEE",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"741108145657",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"6 JALAN CHIN CHIN",
                       "address2":"OFF LORONG LOKE YEW",
                       "address3":null,
                       "postcode":"55200",
                       "city":"KUALA LUMPUR",
                       "state":"W",
                       "stateDesc":"W.P KUALA LUMPUR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"NGOW E-VAN @ EVAN NGOW",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"731121015081",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"1408 JALAN 17/26",
                       "address2":null,
                       "address3":null,
                       "postcode":"46400",
                       "city":"PETALING JAYA",
                       "state":"B",
                       "stateDesc":"SELANGOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"LEE SENG YEOW",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"721007015767",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"B1205 PERDANA VIEW CONDO",
                       "address2":"NO. 21 JALAN PJU 8/1",
                       "address3":"BANDAR DAMANSARA PERDANA",
                       "postcode":"47820",
                       "city":"PETALING JAYA",
                       "state":"B",
                       "stateDesc":"SELANGOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"TAN KIM CHONG",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"720124015315",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"7 JALAN AMAN CERIA 3",
                       "address2":"BANDAR TROPICANA AMAN",
                       "address3":null,
                       "postcode":"42500",
                       "city":"TELOK PANGLIMA GARANG",
                       "state":"B",
                       "stateDesc":"SELANGOR",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 },
                 {
                    "involveType":"PT",
                    "involveTypeDesc":"PARTNER",
                    "involveName":"NG KIM MOI",
                    "involveIdType":"01",
                    "involveIdTypeDesc":"NRIC",
                    "involveId":"651127055420",
                    "involveEffectiveFromDt":"2021-07-21T00:00:00.000Z",
                    "involveEffectiveToDt":"",
                    "entityNo":"LLP0028160-LGN",
                    "entityName":null,
                    "entityNoNewFormat":null,
                    "entityStatus":null,
                    "entityStatusDesc":null,
                    "address":{
                       "address1":"LOT 4280 TAMAN BUKIT PELANDOK",
                       "address2":null,
                       "address3":null,
                       "postcode":"71960",
                       "city":"PORT DICKSON",
                       "state":"N",
                       "stateDesc":"NEGERI SEMBILAN",
                       "country":"MYS",
                       "countryDesc":null,
                       "principalInd":null,
                       "principalIndDesc":null
                    }
                 }
              ],
              "bizCodes":[
                 {
                    "entityBizCode":"64200",
                    "entityBizCodeDesc":"ACTIVITIES OF HOLDING COMPANIES"
                 }
              ]
           }
        } 
```