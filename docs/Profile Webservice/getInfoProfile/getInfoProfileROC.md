# getInfoProfile ROC

## ROC Request Respond, Data Mapping, and Issues

## How to write message request
Mandatory field must be filled as explained below: 
~~~~~~ xml
<customerId>your agent code</customerId>
~~~~~~
Please put your agent code. 

~~~~~~ xml
<customerReferenceNo>TESTING02</customerReferenceNo>
~~~~~~

## Good Message Request & Respond

=== "Good Message Request"

    ``` xml
         <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ws="http://integrasistg.ssm.com.my/InfoService/1/WS">
            <soapenv:Header/>
            <soapenv:Body>
               <ws:getInfoProfile>
                  <!--Optional:-->
                  <header>
                     <!--Optional:-->
                     <customerId>MBDD</customerId>
                     <!--Optional:-->
                     <customerReferenceNo>Testing02</customerReferenceNo>
                     <!--Optional:-->
                     <customerRequestDate></customerRequestDate>
                  </header>
                  <!--Optional:-->
                  <request>
                     <!--Optional:-->
                     <supplyInfoReq>
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
                        <regNo>6386</regNo>
                        <!--Optional:-->
                        <remark></remark>
                        <!--Optional:-->
                        <tableId>ROCINFO</tableId>
                        <!--Optional:-->
                        <type>INFOPROFILE</type>
                     </supplyInfoReq>
                  </request>
               </ws:getInfoProfile>
            </soapenv:Body>
         </soapenv:Envelope>
    ```

