# Comparing `tmp/trytond_edocument_uncefact-7.0.1.tar.gz` & `tmp/trytond_edocument_uncefact-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_edocument_uncefact-7.0.1.tar", last modified: Thu Feb 15 18:36:09 2024, max compression
+gzip compressed data, was "trytond_edocument_uncefact-7.2.0.tar", last modified: Mon Apr 29 15:40:41 2024, max compression
```

## Comparing `trytond_edocument_uncefact-7.0.1.tar` & `trytond_edocument_uncefact-7.2.0.tar`

### file list

```diff
@@ -1,118 +1,117 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.858070 trytond_edocument_uncefact-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-02-15 18:36:07.000000 trytond_edocument_uncefact-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-02-15 18:36:06.000000 trytond_edocument_uncefact-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2650 2024-02-15 18:36:09.858070 trytond_edocument_uncefact-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.851403 trytond_edocument_uncefact-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2024-02-05 16:24:27.000000 trytond_edocument_uncefact-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     6961 2024-02-10 10:11:06.000000 trytond_edocument_uncefact-7.0.1/edocument.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.851403 trytond_edocument_uncefact-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      158 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-15 18:36:09.858070 trytond_edocument_uncefact-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4566 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.824737 trytond_edocument_uncefact-7.0.1/template/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.851403 trytond_edocument_uncefact-7.0.1/template/16B-CII/
--rw-r--r--   0 ced       (1000) ced       (1000)     9285 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/template/16B-CII/CrossIndustryInvoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.851403 trytond_edocument_uncefact-7.0.1/tests/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.824737 trytond_edocument_uncefact-7.0.1/tests/16B-CII/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.824737 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.854736 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/
--rw-r--r--   0 ced       (1000) ced       (1000)     2224 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2068 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     7920 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5740 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5468 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5337 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5354 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2660 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2155 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     5198 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2281 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2593 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2698 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    26450 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3124 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3682 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2547 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3203 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3995 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1932 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2245 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     1896 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2093 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2093 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2025 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4140 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    14278 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     3579 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2576 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    21946 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2263 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2381 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4538 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4451 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2788 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    29382 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2054 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     4329 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2302 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    11400 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2169 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2854 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.824737 trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.858070 trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/
--rw-r--r--   0 ced       (1000) ced       (1000)     3048 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    47531 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    98059 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     6805 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.824737 trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.858070 trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/standard/
--rw-r--r--   0 ced       (1000) ced       (1000)    10120 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)    62572 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)     2127 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4408 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_edocument_uncefact-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       99 2024-02-05 16:24:27.000000 trytond_edocument_uncefact-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:36:09.858070 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2650 2024-02-15 18:36:09.000000 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     9351 2024-02-15 18:36:09.000000 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-15 18:36:09.000000 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-02-15 18:36:09.000000 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:49.000000 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-02-15 18:36:09.000000 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-15 18:36:09.000000 trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.759023 trytond_edocument_uncefact-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-04-29 15:19:56.000000 trytond_edocument_uncefact-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:19:56.000000 trytond_edocument_uncefact-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2650 2024-04-29 15:40:41.759023 trytond_edocument_uncefact-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.749023 trytond_edocument_uncefact-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3081 2024-04-27 16:30:39.000000 trytond_edocument_uncefact-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:10.000000 trytond_edocument_uncefact-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6934 2024-04-22 12:14:36.000000 trytond_edocument_uncefact-7.2.0/edocument.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.752356 trytond_edocument_uncefact-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      187 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      187 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      187 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      158 2024-04-27 16:43:24.000000 trytond_edocument_uncefact-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:41.759023 trytond_edocument_uncefact-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4566 2024-03-17 11:01:36.000000 trytond_edocument_uncefact-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.742356 trytond_edocument_uncefact-7.2.0/template/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.752356 trytond_edocument_uncefact-7.2.0/template/16B-CII/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9285 2024-02-04 18:51:26.000000 trytond_edocument_uncefact-7.2.0/template/16B-CII/CrossIndustryInvoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.752356 trytond_edocument_uncefact-7.2.0/tests/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.742356 trytond_edocument_uncefact-7.2.0/tests/16B-CII/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.742356 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.755689 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2224 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2068 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     7920 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5740 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5468 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5337 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5354 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2660 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2155 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1907 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     5198 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2281 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2593 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2698 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    26450 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3124 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3682 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2547 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3203 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3995 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1932 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2245 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1869 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     1896 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2093 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2093 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2025 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4140 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    14278 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     3579 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2576 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    21946 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2263 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2381 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4538 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4451 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2788 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    29382 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2054 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     4329 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2302 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    11400 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2169 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2854 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.742356 trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.755689 trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3048 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    47531 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    98059 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     6805 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.742356 trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.755689 trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/standard/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10120 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)    62572 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)     2127 2023-01-16 14:00:20.000000 trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_edocument_uncefact-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4408 2024-01-05 00:25:05.000000 trytond_edocument_uncefact-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:10.000000 trytond_edocument_uncefact-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       99 2024-04-29 15:19:52.000000 trytond_edocument_uncefact-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:41.755689 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2650 2024-04-29 15:40:41.000000 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     9333 2024-04-29 15:40:41.000000 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:41.000000 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       74 2024-04-29 15:40:41.000000 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-04-29 15:40:41.000000 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:41.000000 trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/top_level.txt
```

### Comparing `trytond_edocument_uncefact-7.0.1/CHANGELOG` & `trytond_edocument_uncefact-7.2.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-02-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_edocument_uncefact-7.0.1/COPYRIGHT` & `trytond_edocument_uncefact-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/LICENSE` & `trytond_edocument_uncefact-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/PKG-INFO` & `trytond_edocument_uncefact-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_edocument_uncefact
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for electronic document UN/CEFACT
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
-Requires-Dist: trytond_edocument_unece<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_edocument_unece<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 Requires-Dist: lxml; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 EDocument UN/CEFACT Module
 ##########################
 
 Implement electronic document from UN/CEFACT:
 
     * Cross-Industry-Invoice (16B-CII)
