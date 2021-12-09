# getBizProfile

## ROB Request Respond, Data Mapping, and Issues

In pursuant of ROBA Act 1956, any business conducted in Malaysia must be registered. The APIs provide the information about registration of business entity in Malaysia. 

## How to write message request
Mandatory field must be filled as explained below: 
``` xml
<customerId>your agent code</customerId>
```

Please put your agent code. 

```xml
<customerReferenceNo>TESTING02</customerReferenceNo>
```

## Good Message Request and Respond

=== "Good Message Request"
	```xml
	<soapenv:Envelope
		xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
		xmlns:ws="http://integrasistg.ssm.com.my/InfoService/1/WS">
		<soapenv:Header/>
		<soapenv:Body>
			<ws:getBizProfile>
            <!--Optional:-->
            <header>
               <!--Optional:-->
               <customerId>MBDD</customerId>
               <!--Optional:-->
               <customerReferenceNo>TESTING02</customerReferenceNo>
               <!--Optional:-->
               <customerRequestDate></customerRequestDate>
            </header>
            <!--Optional:-->
            <request>
               <!--Optional:-->
               <supplyBizReq>
                  <!--Optional:-->
                  <checkDigit></checkDigit>
                  <gstAmount></gstAmount>
                  <infoAmount></infoAmount>
                  <!--Optional:-->
                  <invoiceNo></invoiceNo>
                  <!--Optional:-->
                  <ipaddress></ipaddress>
                  <!--Optional:-->
                  <lastUpdateDate></lastUpdateDate>
                  <!--Optional:-->
                  <regNo>000008702</regNo>
                  <!--Optional:-->
                  <remark></remark>
                  <!--Optional:-->
                  <tableId>ROBINFO</tableId>
                  <!--Optional:-->
                  <type>INFOPROFILE</type>
               </supplyBizReq>
            </request>
         </ws:getBizProfile>
		</soapenv:Body>
	</soapenv:Envelope>
	```
