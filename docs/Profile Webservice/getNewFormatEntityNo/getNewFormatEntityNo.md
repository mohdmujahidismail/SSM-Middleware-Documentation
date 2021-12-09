# getNewFormatEntityNo

## New Format Entity Number Request Respond, Data Mapping, and Issues

## How to write message request
Mandatory field must be filled as explained below: 
~~~~~~ xml
<customerId>your agent code</customerId>
~~~~~~
Please put your agent code. 

~~~~~~ xml
<customerReferenceNo>MBDDTest</customerReferenceNo>
~~~~~~

## Good Message Request and Respond

=== "Good Message Request"
	```xml
	<soapenv:Envelope
		xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
		xmlns:ws="http://integrasi.ssm.com.my/InfoService/1/WS">
		<soapenv:Header/>
		<soapenv:Body>
			<ws:getNewFormatEntityNo>
				<!--Optional:-->
				<header>
					<!--Optional:-->
					<customerId>MBDD</customerId>
					<!--Optional:-->
					<customerReferenceNo>MBDDTest</customerReferenceNo>
					<!--Optional:-->
					<customerRequestDate></customerRequestDate>
				</header>
				<!--Optional:-->
				<request>
					<!--Optional:-->
					<newFormatEntityNoReq>
						<!--Optional:-->
						<agencyId></agencyId>
						<!--Optional:-->
						<checkDigit>X</checkDigit>
						<!--Optional:-->
						<formatType>OLD</formatType>
						<!--Optional:-->
						<regNo>158665</regNo>
						<!--Optional:-->
						<tableId></tableId>
						<!--Optional:-->
						<type>ROC</type>
					</newFormatEntityNoReq>
				</request>
			</ws:getNewFormatEntityNo>
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
			<inf:getNewFormatEntityNoResponse
				xmlns:inf="http://integrasi.ssm.com.my/InfoService/1/WS"
				xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/">
				<header>
					<customerId>MBDD</customerId>
					<customerReferenceNo>MBDDTest</customerReferenceNo>
					<customerRequestDate/>
					<errorCode/>
					<errorMessage/>
					<hostErrorCode/>
					<hostErrorMessage/>
					<requestTimestamp>2021-11-24T16:18:27.931</requestTimestamp>
					<responseTimestamp>2021-11-24T16:18:27.966</responseTimestamp>
				</header>
				<request>
					<newFormatEntityNoReq>
						<agencyId/>
						<checkDigit>X</checkDigit>
						<formatType>OLD</formatType>
						<regNo>158665</regNo>
						<tableId/>
						<type>ROC</type>
					</newFormatEntityNoReq>
				</request>
				<response>
					<getNewFormatEntityNoReturn>
						<errorMsg/>
						<newFormatNo>198601001038</newFormatNo>
						<oldFormatNo>158665-X</oldFormatNo>
						<successCode>00</successCode>
					</getNewFormatEntityNoReturn>
				</response>
			</inf:getNewFormatEntityNoResponse>
		</soapenv:Body>
	</soapenv:Envelope>
	```