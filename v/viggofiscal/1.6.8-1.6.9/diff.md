# Comparing `tmp/viggofiscal-1.6.8.tar.gz` & `tmp/viggofiscal-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggofiscal-1.6.8.tar", last modified: Mon Jul 31 17:26:57 2023, max compression
+gzip compressed data, was "viggofiscal-1.6.9.tar", last modified: Fri Aug  4 11:22:40 2023, max compression
```

## Comparing `viggofiscal-1.6.8.tar` & `viggofiscal-1.6.9.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.002925 viggofiscal-1.6.8/viggofiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.002925 viggofiscal-1.6.8/viggofiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.002925 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.006925 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.006925 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.006925 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.006925 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.006925 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/centro_resultado/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/centro_resultado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/centro_resultado/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/centro_resultado/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.006925 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/natureza_financeira/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/natureza_financeira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/natureza_financeira/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/natureza_financeira/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cfop/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cfop/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cfop/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstipi/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.010925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.014925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.014925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.014925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.014925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.014925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.014925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/origem/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/origem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/origem/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.014925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/portaria/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/portaria/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/portaria/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms_sugestao/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms_sugestao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms_sugestao/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms_sugestao/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.018925 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/unidade_medida/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-31 17:25:56.000000 viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:57.002925 viggofiscal-1.6.8/viggofiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 17:26:56.000000 viggofiscal-1.6.8/viggofiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-07-31 17:26:56.000000 viggofiscal-1.6.8/viggofiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:26:56.000000 viggofiscal-1.6.8/viggofiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 17:26:56.000000 viggofiscal-1.6.8/viggofiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 17:26:56.000000 viggofiscal-1.6.8/viggofiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.844894 viggofiscal-1.6.9/viggofiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.844894 viggofiscal-1.6.9/viggofiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/centro_resultado/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/centro_resultado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/centro_resultado/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/centro_resultado/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/natureza_financeira/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/natureza_financeira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/natureza_financeira/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/natureza_financeira/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.848894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cfop/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cfop/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cfop/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstipi/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/origem/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/origem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/origem/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.852894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/portaria/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/portaria/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/portaria/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms_sugestao/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms_sugestao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms_sugestao/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms_sugestao/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.856894 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/unidade_medida/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-04 11:21:53.000000 viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:22:40.844894 viggofiscal-1.6.9/viggofiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-04 11:22:40.000000 viggofiscal-1.6.9/viggofiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-08-04 11:22:40.000000 viggofiscal-1.6.9/viggofiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:22:40.000000 viggofiscal-1.6.9/viggofiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 11:22:40.000000 viggofiscal-1.6.9/viggofiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 11:22:40.000000 viggofiscal-1.6.9/viggofiscal.egg-info/top_level.txt
```

### Comparing `viggofiscal-1.6.8/viggofiscal/__init__.py` & `viggofiscal-1.6.9/viggofiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/calculo_fiscal/utils.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/calculo_fiscal/utils.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/centro_resultado/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/centro_resultado/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from viggofiscal.subsystem.financeiro.centro_resultado.resource \
     import CentroResultado
 
 
 class List(operation.List):
 
     def do(self, session, **kwargs):
-        id = kwargs.pop('id', None)
+        centro_resultado_id = kwargs.pop('centro_resultado_id', None)
 
         query = session.query(CentroResultado)
 
         query = self.manager.apply_filters(query, CentroResultado, **kwargs)
-        if id is not None:
-            query = query.filter(CentroResultado.id != id)
+        if centro_resultado_id is not None:
+            query = query.filter(CentroResultado.id != centro_resultado_id)
         query = query.distinct()
 
         total_rows = None
         if self.manager.with_pagination(**kwargs):
             total_rows = query.count()
 
         pagination = Pagination.get_pagination(CentroResultado, **kwargs)
```

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/centro_resultado/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/centro_resultado/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/natureza_financeira/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms_sugestao/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,32 @@
+from viggocore.common import manager
 from viggocore.common.subsystem import operation
 from viggocore.common.subsystem.pagination import Pagination
-from viggocore.common import manager
 
-from viggofiscal.subsystem.financeiro.natureza_financeira.resource \
-    import NaturezaFinanceira
+from viggofiscal.subsystem.parametrizacao.uficms_sugestao.resource import \
+    UficmsSugestao
 
 
 class List(operation.List):
 
     def do(self, session, **kwargs):
-        id = kwargs.pop('id', None)
-
-        query = session.query(NaturezaFinanceira)
+        query = session.query(UficmsSugestao)
+        query = self.manager.apply_filters(query, UficmsSugestao, **kwargs)
 
-        query = self.manager.apply_filters(query, NaturezaFinanceira, **kwargs)
-        if id is not None:
-            query = query.filter(NaturezaFinanceira.id != id)
-        query = query.distinct()
+        dict_compare = {}
+        query = self.manager.apply_filters_includes(
+            query, dict_compare, **kwargs)
 
         total_rows = None
         if self.manager.with_pagination(**kwargs):
             total_rows = query.count()
 
-        pagination = Pagination.get_pagination(NaturezaFinanceira, **kwargs)
+        pagination = Pagination.get_pagination(UficmsSugestao, **kwargs)
         if pagination.order_by is not None:
-            pagination.adjust_order_by(NaturezaFinanceira)
+            pagination.adjust_order_by(UficmsSugestao)
         query = self.driver.apply_pagination(query, pagination)
         result = query.all()
 
         return (result, total_rows)
 
 
 class Manager(manager.CommonManager):
```

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/natureza_financeira/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/natureza_financeira/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/financeiro/portador/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/financeiro/portador/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cfop/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cfop/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cfop/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cfop/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/csticms/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/csticms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstipi/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstipi/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/cstpis/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/cstpis/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/domain_org/router.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/domain_org/router.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/origem/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/origem/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/portaria/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/portaria/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/portaria/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/portaria/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/controller.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/terminal/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/terminal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/uficms_sugestao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py` & `viggofiscal-1.6.9/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.6.8/viggofiscal.egg-info/SOURCES.txt` & `viggofiscal-1.6.9/viggofiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

