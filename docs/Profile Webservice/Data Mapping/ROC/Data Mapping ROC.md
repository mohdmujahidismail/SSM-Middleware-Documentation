# Data Mapping ROC

## **COMPANY PROFILE**

## Company information (ENG)
MAKLUMAT SYARIKAT(Malay)
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>Webservice</th>
			<th>json Node / Parameter</th>
			<th>Object Name</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Company Name</td>
			<td>Nama Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyName</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Last Old Name</td>
			<td>Nama Syarikat Lama</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyOldName</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Date of Change</td>
			<td>Tarikh Pertukaran</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>dateOfChange</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration No.</td>
			<td>No. Pendaftaran</td>
			<td>&nbsp;</td>
			<td>201101006232(934369-T)</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>12 digit new ?</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>201101006232</td>
			<td>GetNewFormatEntityNo</td>
			<td>NewFormatNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Company Number</td>
			<td>No Syarikat</td>
			<td>&nbsp;</td>
			<td>should show e.g :84984-H</td>
			<td>GetCompProfile</td>
			<td>companyNo-checkDigit</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Check Digit</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>T</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Incorporation Date</td>
			<td>Tarikh Penubuhan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>incorpDate</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration Date</td>
			<td>Tarikh Pendaftaran</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>registrationDate</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Jenis</td>
			<td><b>English</b>
				<br> B - LIMITED BY SHARE AND GUARANTEE,
				<br> G - LIMITED BY GUARANTEE
				<br> S - LIMITED BY SHARES
				<br> U - UNLIMITED
				<br> <b>Malay</b>
				<br> B - BERHAD MENURUT SAHAM DAN JAMINAN,
				<br> G - BERHAD MENURUT JAMINAN
				<br> S - BERHAD MENURUT SYER
				<br> U - TIDAK TERHAD</td>
			<td>Base from pdf template : column type is combination of<br><b>Type</b><br>:companyType<br> :companyStatus</td>
			<td>GetCompProfile</td>
			<td>companyType</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Jenis</td>
			<td>R-Private Limited (eng);Syarikat Persendirian(Malay)
				<br> U-Public Limited(eng);Syarikat Awam(Malay)</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyStatus</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Status</td>
			<td>Status</td>
			<td>B - DISSOLVED CONVERSION TO LLP
				<br> C - CEASED BUSINESS
				<br> D - DISSOLVED
				<br> E - EXISTING
				<br> R - REMOVED
				<br> W - WINDING UP
				<br> X - NULL AND VOID BY COURT ORDER
				<br> Y - STRUCK-OFF & WINDING-UP VIA COURT ORDER</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>statusOfCompany</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>LLP NAME</td>
			<td>NAMA PLT</td>
			<td>&nbsp;</td>
			<td>* need to view if status is Dissolved- Conversion to LLP</td>
			<td>GetCompProfile</td>
			<td>llpName</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>LLP NUMBER</td>
			<td>NOMBOR PLT</td>
			<td>&nbsp;</td>
			<td>* need to view if status is Dissolved- Conversion to LLP</td>
			<td>GetCompProfile</td>
			<td>llpNo</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>CONVERSION DATE</td>
			<td>TARIKH PERTUKARAN</td>
			<td>&nbsp;</td>
			<td>* need to view if status is Dissolved- Conversion to LLP</td>
			<td>GetCompProfile</td>
			<td>llpconvertDate</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Registered Address</td>
			<td>Alamat daftar</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>address1</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address2</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address3</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>town</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>state</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Postcode</td>
			<td>Poskod</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>postcode</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Origin</td>
			<td>Tempat Penubuhan</td>
			<td>MAL- Malaysia</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyCountry</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Business Address</td>
			<td>Alamat Perniagaan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>address1</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address2</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address3</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>town</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>state</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Postcode</td>
			<td>Poskod</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>postcode</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Nature of Business</td>
			<td>Jenis Perniagaan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>businessDescription</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
	</tbody>
</table>