```

### Comparing `trytond_edocument_uncefact-7.0.1/doc/conf.py` & `trytond_edocument_uncefact-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
     modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+        'https://docs.tryton.org/${series}/modules-{module}/')
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import configparser
     import subprocess
     import sys
 
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_edocument_uncefact-7.0.1/edocument.py` & `trytond_edocument_uncefact-7.2.0/edocument.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             continue
         yield kind, data, pos
 
 
 class Invoice(Model):
     "EDocument UN/CEFACT Invoice"
     __name__ = 'edocument.uncefact.invoice'
-    __no_slots__ = True  # to work with cached_property
+    __slots__ = ('invoice',)
 
     @classmethod
     def __setup__(cls):
         super(Invoice, cls).__setup__()
         cls.__rpc__.update({
                 'render': RPC(instantiate=0),
                 })
```

### Comparing `trytond_edocument_uncefact-7.0.1/setup.py` & `trytond_edocument_uncefact-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/template/16B-CII/CrossIndustryInvoice.xml` & `trytond_edocument_uncefact-7.2.0/template/16B-CII/CrossIndustryInvoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAccountType_D11A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/EDIFICAS-EU_AccountingAmountType_D11A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/ISO_ISO3AlphaCurrencyCode_2012-08-31.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_ActionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AdjustmentReasonDescriptionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeIdentificationCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AllowanceChargeReasonCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_AutomaticDataCaptureMethodCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CargoOperationalCategoryCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CargoTypeCode_1996Rev2Final.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CommodityIdentificationCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_CommunicationMeansTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_ContactFunctionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DeliveryTermsCode_2010.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DimensionTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_Accounting_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DocumentNameCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DocumentStatusCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DutyTaxFeeTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_DutyorTaxorFeeCategoryCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_EquipmentSizeTypeDescriptionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCodePaymentTermsEvent_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_EventTimeReferenceCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeQuantityUnitBasisCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_FreightChargeTariffCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_GoodsTypeExtensionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeLinear_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeVolume_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MeasurementUnitCommonCodeWeight_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_MessageFunctionCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PackageTypeCode_2006.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PackagingMarkingCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_ChargePaying_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PartyRoleCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentGuaranteeMeansCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansChannelCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentMeansCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PaymentTermsTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_PriceTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_ReferenceTypeCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TimePointFormatCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentCategoryCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportEquipmentFullnessCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportMeansTypeCode_2007.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportModeCode_2.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/codelist/standard/UNECE_TransportMovementStageCode_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_QualifiedDataType_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_ReusableAggregateBusinessInformationEntity_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/data/standard/CrossIndustryInvoice_UnqualifiedDataType_100pD16B.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/standard/ISO_ISOTwo-letterCountryCode_SecondEdition2006.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/standard/UNECE_FreightCostCode_4.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd` & `trytond_edocument_uncefact-7.2.0/tests/16B-CII/identifierlist/standard/UNECE_PaymentTermsDescriptionIdentifier_D16A.xsd`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tests/test_module.py` & `trytond_edocument_uncefact-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/tox.ini` & `trytond_edocument_uncefact-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/PKG-INFO` & `trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_edocument_uncefact
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for electronic document UN/CEFACT
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,19 +48,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
-Requires-Dist: trytond_edocument_unece<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_edocument_unece<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 Requires-Dist: lxml; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 EDocument UN/CEFACT Module
 ##########################
 
 Implement electronic document from UN/CEFACT:
 
     * Cross-Industry-Invoice (16B-CII)
```

### Comparing `trytond_edocument_uncefact-7.0.1/trytond_edocument_uncefact.egg-info/SOURCES.txt` & `trytond_edocument_uncefact-7.2.0/trytond_edocument_uncefact.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 edocument.py
```