=== "Good Message Response"

    ``` xml
         <soapenv:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
            <soapenv:Header/>
            <soapenv:Body>
               <inf:getInfoProfileResponse xmlns:inf="http://integrasistg.ssm.com.my/InfoService/1/WS" xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/">
                  <header>
                     <customerId>MBDD</customerId>
                     <customerReferenceNo>Testing02</customerReferenceNo>
                     <customerRequestDate/>
                     <errorCode/>
                     <errorMessage/>
                     <hostErrorCode/>
                     <hostErrorMessage/>
                     <requestTimestamp>2021-11-25T14:40:26.291</requestTimestamp>
                     <responseTimestamp>2021-11-25T14:40:26.894</responseTimestamp>
                  </header>
                  <request>
                     <supplyInfoReq>
                        <checkDigit/>
                        <gstAmount/>
                        <infoAmount/>
                        <invoiceNo/>
                        <ipaddress/>
                        <regNo>6386</regNo>
                        <remark/>
                        <tableId>ROCINFO</tableId>
                        <type>INFOPROFILE</type>
                     </supplyInfoReq>
                  </request>
                  <response>
                     <getInfoProfileReturn xsi:type="inf:companyInfoProfile">
                        <errorMsg/>
                        <infoId>15961</infoId>
                        <successCode>00</successCode>
                        <rocBalanceSheetInfo/>
                        <rocBalanceSheetListInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <rocBalanceSheetInfos>
                              <rocBalanceSheetInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccType>N</accrualAccType>
                                 <auditFirmAddress1>12TH FLOOR, WISMA TUN SAMBANTHAN</auditFirmAddress1>
                                 <auditFirmAddress2>NO. 2, JALAN SULTAN SULAIMAN</auditFirmAddress2>
                                 <auditFirmAddress3/>
                                 <auditFirmName>FOLKS DFK &amp; CO</auditFirmName>
                                 <auditFirmNo>AF0502</auditFirmNo>
                                 <auditFirmPostcode>50000</auditFirmPostcode>
                                 <auditFirmState>W</auditFirmState>
                                 <auditFirmTown>KUALA LUMPUR</auditFirmTown>
                                 <auditfirmFlag/>
                                 <branchkeycode>0</branchkeycode>
                                 <companyNo>6386</companyNo>
                                 <contigentLiability>0.00</contigentLiability>
                                 <currentAsset>538731135.00</currentAsset>
                                 <dateOfTabling>2005-09-21T16:00:00.000Z</dateOfTabling>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2005-03-30T16:00:00.000Z</financialYearEndDate>
                                 <fixedAsset>134392783.00</fixedAsset>
                                 <fundAndReserve>0.00</fundAndReserve>
                                 <fundReserve>0.00</fundReserve>
                                 <headOfficeAccount>0.00</headOfficeAccount>
                                 <inappropriateProfit>75918000.00</inappropriateProfit>
                                 <liability>421559517.00</liability>
                                 <longTermLiability>89321468.00</longTermLiability>
                                 <minorityInterest>-22256822.00</minorityInterest>
                                 <nonCurrAsset>486421730.00</nonCurrAsset>
                                 <nonCurrentLiability>0.00</nonCurrentLiability>
                                 <otherAsset>254409111.00</otherAsset>
                                 <paidUpCapital>401422628.00</paidUpCapital>
                                 <reserves>45824323.00</reserves>
                                 <shareAppAccount>13363751.00</shareAppAccount>
                                 <sharePremium>45824323.00</sharePremium>
                                 <totalInvestment>97619836.00</totalInvestment>
                              </rocBalanceSheetInfos>
                        <rocBusinessAddressInfo>
                           <errorMsg/>
                           <infoId/>
                           <lastUpdateDate>2020-07-15T07:55:28.000Z</lastUpdateDate>
                           <successCode>00</successCode>
                           <address1>2.01, PJ TOWER</address1>
                           <address2>18 PERSIARAN BARAT</address2>
                           <address3/>
                           <companyNo>6386</companyNo>
                           <postcode>46050</postcode>
                           <state>B</state>
                           <town>PETALING JAYA</town>
                        </rocBusinessAddressInfo>
                        <rocBusinessCodeInfo/>
                        <rocBusinessCodeListInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <rocBusinessCodeInfos>
                              <rocBusinessCodeInfos>
                                 <businessCode>64200</businessCode>
                                 <companyNo>6386</companyNo>
                                 <priority>1</priority>
                              </rocBusinessCodeInfos>
                              <rocBusinessCodeInfos>
                                 <businessCode>64200</businessCode>
                                 <companyNo>6386</companyNo>
                                 <priority>1</priority>
                              </rocBusinessCodeInfos>
                              <rocBusinessCodeInfos>
                                 <businessCode>66191</businessCode>
                                 <companyNo>6386</companyNo>
                                 <priority>1</priority>
                              </rocBusinessCodeInfos>
                           </rocBusinessCodeInfos>
                        </rocBusinessCodeListInfo>
                        <rocChargesInfo/>
                        <rocChargesListInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <rocChargesInfos>
                              <rocChargesInfos>
                                 <ammendNo/>
                                 <chargeAmount>450000.00</chargeAmount>
                                 <chargeCreateDate>1968-07-15T16:30:00.000Z</chargeCreateDate>
                                 <chargeCreateDate1/>
                                 <chargeMortgageType>A</chargeMortgageType>
                                 <chargeNo>002</chargeNo>
                                 <chargeStatus>S</chargeStatus>
                                 <chargeeId>THE CHARTERED BANK</chargeeId>
                                 <chargeeName/>
                                 <companyNo>6386</companyNo>
                                 <form40Date>1968-08-14T16:30:00.000Z</form40Date>
                                 <totalOfCharge/>
                              </rocChargesInfos>
                           </rocChargesInfos>
                        </rocChargesListInfo>
                        <rocCompanyInfo>
                           <errorMsg/>
                           <infoId/>
                           <lastUpdateDate>2020-10-15T07:18:28.000Z</lastUpdateDate>
                           <successCode>00</successCode>
                           <balaceSheetInfo/>
                           <balaceSheetInfoDesc/>
                           <businessDescription>INVESTMENT HOLDING</businessDescription>
                           <checkDigit>K</checkDigit>
                           <companyCountry>MAL</companyCountry>
                           <companyName>AMCORP PROPERTIES BERHAD</companyName>
                           <companyNo>6386</companyNo>
                           <companyOldName>AMDB BERHAD</companyOldName>
                           <companyStatus>U</companyStatus>
                           <companyType>S</companyType>
                           <currency>RM</currency>
                           <dateOfChange>2010-09-07T16:00:00.000Z</dateOfChange>
                           <incomeStatInfo/>
                           <incomeStatInfoDesc/>
                           <incorpDate>1965-12-28T16:30:00.000Z</incorpDate>
                           <infoColon/>
                           <latestDocUpdateDate>2020-10-15T07:15:10.000Z</latestDocUpdateDate>
                           <llpInfo/>
                           <llpInfoDesc/>
                           <llpName/>
                           <llpNo/>
                           <localforeignCompany>L</localforeignCompany>
                           <naBal/>
                           <naProf/>
                           <statusOfCompany>E</statusOfCompany>
                           <wupType/>
                        </rocCompanyInfo>
                        <rocCompanyOfficerInfo/>
                        <rocCompanyOfficerListInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>2, JALAN TEBRAU 1</address1>
                                 <address2>UKAY HEIGHTS</address2>
                                 <address3>MALAYSIA</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1966-10-19T16:30:00.000Z</dob>
                                 <idNo>661020106186</idNo>
                                 <idType>MK</idType>
                                 <name>SHALINA BINTI AZMAN</name>
                                 <officerInfo/>
                                 <postcode>68000</postcode>
                                 <startDate>2007-07-29T16:00:00.000Z</startDate>
                                 <state>B</state>
                                 <town>AMPANG</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>A-07-03, SERAI BUKIT BANDARAYA,</address1>
                                 <address2>98 JALAN MEDANG SERAI,</address2>
                                 <address3>BUKIT BANDARAYA, BANGSAR</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1960-11-17T16:30:00.000Z</dob>
                                 <idNo>601118075627</idNo>
                                 <idType>MK</idType>
                                 <name>SOO KIM WAI</name>
                                 <officerInfo/>
                                 <postcode>59100</postcode>
                                 <startDate>2007-07-29T16:00:00.000Z</startDate>
                                 <state>W</state>
                                 <town>KUALA LUMPUR</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>8 CHANGKAT DATUK SULAIMAN 1</address1>
                                 <address2>TTDI HILLS</address2>
                                 <address3>TAMAN TUN DR ISMAIL</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>S</designationCode>
                                 <dob>1970-05-24T16:30:00.000Z</dob>
                                 <idNo>700525105671</idNo>
                                 <idType>MK</idType>
                                 <name>YAP CHOON SENG</name>
                                 <officerInfo/>
                                 <postcode>60000</postcode>
                                 <startDate>2007-09-06T16:00:00.000Z</startDate>
                                 <state>W</state>
                                 <town>KUALA LUMPUR</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>NO.3, JALAN SS19/3C</address1>
                                 <address2/>
                                 <address3/>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>S</designationCode>
                                 <dob>1958-08-25T16:30:00.000Z</dob>
                                 <idNo>580826055408</idNo>
                                 <idType>MK</idType>
                                 <name>CHUA SIEW CHUAN</name>
                                 <officerInfo/>
                                 <postcode>47500</postcode>
                                 <startDate>2008-04-10T16:00:00.000Z</startDate>
                                 <state>B</state>
                                 <town>SUBANG JAYA</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>06-06 CASA KIARA 2 CONDO</address1>
                                 <address2>14 JALAN KIARA 5</address2>
                                 <address3>BUKIT KIARA</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1955-05-06T16:30:00.000Z</dob>
                                 <idNo>550507075279</idNo>
                                 <idType>MK</idType>
                                 <name>P'NG SOO THENG</name>
                                 <officerInfo/>
                                 <postcode>50480</postcode>
                                 <startDate>2010-05-31T16:00:00.000Z</startDate>
                                 <state>W</state>
                                 <town>KUALA LUMPUR</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>35, PERSIARAN ZAABA</address1>
                                 <address2>TAMAN TUN DR ISMAIL</address2>
                                 <address3>MALAYSIA</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1950-07-15T16:30:00.000Z</dob>
                                 <idNo>500716055121</idNo>
                                 <idType>MK</idType>
                                 <name>TAN BUN POO</name>
                                 <officerInfo/>
                                 <postcode>60000</postcode>
                                 <startDate>2013-05-31T16:00:00.000Z</startDate>
                                 <state>W</state>
                                 <town>KUALA LUMPUR</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>85,PERSIARAN DEDAP</address1>
                                 <address2>BATIK SIERRAMAS</address2>
                                 <address3/>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1950-02-02T16:30:00.000Z</dob>
                                 <idNo>500203075573</idNo>
                                 <idType>MK</idType>
                                 <name>KAMIL AHMAD MERICAN</name>
                                 <officerInfo/>
                                 <postcode>47000</postcode>
                                 <startDate>2013-07-22T16:00:00.000Z</startDate>
                                 <state>B</state>
                                 <town>SUNGAI BULOH</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>NO. 12 JALAN AMAN PERDANA 7B/KU5</address1>
                                 <address2>TAMAN AMAN PERDANA</address2>
                                 <address3>MALAYSIA</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>M</designationCode>
                                 <dob>1961-09-07T16:30:00.000Z</dob>
                                 <idNo>610908085015</idNo>
                                 <idType>MK</idType>
                                 <name>LEE KEEN PONG</name>
                                 <officerInfo/>
                                 <postcode>41050</postcode>
                                 <startDate>2007-07-29T16:00:00.000Z</startDate>
                                 <state>B</state>
                                 <town>KLANG</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>2 JALAN TERBAU 1</address1>
                                 <address2>UKAY HEIGHTS</address2>
                                 <address3>MALAYSIA</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>M</designationCode>
                                 <dob>1974-09-23T16:30:00.000Z</dob>
                                 <idNo>740924145167</idNo>
                                 <idType>MK</idType>
                                 <name>SHAHMAN BIN AZMAN</name>
                                 <officerInfo/>
                                 <postcode>68000</postcode>
                                 <startDate>2012-02-20T16:00:00.000Z</startDate>
                                 <state>B</state>
                                 <town>AMPANG</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>71, JALAN SERI BERINGIN 2,</address1>
                                 <address2>SERI BERINGIN,</address2>
                                 <address3>BUKIT DAMANSARA,  MALAYSIA</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1964-11-25T16:30:00.000Z</dob>
                                 <idNo>641126107533</idNo>
                                 <idType>MK</idType>
                                 <name>LUM SING FAI</name>
                                 <officerInfo/>
                                 <postcode>50490</postcode>
                                 <startDate>2018-11-12T16:00:00.000Z</startDate>
                                 <state>W</state>
                                 <town>KUALA LUMPUR</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>47, JALAN MATAHARI,</address1>
                                 <address2>TAMAN WESTPOOL,</address2>
                                 <address3/>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1967-11-12T16:30:00.000Z</dob>
                                 <idNo>671113086435</idNo>
                                 <idType>MK</idType>
                                 <name>TAN EWE SEONG</name>
                                 <officerInfo/>
                                 <postcode>31400</postcode>
                                 <state>A</state>
                                 <town>IPOH</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>2.01 PJ TOWER</address1>
                                 <address2>AMCORP TRADE CENTRE</address2>
                                 <address3>18 JALAN PERSIARAN BARAT</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <idNo>6386</idNo>
                                 <idType>C</idType>
                                 <name>AMCORP PROPERTIES BERHAD SHARE BUY BACK ACCOUNT</name>
                                 <officerInfo/>
                                 <postcode>46050</postcode>
                                 <resignDate>2018-12-28T16:00:00.000Z</resignDate>
                                 <state>B</state>
                                 <town>PETALING JAYA</town>
                              </rocCompanyOfficerInfos>
                              <rocCompanyOfficerInfos>
                                 <address1>NO. 18 JALAN BU 3/5</address1>
                                 <address2>BANDAR UTAMA</address2>
                                 <address3>MALAYSIA</address3>
                                 <appointmentDate/>
                                 <companyNo>6386</companyNo>
                                 <designationCode>D</designationCode>
                                 <dob>1960-08-13T16:30:00.000Z</dob>
                                 <idNo>600814075191</idNo>
                                 <idType>MK</idType>
                                 <name>MAZLAN BIN MANSOR</name>
                                 <officerInfo/>
                                 <postcode>47800</postcode>
                                 <startDate>2020-09-30T16:00:00.000Z</startDate>
                                 <state>B</state>
                                 <town>PETALING JAYA</town>
                              </rocCompanyOfficerInfos>
                           </rocCompanyOfficerInfos>
                        </rocCompanyOfficerListInfo>
                        <rocDocumentLodgeInfo/>
                        <rocDocumentLodgeListInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2020-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2019-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2018-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2017-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2016-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2015-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2014-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2013-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2012-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2011-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2010-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2009-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2008-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2007-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2006-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                              <rocDocumentLodgeInfos>
                                 <companyNo/>
                                 <documentDate>2005-03-30T16:00:00.000Z</documentDate>
                                 <formTrx>557</formTrx>
                              </rocDocumentLodgeInfos>
                           </rocDocumentLodgeInfos>
                        </rocDocumentLodgeListInfo>
                        <rocProfitLossInfo/>
                        <rocProfitLossListInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2006-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>-109237888.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>-287639518.00</inappropriateProfitCf>
                                 <minorityInterest>-32717004.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>-145684626.00</profitAfterTax>
                                 <profitBeforeTax>-143429305.00</profitBeforeTax>
                                 <profitShareholder>-178401630.00</profitShareholder>
                                 <revenue>219612900.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2007-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>-287639518.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>-263383955.00</inappropriateProfitCf>
                                 <minorityInterest>-271821.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>24527384.00</profitAfterTax>
                                 <profitBeforeTax>19764265.00</profitBeforeTax>
                                 <profitShareholder>24255563.00</profitShareholder>
                                 <revenue>284892058.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2008-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>-263383955.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>-277840761.00</inappropriateProfitCf>
                                 <minorityInterest>3500576.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>-3787453.00</priorAdjustment>
                                 <profitAfterTax>-14169929.00</profitAfterTax>
                                 <profitBeforeTax>-5858038.00</profitBeforeTax>
                                 <profitShareholder>-10669353.00</profitShareholder>
                                 <revenue>425996524.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2010-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>-260162294.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>139583084.00</inappropriateProfitCf>
                                 <minorityInterest>-2260053.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>356549955.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>35919989.00</profitAfterTax>
                                 <profitBeforeTax>18876909.00</profitBeforeTax>
                                 <profitShareholder>33659936.00</profitShareholder>
                                 <revenue>240701487.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>9535487.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2012-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>187566000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>276567000.00</inappropriateProfitCf>
                                 <minorityInterest>-1692000.00</minorityInterest>
                                 <netDividend>-12894000.00</netDividend>
                                 <others>-81000.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>103668000.00</profitAfterTax>
                                 <profitBeforeTax>101061000.00</profitBeforeTax>
                                 <profitShareholder>101976000.00</profitShareholder>
                                 <revenue>256831000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2013-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>276567000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>360592000.00</inappropriateProfitCf>
                                 <minorityInterest>104000.00</minorityInterest>
                                 <netDividend>-13538000.00</netDividend>
                                 <others>-114000.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>96692000.00</profitAfterTax>
                                 <profitBeforeTax>95907000.00</profitBeforeTax>
                                 <profitShareholder>96796000.00</profitShareholder>
                                 <revenue>174048000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>881000.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2014-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>360592000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>519358000.00</inappropriateProfitCf>
                                 <minorityInterest>-571000.00</minorityInterest>
                                 <netDividend>-12987000.00</netDividend>
                                 <others>451000.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>171873000.00</profitAfterTax>
                                 <profitBeforeTax>153730000.00</profitBeforeTax>
                                 <profitShareholder>171302000.00</profitShareholder>
                                 <revenue>170194000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>N</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2015-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>519358000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>488953000.00</inappropriateProfitCf>
                                 <minorityInterest>-1197000.00</minorityInterest>
                                 <netDividend>-65905000.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>36697000.00</profitAfterTax>
                                 <profitBeforeTax>41198000.00</profitBeforeTax>
                                 <profitShareholder>35500000.00</profitShareholder>
                                 <revenue>173606000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>N</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2016-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>488953000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>551155000.00</inappropriateProfitCf>
                                 <minorityInterest>-2390000.00</minorityInterest>
                                 <netDividend>-22749000.00</netDividend>
                                 <others>496000.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>86845000.00</profitAfterTax>
                                 <profitBeforeTax>90984000.00</profitBeforeTax>
                                 <profitShareholder>84455000.00</profitShareholder>
                                 <revenue>168244000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount></accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType></financialReportType>
                                 <financialYearEndDate>2017-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>551155000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>529145000.00</inappropriateProfitCf>
                                 <minorityInterest>-2195000.00</minorityInterest>
                                 <netDividend>-40683000.00</netDividend>
                                 <others>476000.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>20392000.00</profitAfterTax>
                                 <profitBeforeTax>32467000.00</profitBeforeTax>
                                 <profitShareholder>18197000.00</profitShareholder>
                                 <revenue>188225000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>N</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2018-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>529145000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>648953000.00</inappropriateProfitCf>
                                 <minorityInterest>-2901000.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>-22512000.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>145221000.00</profitAfterTax>
                                 <profitBeforeTax>175255000.00</profitBeforeTax>
                                 <profitShareholder>142320000.00</profitShareholder>
                                 <revenue>134085000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount></accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType></financialReportType>
                                 <financialYearEndDate>2019-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>644901000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>645742000.00</inappropriateProfitCf>
                                 <minorityInterest>-3519000.00</minorityInterest>
                                 <netDividend>-42767000.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>47127000.00</profitAfterTax>
                                 <profitBeforeTax>32937000.00</profitBeforeTax>
                                 <profitShareholder>43608000.00</profitShareholder>
                                 <revenue>147126000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>N</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2005-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>-108781988.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>-109237888.00</inappropriateProfitCf>
                                 <minorityInterest>-5007251.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>4551351.00</profitAfterTax>
                                 <profitBeforeTax>6446334.00</profitBeforeTax>
                                 <profitShareholder>-455900.00</profitShareholder>
                                 <revenue>247744077.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2011-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>138885000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>187566000.00</inappropriateProfitCf>
                                 <minorityInterest>-2306000.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>50987000.00</profitAfterTax>
                                 <profitBeforeTax>52331000.00</profitBeforeTax>
                                 <profitShareholder>48681000.00</profitShareholder>
                                 <revenue>110111000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>Y</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2009-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>-277840761.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>-260162294.00</inappropriateProfitCf>
                                 <minorityInterest>-772318.00</minorityInterest>
                                 <netDividend>0.00</netDividend>
                                 <others>0.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>18450785.00</profitAfterTax>
                                 <profitBeforeTax>-7430593.00</profitBeforeTax>
                                 <profitShareholder>17678467.00</profitShareholder>
                                 <revenue>176494521.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                              <rocProfitLossInfos>
                                 <errorMsg/>
                                 <infoId/>
                                 <successCode/>
                                 <accrualAccount>N</accrualAccount>
                                 <companyNo>6386</companyNo>
                                 <extraOrdinaryItem>0.00</extraOrdinaryItem>
                                 <financialReportType>Y</financialReportType>
                                 <financialYearEndDate>2020-03-30T16:00:00.000Z</financialYearEndDate>
                                 <grossDividendRate>0.00</grossDividendRate>
                                 <inappropriateProfitBf>645742000.00</inappropriateProfitBf>
                                 <inappropriateProfitCf>611449000.00</inappropriateProfitCf>
                                 <minorityInterest>-1993000.00</minorityInterest>
                                 <netDividend>-36922000.00</netDividend>
                                 <others>154000.00</others>
                                 <priorAdjustment>0.00</priorAdjustment>
                                 <profitAfterTax>4468000.00</profitAfterTax>
                                 <profitBeforeTax>17965000.00</profitBeforeTax>
                                 <profitShareholder>2475000.00</profitShareholder>
                                 <revenue>179533000.00</revenue>
                                 <surplusAfterTax>0.00</surplusAfterTax>
                                 <surplusBeforeTax>0.00</surplusBeforeTax>
                                 <surplusDeficitAfterTax>0.00</surplusDeficitAfterTax>
                                 <surplusDeficitBeforeTax>0.00</surplusDeficitBeforeTax>
                                 <totalExpenditure>0.00</totalExpenditure>
                                 <totalIncome>0.00</totalIncome>
                                 <totalRevenue>0.00</totalRevenue>
                                 <transferred>0.00</transferred>
                                 <turnover>0.00</turnover>
                              </rocProfitLossInfos>
                           </rocProfitLossInfos>
                        </rocProfitLossListInfo>
                        <rocRegAddressInfo>
                           <errorMsg/>
                           <infoId/>
                           <lastUpdateDate>2009-11-16T11:46:04.000Z</lastUpdateDate>
                           <successCode>00</successCode>
                           <address1>LEVEL 7, MENARA MILENIUM</address1>
                           <address2>JALAN DAMANLELA</address2>
                           <address3>PUSAT BANDAR DAMANSARA, DAMANSARA HEIGHTS</address3>
                           <companyNo>6386</companyNo>
                           <postcode>50490</postcode>
                           <state>W</state>
                           <town>KUALA LUMPUR</town>
                        </rocRegAddressInfo>
                        <rocShareCapitalInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <authorisedCapital>600000000.0000</authorisedCapital>
                           <companyNo>6386</companyNo>
                           <currency>RM</currency>
                           <currenyNominal>NOMINAL (sen)</currenyNominal>
                           <ordAIssuedCash xsi:type="soapenc:long">0</ordAIssuedCash>
                           <ordAIssuedNominal>0.0000</ordAIssuedNominal>
                           <ordAIssuedNonCash xsi:type="soapenc:long">0</ordAIssuedNonCash>
                           <ordANominalValue>0.0000</ordANominalValue>
                           <ordANumberOfShares>0</ordANumberOfShares>
                           <ordAmountAValue>0.0000</ordAmountAValue>
                           <ordAmountBValue>0.0000</ordAmountBValue>
                           <ordAmountValue>450000000.0000</ordAmountValue>
                           <ordBIssuedCash xsi:type="soapenc:long">0</ordBIssuedCash>
                           <ordBIssuedNominal>0.0000</ordBIssuedNominal>
                           <ordBIssuedNonCash xsi:type="soapenc:long">0</ordBIssuedNonCash>
                           <ordBNominalValue>0.0000</ordBNominalValue>
                           <ordBNumberOfShares>0</ordBNumberOfShares>
                           <ordIssuedCash xsi:type="soapenc:long">80370883</ordIssuedCash>
                           <ordIssuedNominal>43.0000</ordIssuedNominal>
                           <ordIssuedNonCash xsi:type="soapenc:long">652763336</ordIssuedNonCash>
                           <ordNominalValue>50.0000</ordNominalValue>
                           <ordNumberOfShares>900000000</ordNumberOfShares>
                           <othAIssuedCash xsi:type="soapenc:long">0</othAIssuedCash>
                           <othAIssuedNonCash xsi:type="soapenc:long">0</othAIssuedNonCash>
                           <othAmountValue>0.0000</othAmountValue>
                           <othBIssuedCash xsi:type="soapenc:long">0</othBIssuedCash>
                           <othBIssuedNonCash xsi:type="soapenc:long">0</othBIssuedNonCash>
                           <othIssuedCash xsi:type="soapenc:long">0</othIssuedCash>
                           <othIssuedNominal>0.0000</othIssuedNominal>
                           <othIssuedNonCash xsi:type="soapenc:long">0</othIssuedNonCash>
                           <othNominalValue>0.0000</othNominalValue>
                           <othNumberOfShares>0</othNumberOfShares>
                           <prefAIssuedCash xsi:type="soapenc:long">0</prefAIssuedCash>
                           <prefAIssuedNominal>0.0000</prefAIssuedNominal>
                           <prefAIssuedNonCash xsi:type="soapenc:long">0</prefAIssuedNonCash>
                           <prefANominalValue>0.0000</prefANominalValue>
                           <prefANumberOfShares>0</prefANumberOfShares>
                           <prefAmountAValue>0.0000</prefAmountAValue>
                           <prefAmountBValue>0.0000</prefAmountBValue>
                           <prefAmountValue>150000000.0000</prefAmountValue>
                           <prefBIssuedCash xsi:type="soapenc:long">509350516</prefBIssuedCash>
                           <prefBIssuedNominal>70.0000</prefBIssuedNominal>
                           <prefBIssuedNonCash xsi:type="soapenc:long">0</prefBIssuedNonCash>
                           <prefBNominalValue>0.0000</prefBNominalValue>
                           <prefBNumberOfShares>0</prefBNumberOfShares>
                           <prefIssuedCash xsi:type="soapenc:long">0</prefIssuedCash>
                           <prefIssuedNominal>0.0000</prefIssuedNominal>
                           <prefIssuedNonCash xsi:type="soapenc:long">0</prefIssuedNonCash>
                           <prefNominalValue>50.0000</prefNominalValue>
                           <prefNumberOfShares xsi:type="soapenc:long">300000000</prefNumberOfShares>
                           <totalIssued>36106001003.6900</totalIssued>
                        </rocShareCapitalInfo>
                        <rocShareholderInfo/>
                        <rocShareholderListInfo>
                           <errorMsg/>
                           <infoId/>
                           <successCode>00</successCode>
                           <rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>1166-T</idNo>
                                 <idType>C</idType>
                                 <name>AMCORP GROUP BERHAD</name>
                                 <share>158140531.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <dob>1938-10-10T16:40:00.000Z</dob>
                                 <idNo>381011085268</idNo>
                                 <idType>MK</idType>
                                 <name>SOO NGIK GEE@SOO YEH JOO</name>
                                 <share>8757000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>708932-T</idNo>
                                 <idType>C</idType>
                                 <name>ROCKWILLS TRUSTEE BERHAD</name>
                                 <share>29001000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <dob>1935-12-08T16:40:00.000Z</dob>
                                 <idNo>351209085573</idNo>
                                 <idType>MK</idType>
                                 <name>RAJA KARIB SHAH BIN RAJA SHAHRUDIN,DATO'</name>
                                 <share>2347583.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>845247-D</idNo>
                                 <idType>C</idType>
                                 <name>BIOTIARA SDN. BHD.</name>
                                 <share>3000000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>857890-H</idNo>
                                 <idType>C</idType>
                                 <name>MUTIARA ARCA SDN. BHD.</name>
                                 <share>13835284.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>-</idNo>
                                 <idType>XRS</idType>
                                 <name>REMAINING SHAREHOLDERS FOR BERHAD COMPANY</name>
                                 <share>622154475.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <dob>1940-07-10T16:40:00.000Z</dob>
                                 <idNo>400711105232</idNo>
                                 <idType>MK</idType>
                                 <name>ZAINAB BINTI S.YUSOFF BUX</name>
                                 <share>4532700.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <dob>1967-11-12T16:30:00.000Z</dob>
                                 <idNo>671113086435</idNo>
                                 <idType>MK</idType>
                                 <name>TAN EWE SEONG</name>
                                 <share>2800000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <dob>1941-08-29T16:40:00.000Z</dob>
                                 <idNo>410830085069</idNo>
                                 <idType>MK</idType>
                                 <name>TAN BENG GUAN</name>
                                 <share>4100000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>3077-T</idNo>
                                 <idType>C</idType>
                                 <name>NEOH CHOO EE &amp; COMPANY, SDN. BERHAD</name>
                                 <share>5000000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <dob>1956-04-01T16:30:00.000Z</dob>
                                 <idNo>560402075124</idNo>
                                 <idType>MK</idType>
                                 <name>YEOH GUAN LIEW</name>
                                 <share>2027100.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <dob>1980-09-28T16:30:00.000Z</dob>
                                 <idNo>800929146697</idNo>
                                 <idType>MK</idType>
                                 <name>ADAM SHAH BIN AZLAN</name>
                                 <share>7125100.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>274740-T</idNo>
                                 <idType>C</idType>
                                 <name>CIMB GROUP NOMINEES (TEMPATAN) SDN. BHD. PLEDGED SECURITIES ACCOUNT FOR AMCORP GROUP BERHAD (AGB CBC</name>
                                 <share>122500000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>122372-P</idNo>
                                 <idType>C</idType>
                                 <name>AL WAKALAH NOMINEES (TEMPATAN) SDN BHD PLEDGED SECURITIES ACCOUNT FOR AMCORP GROUP BERHAD</name>
                                 <share>84000000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>31121-M</idNo>
                                 <idType>C</idType>
                                 <name>BBL NOMINEES (TEMPATAN) SDN. BHD. PLEDGED SECURITIES ACCOUNT FOR AMCORP GROUP BERHAD</name>
                                 <share>55000000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>274740-T</idNo>
                                 <idType>C</idType>
                                 <name>CIMB GROUP NOMINEES (TEMPATAN) SDN. BHD. PLEDGED SECURITIES ACCOUNT FOR AMCORP GROUP BERHAD</name>
                                 <share>35000000.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>42234-H</idNo>
                                 <idType>C</idType>
                                 <name>ALLIANCEGROUP NOMINEES (TEMPATAN) SDN BHD PLEDGED SECURITIES ACCOUNT FOR AMCORP GROUP BERHAD</name>
                                 <share>40985600.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>262422-A</idNo>
                                 <idType>C</idType>
                                 <name>UOB KAY HIAN NOMINEES (ASING) SDN BHD EXEMPT AN FOR UOB KAY HIAN PTE LTD (A/C CLIENTS)</name>
                                 <share>3789837.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>265422-M</idNo>
                                 <idType>C</idType>
                                 <name>CIMSEC NOMINEES (ASING ) SDN BHD (EXEMPT AN FOR CGS-CIMB SECURITIES (SINGAPORE) PTE LTD)</name>
                                 <share>1693525.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                              <rocShareholderInfos>
                                 <companyNo>6386</companyNo>
                                 <idNo>6386-K</idNo>
                                 <idType>C</idType>
                                 <name>AMCORP PROPERTIES BERHAD SHARE BUY BACK ACCOUNT</name>
                                 <share>18346500.00</share>
                                 <shareVol/>
                              </rocShareholderInfos>
                           </rocShareholderInfos>
                        </rocShareholderListInfo>
                     </getInfoProfileReturn>
                  </response>
               </inf:getInfoProfileResponse>
            </soapenv:Body>
         </soapenv:Envelope>
    ```