## Summary of Share Capital(ENG)
Maklumat Modal(MALAY)
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>&nbsp;</th>
			<th>json Node</th>
			<th>Object Name</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Column Name(English)</td>
			<td>Column Name(MALAY)</td>
			<td>Sample Data</td>
			<td>Remarks</td>
			<td>&nbsp;</td>
			<td>json Node</td>
			<td>Object Name</td>
			<td>Sdn Bhd</td>
			<td>CLBG</td>
			<td>Foreign</td>
		</tr>
		<tr>
			<td>Company Name</td>
			<td>Nama Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyName</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration No.</td>
			<td>No. Pendaftaran</td>
			<td>&nbsp;</td>
			<td>201101006232<br>(934369-T)</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>12-digit new</td>
			<td>12-digit baru</td>
			<td>&nbsp;</td>
			<td>201101006232</td>
			<td>GetNewFormatEntityNo</td>
			<td>NewEntityNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Company Number</td>
			<td>No. Syarikat</td>
			<td>&nbsp;</td>
			<td>934369</td>
			<td>GetCompProfile</td>
			<td>companyNo</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Check Digit</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>T</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Currency</td>
			<td>&nbsp;</td>
			<td>Handle on currency type if foreign company(RM,SGD,USD etc</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>currency</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>TOTAL AUTHORIZED </td>
			<td>JUMLAH DIBENARKAN</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>authorisedCapital</td>
			<td>rocCompanyInfo</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>ORDINARY/AMT</td>
			<td>BIASA/JUMLAH</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>(ordNumberOfShares*ordNominalValue)/100; OR OrdAmountvalue</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>ORDINARY/DIVIDED INTO</td>
			<td>BIASA/BAHAGI KEPADA</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>ordNumberOfShares</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>ORDINARY/NOMINAL VALUE</td>
			<td>BIASA/AMAUN NOMINAL (sen)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>ordNominalValue</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>PREFERENCE/AMT</td>
			<td>PREFEREN/JUMLAH</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>(prefNumberOfShares*prefNominalValue)/100;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>PREFERENCE/DIVIDED INTO</td>
			<td>PREFEREN/BAHAGI KEPADA</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>prefNumberOfShares</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>PREFERENCE/NOMINAL VALUE</td>
			<td>PREFEREN/AMAUN NOMINAL (sen)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>prefNominalValue</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>OTHERS/AMT</td>
			<td>LAIN-LAIN/JUMLAH</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>(othNumberOfShares*othNominalValue)/100</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>OTHERS/DIVIDED INTO</td>
			<td>LAIN-LAIN/BAHAGI KEPADA</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>othNumberOfShares</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>OTHERS/NOMINAL VALUE</td>
			<td>LAIN-LAIN/AMAUN NOMINAL(sen)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>othNominalValue</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>TOTAL ISSUED(RM)</td>
			<td>JUMLAH DITERBITKAN(RM)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display 0 if don`t have any value</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>ORDINARY/CASH</td>
			<td>BIASA/TUNAI</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>ordIssuedCash</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display 0 if don`t have any value</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>ORDINARY/OTHERWISE THAN CASH</td>
			<td>BIASA/SELAIN DARI TUNAI</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>ordIssuedNonCash</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display 0 if don`t have any value</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>ORDINARY/NOMINAL VALUE</td>
			<td>BIASA/AMAUN NOMINAL (sen)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>ordNominalValue</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>PREFERENCE/CASH</td>
			<td>PREFEREN/TUNAI</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>prefIssuedCash</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display 0 if don`t have any value</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>PREFERENCE/OTHERWISE THAN CASH</td>
			<td>PREFEREN/SELAIN DARI TUNAI</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>prefIssuedNonCash</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display 0 if don`t have any value</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>PEREFERENCE/NOMINAL VALUE</td>
			<td>PREFEREN/AMAUN NOMINAL (sen)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>prefIssuedNominal</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>OTHERS/CASH</td>
			<td>LAIN-LAIN/TUNAI</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>othIssuedCash</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes, but will display 0 if don`t have any value</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>OTHER/OTHERWISE THAN CASH</td>
			<td>LAIN-LAIN/SELAIN DARI TUNAI</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>othIssuedNonCash</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes, but will display 0 if don`t have any value</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>OTHER/NOMINAL VALUE</td>
			<td>LAIN-LAIN/AMAUN NOMINAL(sen)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>othNominalValue</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td></td>
		</tr>
	</tbody>
</table>

## Directors/Officers(ENG)
MAKLUMAT PENGARAH DAN PEGAWAI(Malay)
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>Webservice</th>
			<th>json Node</th>
			<th>Object Name</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Company Name</td>
			<td>Nama Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyName</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration No.</td>
			<td>No. Pendaftaran</td>
			<td>&nbsp;</td>
			<td>201101006232(934369-T)</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>12-digit new</td>
			<td>12-digit baru</td>
			<td>&nbsp;</td>
			<td>201101006232</td>
			<td>GetNewFormatEntityNo</td>
			<td>NewEntityNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Company Number</td>
			<td>No. Syarikat</td>
			<td>&nbsp;</td>
			<td>934369</td>
			<td>GetCompProfile</td>
			<td>companyNo</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Check Digit</td>
			<td>Angka Uji</td>
			<td>&nbsp;</td>
			<td>T</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Name</td>
			<td>Nama </td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>name</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Address</td>
			<td>Alamat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>address1</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>address2</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>address3</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>postcode</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>town</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>state</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>IC/PASSPORT</td>
			<td>KP/Paspot</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>idNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Designation</td>
			<td>Jawatan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>designationCode</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Date of Appointment</td>
			<td>Tarikh Lantikan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>startDate</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
	</tbody>
</table>

## Shareholder/Members(ENG)
MAKLUMAT PEMEGANG SYER(Malay)
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>&nbsp;</th>
			<th>json Node</th>
			<th>&nbsp;</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Company Name</td>
			<td>Nama Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>companyName</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration No.</td>
			<td>No. Pendaftaran</td>
			<td>&nbsp;</td>
			<td>201101006232<br>(934369-T)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>12-digit new ?</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>201101006232</td>
			<td>GetNewFormatEntityNo</td>
			<td>NewEntityNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Company Number</td>
			<td>No. Syarikat</td>
			<td>&nbsp;</td>
			<td>934369</td>
			<td>&nbsp;</td>
			<td>companyNo</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Check Digit</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>T</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>IC/PASSPORT/COMPANY NO</td>
			<td>KP/Paspot/No Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>idNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
		<tr>
			<td>NAME/COMPANY NAME</td>
			<td>Nama/Nama Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>name</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
		<tr>
			<td>total of share</td>
			<td>Jumlah Syer</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>share</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
	</tbody>
</table>

## Company Charges(ENG)
MAKLUMAT GADAIAN(Malay)
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>&nbsp;</th>
			<th>json Node</th>
			<th>&nbsp;</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Company Name</td>
			<td>Nama Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>companyName</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration No.</td>
			<td>No. Pendaftaran</td>
			<td>&nbsp;</td>
			<td>201101006232<br>(934369-T)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>12-digit new ?</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>201101006232</td>
			<td>GetNewFormatEntityNo</td>
			<td>NewEntityNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Company Number</td>
			<td>No. Syarikat</td>
			<td>&nbsp;</td>
			<td>934369</td>
			<td>&nbsp;</td>
			<td>companyNo</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Check Digit</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>T</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Charge Number</td>
			<td>No Gadaian</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>chargeNo</td>
			<td>&nbsp;</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
		<tr>
			<td>Total of charge</td>
			<td>Jumlah Gadaian</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>chargeAmount</td>
			<td>&nbsp;</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
		<tr>
			<td>Date of Creation</td>
			<td>Tarikh Wujud</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>chargeCreateDate</td>
			<td>&nbsp;</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
		<tr>
			<td>Name of Chargee</td>
			<td>Pemegang Gadaian</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>chargeeName</td>
			<td>&nbsp;</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
		<tr>
			<td>Charge Status</td>
			<td>Status Gadaian</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>chargeStatus</td>
			<td>&nbsp;</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
			<td>Yes, but will display "No Information" if don`t have any value</td>
		</tr>
	</tbody>
</table>

## Summary of Financial Information(ENG)
RINGKASAN PENYATA KEWANGAN(Malay)
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>&nbsp;</th>
			<th>json Node</th>
			<th>&nbsp;</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Company Name</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>companyName</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration No.</td>
			<td>No. Pendaftaran</td>
			<td>&nbsp;</td>
			<td>201101006232(934369-T)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>12-digit new ?</td>
			<td>12-digit new ?</td>
			<td>&nbsp;</td>
			<td>201101006232</td>
			<td>GetNewFormatEntityNo</td>
			<td>NewEntityNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Company Number</td>
			<td>No. Syarikat</td>
			<td>&nbsp;</td>
			<td>934369</td>
			<td>&nbsp;</td>
			<td>companyNo</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Check Digit</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>T</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Auditor</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>auditFirmName</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Auditor Address</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>auditFirmAddress1</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>auditFirmAddress2</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>auditFirmAddress3</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>auditFirmPostcode</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>auditFirmTown</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>auditFirmState</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Exempt Private Company</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>To be determine. Currently just put N/A</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Financial Year End</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>financialYearEndDate</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Unqualified reports</td>
			<td>&nbsp;</td>
			<td>Y-unqualified,N-Qualified</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>financialReportType</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Consolidated accounts</td>
			<td>&nbsp;</td>
			<td>N-not consolidated,Y-Consolidated</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>accrualAccount</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Date of Tabling</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>dateOfTabling</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
	</tbody>
</table>

### Summary of Financial Information(BALANCE SHEET ITEMS)

<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>XML node</th>
			<th>json Node;</th>
			<th>&nbsp;</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Non-current assets</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>NonCurrentAsset</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Current Assets</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>currentAsset</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Non-current liabilities</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>nonCurrentLiability</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Current liabilities</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>liability</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Share Capital</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company</td>
			<td>&nbsp;</td>
			<td>paidUpCapital</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Reserve</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company</td>
			<td>&nbsp;</td>
			<td>Reserve</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Retain Earning</td>
			<td>* Tiada parameter</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>InappropriateProfit</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Minority Interest</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company</td>
			<td>&nbsp;</td>
			<td>minorityInterest</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Fund and Reserve</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for CLBG company</td>
			<td>&nbsp;</td>
			<td>fundAndReserve</td>
			<td>&nbsp;</td>
			<td>No</td>
			<td>Yes</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Head office Account</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for foreign company</td>
			<td>&nbsp;</td>
			<td>headOfficeAccount</td>
			<td>&nbsp;</td>
			<td>No</td>
			<td>No</td>
			<td>Yes</td>
		</tr>
	</tbody>
</table>

### Summary of Financial Information(INCOME STATEMENT ITEMS)
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Column Name(English)</th>
			<th>Column Name(MALAY)</th>
			<th>Sample Data</th>
			<th>Remarks</th>
			<th>&nbsp;</th>
			<th>json Node;</th>
			<th>&nbsp;</th>
			<th>Sdn Bhd</th>
			<th>CLBG</th>
			<th>Foreign</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Total Income</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>totalIncome</td>
			<td>&nbsp;</td>
			<td>No</td>
			<td>Yes</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Total Expenditure</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>TotalRevenue</td>
			<td>&nbsp;</td>
			<td>No</td>
			<td>Yes</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Revenue</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company & foreign company</td>
			<td>&nbsp;</td>
			<td>revenue</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Profit/(loss) before tax</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company & foreign company</td>
			<td>&nbsp;</td>
			<td>profitBeforeTax</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Profit/(loss) after tax</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company & foreign company</td>
			<td>&nbsp;</td>
			<td>profitAfterTax</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Net dividen</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company</td>
			<td>&nbsp;</td>
			<td>netDividend</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Minority Interest</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for local company</td>
			<td>&nbsp;</td>
			<td>minorityInterest</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Surplus/(Deficit) before tax</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for CLBG company</td>
			<td>&nbsp;</td>
			<td>surplusBeforeTax</td>
			<td>&nbsp;</td>
			<td>No</td>
			<td>Yes</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Surplus/(Deficit) after tax</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for CLBG company</td>
			<td>&nbsp;</td>
			<td>surplusAfterTax</td>
			<td>&nbsp;</td>
			<td>No</td>
			<td>Yes</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Unappropriated Profit B/Forward</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>*view for CLBG company </td>
			<td>&nbsp;</td>
			<td>inappropriateProfitBf</td>
			<td>&nbsp;</td>
			<td>No</td>
			<td>Yes</td>
			<td>No</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td></td>
		</tr>
	</tbody>
</table>

<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>Stamp</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>For document with ctc</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>CTC QR Code</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>User ID</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Printing Date with Time (Center)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Printing Date (Right Side)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Printing Date with Time (Bottom)</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td></td>
		</tr>
	</tbody>
</table>


<!-- <iframe width="880" height="664" frameborder="0" scrolling="no" src="https://ssmmy.sharepoint.com/sites/UnitPembekalanData/_layouts/15/Doc.aspx?sourcedoc={0d607c4b-c44c-403b-a205-32b6a21ad5b5}&action=embedview&wdAllowInteractivity=False&wdHideGridlines=True&wdHideHeaders=True&wdDownloadButton=True&wdInConfigurator=True"></iframe> -->