# Entrega da ponderada do grupo 1 
por: Edu HOS


# Diagrama Entidade-Relacionamento

Abaixo está o diagrama entidade-relacionamento que contempla as principais entidades relacionadas aos dados mestres identificados no projeto.

![Mapa de Entidade-Relacionamento](https://res.cloudinary.com/dmornatkl/image/upload/v1726252576/Captura_de_tela_2024-09-12_173011_ytrxoc.png)

[Link para o arquivo](https://drive.google.com/file/d/1oAj_M9-C-gA04soC9Lj0CfuCL5wn6nyW/view?usp=sharing)

```markdown

<?xml version="1.0" encoding="utf-8" ?>
<!-- SQL XML created by WWW SQL Designer, https://github.com/ondras/wwwsqldesigner/ -->
<!-- Active URL: https://sql.toad.cz/ -->
<sql>
<datatypes db="mysql">
	<group label="Numeric" color="rgb(238,238,170)">
		<type label="Integer" length="0" sql="INTEGER" quote=""/>
	 	<type label="TINYINT" length="0" sql="TINYINT" quote=""/>
	 	<type label="SMALLINT" length="0" sql="SMALLINT" quote=""/>
	 	<type label="MEDIUMINT" length="0" sql="MEDIUMINT" quote=""/>
	 	<type label="INT" length="0" sql="INT" quote=""/>
		<type label="BIGINT" length="0" sql="BIGINT" quote=""/>
		<type label="Decimal" length="1" sql="DECIMAL" re="DEC" quote=""/>
		<type label="Single precision" length="0" sql="FLOAT" quote=""/>
		<type label="Double precision" length="0" sql="DOUBLE" re="DOUBLE" quote=""/>
	</group>
	<group label="Character" color="rgb(255,200,200)">
		<type label="Char" length="1" sql="CHAR" quote="'"/>
		<type label="Varchar" length="1" sql="VARCHAR" quote="'"/>
		<type label="Text" length="0" sql="MEDIUMTEXT" re="TEXT" quote="'"/>
		<type label="Binary" length="1" sql="BINARY" quote="'"/>
		<type label="Varbinary" length="1" sql="VARBINARY" quote="'"/>
		<type label="BLOB" length="0" sql="BLOB" re="BLOB" quote="'"/>
	</group>
	<group label="Date &amp; Time" color="rgb(200,255,200)">
		<type label="Date" length="0" sql="DATE" quote="'"/>
		<type label="Time" length="0" sql="TIME" quote="'"/>
		<type label="Datetime" length="0" sql="DATETIME" quote="'"/>
		<type label="Year" length="0" sql="YEAR" quote=""/>
		<type label="Timestamp" length="0" sql="TIMESTAMP" quote="'"/>
	</group>
	
	<group label="Miscellaneous" color="rgb(200,200,255)">
		<type label="ENUM" length="1" sql="ENUM" quote=""/>
		<type label="SET" length="1" sql="SET" quote=""/>
		<type label="Bit" length="0" sql="bit" quote=""/>
	</group>
</datatypes><table x="455" y="161" name="OCRD">
<row name="CardCode" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="CardName" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="CardForeignName" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="CardType" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="GroupCode" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="Phone1" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="Phone2" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="Cellular" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="Fax" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="EmailAddress" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="ShippingType" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="WebSite" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="CompanyPrivate" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<key type="PRIMARY" name="">
<part>CardCode</part>
</key>
</table>
<table x="195" y="138" name="CRD1">
<row name="id" null="1" autoincrement="1">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="CardCode" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default><relation table="OCRD" row="CardCode" />
</row>
<row name="AdresType" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="Address" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="AddrType" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="Street" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="StreetNo" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="Block" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="City" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="County" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="State" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="ZipCode" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="Country" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="Building" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<key type="PRIMARY" name="">
<part>id</part>
</key>
</table>
<table x="802" y="301" name="CRD7">
<row name="id" null="1" autoincrement="1">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="CardCode" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default><relation table="OCRD" row="CardCode" />
</row>
<row name="LineNum" null="1" autoincrement="0">
<datatype>BINARY</datatype>
<default>NULL</default></row>
<row name="Address" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="CNAECode" null="1" autoincrement="0">
<datatype>INTEGER</datatype>
<default>NULL</default></row>
<row name="TaxId0" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId1" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId2" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId3" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId4" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId5" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId6" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId7" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="TaxId8" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<key type="PRIMARY" name="">
<part>id</part>
</key>
</table>
<table x="801" y="8" name="OCRB">
<row name="id" null="1" autoincrement="1">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="Cardcode" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default><relation table="OCRD" row="CardCode" />
</row>
<row name="LineNum" null="1" autoincrement="0">
<datatype>BINARY</datatype>
<default>NULL</default></row>
<row name="County" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="BankCode" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="Branch" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="UserNo1" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="AccountNo" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="UserNo2" null="1" autoincrement="0">
<datatype>VARCHAR</datatype>
<default>NULL</default></row>
<row name="AccountName" null="1" autoincrement="0">
<datatype>MEDIUMTEXT</datatype>
<default>NULL</default></row>
<key type="PRIMARY" name="">
<part>id</part>
</key>
</table>
</sql>
```

---

## SQL Gerado

```sql
-- ---
-- Table 'OCRD'
-- ---
DROP TABLE IF EXISTS `OCRD`;

CREATE TABLE `OCRD` (
  `CardCode` VARCHAR NULL DEFAULT NULL,
  `CardName` VARCHAR NULL DEFAULT NULL,
  `CardForeignName` VARCHAR NULL DEFAULT NULL,
  `CardType` VARCHAR NULL DEFAULT NULL,
  `GroupCode` INTEGER NULL DEFAULT NULL,
  `Phone1` INTEGER NULL DEFAULT NULL,
  `Phone2` INTEGER NULL DEFAULT NULL,
  `Cellular` INTEGER NULL DEFAULT NULL,
  `Fax` INTEGER NULL DEFAULT NULL,
  `EmailAddress` VARCHAR NULL DEFAULT NULL,
  `ShippingType` VARCHAR NULL DEFAULT NULL,
  `WebSite` VARCHAR NULL DEFAULT NULL,
  `CompanyPrivate` VARCHAR NULL DEFAULT NULL,
  PRIMARY KEY (`CardCode`)
);

-- ---
-- Table 'CRD1'
-- ---
DROP TABLE IF EXISTS `CRD1`;

CREATE TABLE `CRD1` (
  `id` VARCHAR NULL AUTO_INCREMENT DEFAULT NULL,
  `CardCode` VARCHAR NULL DEFAULT NULL,
  `AdresType` VARCHAR NULL DEFAULT NULL,
  `Address` VARCHAR NULL DEFAULT NULL,
  `AddrType` VARCHAR NULL DEFAULT NULL,
  `Street` VARCHAR NULL DEFAULT NULL,
  `StreetNo` INTEGER NULL DEFAULT NULL,
  `Block` VARCHAR NULL DEFAULT NULL,
  `City` VARCHAR NULL DEFAULT NULL,
  `County` INTEGER NULL DEFAULT NULL,
  `State` VARCHAR NULL DEFAULT NULL,
  `ZipCode` INTEGER NULL DEFAULT NULL,
  `Country` VARCHAR NULL DEFAULT NULL,
  `Building` VARCHAR NULL DEFAULT NULL,
  PRIMARY KEY (`id`)
);

-- ---
-- Table 'CRD7'
-- ---
DROP TABLE IF EXISTS `CRD7`;

CREATE TABLE `CRD7` (
  `id` VARCHAR NULL AUTO_INCREMENT DEFAULT NULL,
  `CardCode` VARCHAR NULL DEFAULT NULL,
  `LineNum` BINARY NULL DEFAULT NULL,
  `Address` VARCHAR NULL DEFAULT NULL,
  `CNAECode` INTEGER NULL DEFAULT NULL,
  `TaxId0` VARCHAR NULL DEFAULT NULL,
  `TaxId1` VARCHAR NULL DEFAULT NULL,
  `TaxId2` VARCHAR NULL DEFAULT NULL,
  `TaxId3` VARCHAR NULL DEFAULT NULL,
  `TaxId4` VARCHAR NULL DEFAULT NULL,
  `TaxId5` VARCHAR NULL DEFAULT NULL,
  `TaxId6` VARCHAR NULL DEFAULT NULL,
  `TaxId7` VARCHAR NULL DEFAULT NULL,
  `TaxId8` VARCHAR NULL DEFAULT NULL,
  PRIMARY KEY (`id`)
);

-- ---
-- Table 'OCRB'
-- ---
DROP TABLE IF EXISTS `OCRB`;

CREATE TABLE `OCRB` (
  `id` VARCHAR NULL AUTO_INCREMENT DEFAULT NULL,
  `Cardcode` VARCHAR NULL DEFAULT NULL,
  `LineNum` BINARY NULL DEFAULT NULL,
  `County` VARCHAR NULL DEFAULT NULL,
  `BankCode` VARCHAR NULL DEFAULT NULL,
  `Branch` VARCHAR NULL DEFAULT NULL,
  `UserNo1` VARCHAR NULL DEFAULT NULL,
  `AccountNo` VARCHAR NULL DEFAULT NULL,
  `UserNo2` VARCHAR NULL DEFAULT NULL,
  `AccountName` MEDIUMTEXT NULL DEFAULT NULL,
  PRIMARY KEY (`id`)
);

-- ---
-- Foreign Keys
-- ---
ALTER TABLE `CRD1` ADD FOREIGN KEY (CardCode) REFERENCES `OCRD` (`CardCode`);
ALTER TABLE `CRD7` ADD FOREIGN KEY (CardCode) REFERENCES `OCRD` (`CardCode`);
ALTER TABLE `OCRB` ADD FOREIGN KEY (Cardcode) REFERENCES `OCRD` (`CardCode`);
```

---

## Agradecimentos hihiii ⭐⭐⭐⭐

![Imagem de agradecimento 1](https://i.pinimg.com/564x/86/65/1a/86651aa00febc0e81064721021af97d2.jpg)

![Imagem de agradecimento 2](https://i.pinimg.com/564x/38/bd/66/38bd669747f95f4085c2dfdc1f56fa84.jpg)