=== "Good Message Response"
	```xml
	<soapenv:Envelope
		xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
		xmlns:xsd="http://www.w3.org/2001/XMLSchema"
		xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
		<soapenv:Header/>
		<soapenv:Body>
			<inf:getBizProfileResponse
            xmlns:inf="http://integrasistg.ssm.com.my/InfoService/1/WS"
            xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/">
            <header>
               <customerId>MBDD</customerId>
               <customerReferenceNo>TESTING02</customerReferenceNo>
               <customerRequestDate/>
               <errorCode/>
               <errorMessage/>
               <hostErrorCode/>
               <hostErrorMessage/>
               <requestTimestamp>2021-07-12T12:06:06.658</requestTimestamp>
               <responseTimestamp>2021-07-12T12:06:06.786</responseTimestamp>
            </header>
            <request>
               <supplyInfoReq>
                  <checkDigit/>
                  <gstAmount/>
                  <infoAmount/>
                  <invoiceNo/>
                  <ipaddress/>
                  <regNo>000008702</regNo>
                  <remark/>
                  <tableId>ROBINFO</tableId>
                  <type>INFOPROFILE</type>
               </supplyInfoReq>
            </request>
            <response>
               <getBizProfileReturn xsi:type="inf:businessInfoProfile">
                  <errorMsg/>
                  <infoId>82049285</infoId>
                  <successCode>00</successCode>
                  <robBusinessInfo>
                     <errorMsg/>
                     <infoId/>
                     <successCode>00</successCode>
                     <ammendmentDate>2016-06-29T16:00:00.000Z</ammendmentDate>
                     <checkDigit>T</checkDigit>
                     <description>MENJUAL &amp; MEMBAIKI MOTOSIKAL DAN BASIKAL</description>
                     <endBusinessDate>2022-05-25T16:00:00.000Z</endBusinessDate>
                     <llpName/>
                     <llpNo/>
                     <mainAddress1>C 22, SIN HOE GARDEN</mainAddress1>
                     <mainAddress2/>
                     <mainAddress3/>
                     <mainPostcode>75150</mainPostcode>
                     <mainState>M</mainState>
                     <mainTown>BUKIT BARU</mainTown>
                     <nameType>T</nameType>
                     <ownerCount>1</ownerCount>
                     <postAddress1>C 22, SIN HOE GARDEN</postAddress1>
                     <postAddress2/>
                     <postAddress3/>
                     <postPostcode>75150</postPostcode>
                     <postState>M</postState>
                     <postTown>BUKIT BARU</postTown>
                     <referenceNo>000008702</referenceNo>
                     <registrationDate>1987-05-31T16:00:00.000Z</registrationDate>
                     <registrationName>KENG HENG MOTOR</registrationName>
                     <registrationNo>000008702</registrationNo>
                     <revokeReasonType/>
                     <startBusinessDate>1987-05-31T16:00:00.000Z</startBusinessDate>
                     <status>A</status>
                  </robBusinessInfo>
                  <robOwnershipInfo xsi:nil="true"/>
                  <robOwnershipListInfo>
                     <errorMsg/>
                     <infoId/>
                     <successCode>00</successCode>
                     <robOwnerShipInfos>
                        <robOwnerShipInfos>
                           <address1>C 22 SIN HOE GARDEN</address1>
                           <address2/>
                           <address3/>
                           <ammendmentType>B</ammendmentType>
                           <checkDigit>T</checkDigit>
                           <color>B</color>
                           <createDate>2004-06-18T00:22:23.000Z</createDate>
                           <dob>1959-02-03T16:30:00.000Z</dob>
                           <entryDate>1977-05-04T16:30:00.000Z</entryDate>
                           <gender>L</gender>
                           <idCardNumber>5544416</idCardNumber>
                           <idCardType>K</idCardType>
                           <nationality>MAL</nationality>
                           <newIcNo>590204045159</newIcNo>
                           <othColor/>
                           <othRace/>
                           <ownerName>NG CHING POO</ownerName>
                           <ownershipLink></ownershipLink>
                           <postcode>75150</postcode>
                           <race>C</race>
                           <registrationName>KENG HENG MOTOR</registrationName>
                           <registrationNo>000008702</registrationNo>
                           <state>M</state>
                           <status>A</status>
                           <town>BUKIT BARU</town>
                           <updateDate>2016-06-30T01:39:25.000Z</updateDate>
                        </robOwnerShipInfos>
                     </robOwnerShipInfos>
                  </robOwnershipListInfo>
                  <robBusinessCodeInfo xsi:nil="true"/>
                  <robBusinessCodeListInfo>
                     <errorMsg/>
                     <infoId/>
                     <successCode>00</successCode>
                     <robBusinessCodeInfos>
                        <robBusinessCodeInfos>
                           <businessCode>46431</businessCode>
                           <checkDigit>T</checkDigit>
                           <description>JUALAN BORONG BASIKAL DAN KOMPONEN (TERMASUK ALAT GANTI) DAN AKSESORI</description>
                           <descriptionEnglish>WHOLESALE OF BICYCLES AND THEIR PARTS AND ACCESSORIES</descriptionEnglish>
                           <registrationName>KENG HENG MOTOR</registrationName>
                           <registrationNo>000008702</registrationNo>
                        </robBusinessCodeInfos>
                        <robBusinessCodeInfos>
                           <businessCode>46431</businessCode>
                           <checkDigit>T</checkDigit>
                           <description>JUALAN BORONG BASIKAL DAN KOMPONEN (TERMASUK ALAT GANTI) DAN AKSESORI</description>
                           <descriptionEnglish>WHOLESALE OF BICYCLES AND THEIR PARTS AND ACCESSORIES</descriptionEnglish>
                           <registrationName>KENG HENG MOTOR</registrationName>
                           <registrationNo>000008702</registrationNo>
                        </robBusinessCodeInfos>
                     </robBusinessCodeInfos>
                  </robBusinessCodeListInfo>
                  <robBranchInfo xsi:nil="true"/>
                  <robBranchListInfo>
                     <errorMsg>No Data</errorMsg>
                     <infoId/>
                     <successCode>11</successCode>
                     <robBranchInfos/>
                  </robBranchListInfo>
               </getBizProfileReturn>
            </response>
         </inf:getBizProfileResponse>
		</soapenv:Body>
	</soapenv:Envelope>
	```



## Understanding the biz owner ID number


## Two IC number, both old and new

* Some of the owner carries two IC numbers which are both old and new
* The new IC number is stored in newIcNo
* old IC number is stored in idCardNumber
* idCardType is always K

Sample ROB number
* No. ROB = 000008702

~~~~~~ xml
<idCardNumber>5544416</idCardNumber>
<idCardType>K</idCardType>
<nationality>MAL</nationality>
<newIcNo>590204045159</newIcNo>
~~~~~~

## New IC number 

Most of business owner carries only one type of IC, which is new IC number.
* idCardType is always K,
* but idCardNumber is empty,
* newIcNo has value.

Sample Rob Number
* No. ROB =  TR0215204
~~~~~~ xml
<dob>1981-10-04T16:30:00.000Z</dob>
<entryDate>2020-06-29T16:00:00.000Z</entryDate>
<gender>P</gender>
<idCardNumber/>
<idCardType>K</idCardType>
<nationality>MAL</nationality>
<newIcNo>811005065524</newIcNo>
<othColor/>
<othRace/>
<ownerName>NORSHAFIZAN BINTI ENDOT</ownerName>
~~~~~~

## Recommendation

It is our recommendation to check newIcNo for ID number, if there's no newIcNo then check idCardNumber and refer to idCardType for ID number. 


## Rare Cases of ROB 

