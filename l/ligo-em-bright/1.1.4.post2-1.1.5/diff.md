# Comparing `tmp/ligo_em_bright-1.1.4.post2.tar.gz` & `tmp/ligo_em_bright-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo_em_bright-1.1.4.post2.tar", max compression
+gzip compressed data, was "ligo_em_bright-1.1.5.tar", max compression
```

## Comparing `ligo_em_bright-1.1.4.post2.tar` & `ligo_em_bright-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.4.post2/LICENSE
--rw-r--r--   0        0        0      985 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.4.post2/README.md
--rw-r--r--   0        0        0      834 2023-06-16 16:12:49.363769 ligo_em_bright-1.1.4.post2/ligo/em_bright/__init__.py
--rw-r--r--   0        0        0     9890 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.4.post2/ligo/em_bright/categorize.py
--rw-r--r--   0        0        0     9860 2023-06-16 13:38:30.690326 ligo_em_bright-1.1.4.post2/ligo/em_bright/computeDiskMass.py
--rw-r--r--   0        0        0    15224 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.4.post2/ligo/em_bright/dag_writer.py
--rw-r--r--   0        0        0     2407 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.4.post2/ligo/em_bright/data/__init__.py
--rw-r--r--   0        0        0     8609 2023-06-16 13:38:30.690326 ligo_em_bright-1.1.4.post2/ligo/em_bright/em_bright.py
--rw-r--r--   0        0        0        0 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.4.post2/ligo/em_bright/tests/__init__.py
--rw-r--r--   0        0        0      307 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.4.post2/ligo/em_bright/tests/data/test_categorize_data.tbl
--rw-r--r--   0        0        0    10374 2023-06-16 16:12:08.206384 ligo_em_bright-1.1.4.post2/ligo/em_bright/tests/test_em_bright.py
--rw-r--r--   0        0        0    23921 2023-04-07 01:46:47.038281 ligo_em_bright-1.1.4.post2/ligo/em_bright/utils.py
--rw-r--r--   0        0        0     1334 2023-06-16 16:13:56.657856 ligo_em_bright-1.1.4.post2/pyproject.toml
--rw-r--r--   0        0        0     1706 1970-01-01 00:00:00.000000 ligo_em_bright-1.1.4.post2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-02 19:51:52.112296 ligo_em_bright-1.1.5/LICENSE
+-rw-r--r--   0        0        0      977 2023-06-02 19:51:52.113296 ligo_em_bright-1.1.5/README.md
+-rw-r--r--   0        0        0      828 2023-08-04 19:28:07.424785 ligo_em_bright-1.1.5/ligo/em_bright/__init__.py
+-rw-r--r--   0        0        0     9617 2023-06-27 22:48:05.855588 ligo_em_bright-1.1.5/ligo/em_bright/categorize.py
+-rw-r--r--   0        0        0     9917 2023-08-04 19:27:32.802778 ligo_em_bright-1.1.5/ligo/em_bright/computeDiskMass.py
+-rw-r--r--   0        0        0    14843 2023-06-02 19:51:52.119296 ligo_em_bright-1.1.5/ligo/em_bright/dag_writer.py
+-rw-r--r--   0        0        0     2322 2023-06-02 19:51:53.643297 ligo_em_bright-1.1.5/ligo/em_bright/data/__init__.py
+-rw-r--r--   0        0        0    10888 2023-08-04 15:30:46.617468 ligo_em_bright-1.1.5/ligo/em_bright/em_bright.py
+-rw-r--r--   0        0        0        0 2023-06-02 19:51:53.645297 ligo_em_bright-1.1.5/ligo/em_bright/tests/__init__.py
+-rw-r--r--   0        0        0      303 2023-06-02 19:51:53.646297 ligo_em_bright-1.1.5/ligo/em_bright/tests/data/test_categorize_data.tbl
+-rw-r--r--   0        0        0    11237 2023-08-04 16:07:27.381322 ligo_em_bright-1.1.5/ligo/em_bright/tests/test_em_bright.py
+-rw-r--r--   0        0        0    23258 2023-06-02 19:51:53.648297 ligo_em_bright-1.1.5/ligo/em_bright/utils.py
+-rw-r--r--   0        0        0     1328 2023-08-04 16:05:22.102290 ligo_em_bright-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 ligo_em_bright-1.1.5/PKG-INFO
```

### Comparing `ligo_em_bright-1.1.4.post2/README.md` & `ligo_em_bright-1.1.5/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ligo.em_bright
-
-This library provides the tools to compute the possibility of merging gravitational-wave binaries to have an electromagnetic counterpart or having a component in the lower mass-gap region. The data products are source properties
-- `HasNS`: The mass of at least one of the compact binary coalescence is consistent with a neutron star.
-- `HasRemnant`: A non-zero amount of remnant matter remained outside the final compact object (a necessary but not sufficient condition to produce certain kinds of electromagnetic emission such as a short GRB or a kilonova).
-- `HasMassGap`: The mass of at least one of the compact binary coalescence is consistent with lower mass-gap region i.e. between 3-5 solar mass.
-
-The `HasNS` and `HasRemnant` quantities depend on, and are marginalized over, several neutron star equations of state (EOS). The marginalization is done using data from [GW170817](https://www.gw-openscience.org/eventapi/html/GWTC-1-confident/GW170817/).
+# ligo.em_bright
+
+This library provides the tools to compute the possibility of merging gravitational-wave binaries to have an electromagnetic counterpart or having a component in the lower mass-gap region. The data products are source properties
+- `HasNS`: The mass of at least one of the compact binary coalescence is consistent with a neutron star.
+- `HasRemnant`: A non-zero amount of remnant matter remained outside the final compact object (a necessary but not sufficient condition to produce certain kinds of electromagnetic emission such as a short GRB or a kilonova).
+- `HasMassGap`: The mass of at least one of the compact binary coalescence is consistent with lower mass-gap region i.e. between 3-5 solar mass.
+
+The `HasNS` and `HasRemnant` quantities depend on, and are marginalized over, several neutron star equations of state (EOS). The marginalization is done using data from [GW170817](https://www.gw-openscience.org/eventapi/html/GWTC-1-confident/GW170817/).
```

### Comparing `ligo_em_bright-1.1.4.post2/ligo/em_bright/__init__.py` & `ligo_em_bright-1.1.5/ligo/em_bright/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.1.4.post2'
+__version__ = '1.1.5'
 
 PACKAGE_DATA_BASE_URL = (
     'https://git.ligo.org/emfollow/em-properties/em-bright/'
     f'-/raw/v{__version__}/ligo/em_bright/data'
 )
 
 PACKAGE_DATA_LINKS = {name: f'{PACKAGE_DATA_BASE_URL}/{name}' for name in (
```

### Comparing `ligo_em_bright-1.1.4.post2/ligo/em_bright/categorize.py` & `ligo_em_bright-1.1.5/ligo/em_bright/categorize.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-# Copyright (C) 2020 Shaon Ghosh, Deep Chatterjee
-#
-# This program is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by the
-# Free Software Foundation; either version 2 of the License, or (at your
-# option) any later version.
-#
-# This program is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-
-
-import argparse
-import functools
-import os
-
-import numpy as np
-import pandas as pd
-import pickle
-
-from . import computeDiskMass
-from .data import EOS_BAYES_FACTORS, EOS_MAX_MASS
-
-
-class _TupleHandler(object):
-    def __call__(self, func):
-        @functools.wraps(func)
-        def handle(*args, **kwargs):
-            try:
-                (infile, outfile, max_mass, eosname), *_ = args
-            except (ValueError, TypeError):
-                return func(*args, **kwargs)
-            return func(infile, outfile, max_mass, eosname)
-        return handle
-
-
-def regularize(m1, m2, chi1, chi2):
-    '''Transform masses based on the convention m1 > m2.
-    Apply the same for spins.
-    '''
-    # Find cases where the mass2 is greater than the mass1
-    largerMass1 = m1 >= m2
-    largerMass2 = m2 > m1
-
-    # Set up vectors to store the regularized masses and spins
-    m_primary = np.zeros_like(m1)
-    m_secondary = np.zeros_like(m2)
-    chi_primary = np.zeros_like(chi1)
-    chi_secondary = np.zeros_like(chi2)
-
-    # Swap vales of masses if mass1 < mass2
-    m_primary[largerMass1] = m1[largerMass1]
-    m_primary[~largerMass1] = m2[largerMass2]
-    m_secondary[~largerMass2] = m2[~largerMass2]
-    m_secondary[largerMass2] = m1[~largerMass1]
-
-    # Assign the spin values accordingly
-    chi_primary[largerMass1] = chi1[largerMass1]
-    chi_primary[~largerMass1] = chi2[~largerMass1]
-    chi_secondary[~largerMass2] = chi2[~largerMass2]
-    chi_secondary[largerMass2] = chi1[~largerMass1]
-
-    return (m_primary, m_secondary, chi_primary, chi_secondary)
-
-
-@_TupleHandler()
-def embright_categorization(inFile, outFile, eosname='2H', mNs_mass=None):
-    '''Categorize whether the binary has a neutron star, and any non-zero
-    remnant post merger, based on the ``eosname``.
-
-    Parameters
-    ----------
-    inFile : str
-        input filename
-    outFile : str
-        output filename
-    eosname : str
-        neutron star equation of state. Assumed implemented in lalsimulation.
-        Default 2H.
-    mNS_mass : float
-        Provide to override the maximum mass from ``eosname``.
-    '''
-    df = pd.read_table(inFile, delimiter='\t')
-    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
-    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
-    redshift_inj = df.inj_redshift.values
-    m1_inj_source = m1_inj / (1 + redshift_inj)
-    m2_inj_source = m2_inj / (1 + redshift_inj)
-
-    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
-    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
-    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
-        m1_inj, m2_inj, chi1_inj, chi2_inj
-    )
-    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
-        m1_rec, m2_rec, chi1_rec, chi2_rec
-    )
-    m1_inj_source, m2_inj_source, _, _ = regularize(
-        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
-    )  # spins regularized from previous step.
-    if mNs_mass:
-        NS_classified = m2_inj_source < mNs_mass
-    else:
-        NS_classified = m2_inj_source < EOS_MAX_MASS[eosname]
-    NS_classified = NS_classified.astype(int)
-
-    R_isco_hat_inj = computeDiskMass.compute_isco(chi1_inj)
-    R_isco_hat_rec = computeDiskMass.compute_isco(chi1_rec)
-
-    Compactness_inj, *_ = computeDiskMass.computeCompactness(m2_inj,
-                                                             eosname=eosname)
-    Compactness_rec, *_ = computeDiskMass.computeCompactness(m2_rec,
-                                                             eosname=eosname)
-
-    mc_inj = (m1_inj*m2_inj)**(3/5)/((m1_inj + m2_inj)**(1/5))
-    mc_rec = (m1_rec*m2_rec)**(3/5)/((m1_rec + m2_rec)**(1/5))
-
-    frac_mc_err = np.abs(mc_inj - mc_rec)/mc_inj
-
-    q_inj = m1_inj/m2_inj
-    q_rec = m1_rec/m2_rec
-
-    disk_mass_inj = computeDiskMass.computeDiskMass(
-        m1_inj_source, m2_inj_source, chi1_inj,
-        chi2_inj, eosname=eosname
-    )
-    EMB_classified = disk_mass_inj > 1e-3
-    EMB_classified = EMB_classified.astype(int)
-
-    output = np.vstack(
-        (m1_inj, m2_inj, chi1_inj, chi2_inj, redshift_inj,
-         mc_inj, q_inj, R_isco_hat_inj, Compactness_inj,
-         m1_rec, m2_rec, chi1_rec, chi2_rec,
-         mc_rec, frac_mc_err, q_rec, R_isco_hat_rec, Compactness_rec,
-         df.cfar.values, df.snr.values, df.gpstime.values, NS_classified,
-         EMB_classified)
-    ).T
-
-    df_complete = pd.DataFrame(output, columns=[
-        'm1_inj', 'm2_inj', 'chi1_inj', 'chi2_inj', 'inj_redshift',
-        'mc_inj', 'q_inj', 'R_isco_inj', 'Compactness_inj',
-        'm1_rec', 'm2_rec', 'chi1_rec', 'chi2_rec', 'mc_rec',
-        'frac_mc_err', 'q_rec', 'R_isco_rec', 'Compactness_rec',
-        'cfar', 'snr', 'gpstime', 'NS', 'EMB']
-    )
-    # drop NSs above max-mass
-    try:
-        max_mass = EOS_MAX_MASS[eosname]
-    except KeyError:
-        raise NotImplementedError
-    drop_mask = (m1_inj_source > max_mass) & (m1_inj_source < 3.0)  # noqa: E501; Restricts m2 by construction
-    df_complete = df_complete.loc[~drop_mask]
-    with open(outFile, 'wb') as f:
-        pickle.dump(df_complete, f)
-    return df_complete
-
-
-@_TupleHandler()
-def mass_gap_categorization(inFile, outFile):
-    '''Categorize whether the binary is in the lower mass gap
-    i.e., any component is between 3 and 5 solar mass
-
-    Parameters
-    ----------
-    inFile : str
-        input filename
-    outFile : str
-        output filename
-    '''
-    df = pd.read_table(inFile, delimiter='\t')
-    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
-    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
-    redshift_inj = df.inj_redshift.values
-    m1_inj_source = m1_inj / (1 + redshift_inj)
-    m2_inj_source = m2_inj / (1 + redshift_inj)
-
-    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
-    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
-    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
-        m1_inj, m2_inj, chi1_inj, chi2_inj
-    )
-    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
-        m1_rec, m2_rec, chi1_rec, chi2_rec
-    )
-    m1_inj_source, m2_inj_source, _, _ = regularize(
-        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
-    )  # spins regularized from previous step.
-    massgap_classified = (m1_inj_source > 3.0) & (m1_inj_source < 5.0)
-    massgap_classified += (m2_inj_source > 3.0) & (m2_inj_source < 5.0)
-    output = np.vstack(
-        (m1_inj_source, m2_inj_source, m1_inj, m2_inj, chi1_inj,
-         chi2_inj, redshift_inj, m1_rec, m2_rec, chi1_rec, chi2_rec,
-         df.cfar.values, df.snr.values, df.gpstime.values,
-         massgap_classified)
-    ).T
-
-    df_complete = pd.DataFrame(output, columns=[
-        'm1_inj_source', 'm2_inj_source', 'm1_inj', 'm2_inj', 'chi1_inj',
-        'chi2_inj', 'inj_redshift', 'm1_rec', 'm2_rec', 'chi1_rec',
-        'chi2_rec', 'cfar', 'snr', 'gpstime', 'mass_gap']
-    )
-    with open(outFile, 'wb') as f:
-        pickle.dump(df_complete, f)
-    return df_complete
-
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-i", "--input", action="store", type=str,
-                        help="Name of the input file")
-    parser.add_argument("-o", "--output", action="store", type=str,
-                        help="Name of the output file")
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument(
-        "-e", "--eosname", default='2H',
-        help="Equation of state used compute remnant matter."
-    )
-    group.add_argument(
-        "--mass-gap", required=False, action="store_true",
-        default=False, help="Supply for mass gap categorization")
-
-    args = parser.parse_args()
-
-    if args.mass_gap:
-        mass_gap_categorization(args.input, args.output)
-    else:
-        embright_categorization(args.input, args.output,
-                                eosname=args.eosname)
-
-
-def main_all():
-    parser = argparse.ArgumentParser(
-        "Run categorization on all available EoSs: "
-        f"{EOS_BAYES_FACTORS.keys()}\n"
-        "Output will be tagged by EoS names."
-    )
-    parser.add_argument(
-        "-i", "--input", action="store", type=str,
-        help="Name of the input file"
-    )
-    parser.add_argument(
-        "-d", "--output-directory", type=str,
-        help="Output directory"
-    )
-    parser.add_argument(
-        "-o", "--output-prefix", action="store",
-        type=str, help="Input prefix "
-    )
-    parser.add_argument(
-        "-p", "--pool", default=1, type=int,
-        help="Pool size"
-    )
-    args = parser.parse_args()
-
-    from multiprocessing import Pool
-    eos_args = [
-        (
-            args.input, os.path.join(
-                args.output_directory,
-                f"{args.output_prefix}_{eosname}.pkl"
-            ),
-            EOS_MAX_MASS[eosname],
-            eosname
-        )
-        for eosname in EOS_BAYES_FACTORS
-    ]
-    with Pool(args.pool) as p:
-        p.map(embright_categorization, eos_args)
+# Copyright (C) 2020 Shaon Ghosh, Deep Chatterjee
+#
+# This program is free software; you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation; either version 2 of the License, or (at your
+# option) any later version.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
+# Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+
+
+import argparse
+import functools
+import os
+
+import numpy as np
+import pandas as pd
+import pickle
+
+from . import computeDiskMass
+from .data import EOS_BAYES_FACTORS, EOS_MAX_MASS
+
+
+class _TupleHandler(object):
+    def __call__(self, func):
+        @functools.wraps(func)
+        def handle(*args, **kwargs):
+            try:
+                (infile, outfile, max_mass, eosname), *_ = args
+            except (ValueError, TypeError):
+                return func(*args, **kwargs)
+            return func(infile, outfile, max_mass, eosname)
+        return handle
+
+
+def regularize(m1, m2, chi1, chi2):
+    '''Transform masses based on the convention m1 > m2.
+    Apply the same for spins.
+    '''
+    # Find cases where the mass2 is greater than the mass1
+    largerMass1 = m1 >= m2
+    largerMass2 = m2 > m1
+
+    # Set up vectors to store the regularized masses and spins
+    m_primary = np.zeros_like(m1)
+    m_secondary = np.zeros_like(m2)
+    chi_primary = np.zeros_like(chi1)
+    chi_secondary = np.zeros_like(chi2)
+
+    # Swap vales of masses if mass1 < mass2
+    m_primary[largerMass1] = m1[largerMass1]
+    m_primary[~largerMass1] = m2[largerMass2]
+    m_secondary[~largerMass2] = m2[~largerMass2]
+    m_secondary[largerMass2] = m1[~largerMass1]
+
+    # Assign the spin values accordingly
+    chi_primary[largerMass1] = chi1[largerMass1]
+    chi_primary[~largerMass1] = chi2[~largerMass1]
+    chi_secondary[~largerMass2] = chi2[~largerMass2]
+    chi_secondary[largerMass2] = chi1[~largerMass1]
+
+    return (m_primary, m_secondary, chi_primary, chi_secondary)
+
+
+@_TupleHandler()
+def embright_categorization(inFile, outFile, eosname='2H', mNs_mass=None):
+    '''Categorize whether the binary has a neutron star, and any non-zero
+    remnant post merger, based on the ``eosname``.
+
+    Parameters
+    ----------
+    inFile : str
+        input filename
+    outFile : str
+        output filename
+    eosname : str
+        neutron star equation of state. Assumed implemented in lalsimulation.
+        Default 2H.
+    mNS_mass : float
+        Provide to override the maximum mass from ``eosname``.
+    '''
+    df = pd.read_table(inFile, delimiter='\t')
+    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
+    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
+    redshift_inj = df.inj_redshift.values
+    m1_inj_source = m1_inj / (1 + redshift_inj)
+    m2_inj_source = m2_inj / (1 + redshift_inj)
+
+    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
+    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
+    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
+        m1_inj, m2_inj, chi1_inj, chi2_inj
+    )
+    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
+        m1_rec, m2_rec, chi1_rec, chi2_rec
+    )
+    m1_inj_source, m2_inj_source, _, _ = regularize(
+        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
+    )  # spins regularized from previous step.
+    if mNs_mass:
+        NS_classified = m2_inj_source < mNs_mass
+    else:
+        NS_classified = m2_inj_source < EOS_MAX_MASS[eosname]
+    NS_classified = NS_classified.astype(int)
+
+    R_isco_hat_inj = computeDiskMass.compute_isco(chi1_inj)
+    R_isco_hat_rec = computeDiskMass.compute_isco(chi1_rec)
+
+    Compactness_inj, *_ = computeDiskMass.computeCompactness(m2_inj,
+                                                             eosname=eosname)
+    Compactness_rec, *_ = computeDiskMass.computeCompactness(m2_rec,
+                                                             eosname=eosname)
+
+    mc_inj = (m1_inj*m2_inj)**(3/5)/((m1_inj + m2_inj)**(1/5))
+    mc_rec = (m1_rec*m2_rec)**(3/5)/((m1_rec + m2_rec)**(1/5))
+
+    frac_mc_err = np.abs(mc_inj - mc_rec)/mc_inj
+
+    q_inj = m1_inj/m2_inj
+    q_rec = m1_rec/m2_rec
+
+    disk_mass_inj = computeDiskMass.computeDiskMass(
+        m1_inj_source, m2_inj_source, chi1_inj,
+        chi2_inj, eosname=eosname
+    )
+    EMB_classified = disk_mass_inj > 1e-3
+    EMB_classified = EMB_classified.astype(int)
+
+    output = np.vstack(
+        (m1_inj, m2_inj, chi1_inj, chi2_inj, redshift_inj,
+         mc_inj, q_inj, R_isco_hat_inj, Compactness_inj,
+         m1_rec, m2_rec, chi1_rec, chi2_rec,
+         mc_rec, frac_mc_err, q_rec, R_isco_hat_rec, Compactness_rec,
+         df.cfar.values, df.snr.values, df.gpstime.values, NS_classified,
+         EMB_classified)
+    ).T
+
+    df_complete = pd.DataFrame(output, columns=[
+        'm1_inj', 'm2_inj', 'chi1_inj', 'chi2_inj', 'inj_redshift',
+        'mc_inj', 'q_inj', 'R_isco_inj', 'Compactness_inj',
+        'm1_rec', 'm2_rec', 'chi1_rec', 'chi2_rec', 'mc_rec',
+        'frac_mc_err', 'q_rec', 'R_isco_rec', 'Compactness_rec',
+        'cfar', 'snr', 'gpstime', 'NS', 'EMB']
+    )
+    # drop NSs above max-mass
+    try:
+        max_mass = EOS_MAX_MASS[eosname]
+    except KeyError:
+        raise NotImplementedError
+    drop_mask = (m1_inj_source > max_mass) & (m1_inj_source < 3.0)  # noqa: E501; Restricts m2 by construction
+    df_complete = df_complete.loc[~drop_mask]
+    with open(outFile, 'wb') as f:
+        pickle.dump(df_complete, f)
+    return df_complete
+
+
+@_TupleHandler()
+def mass_gap_categorization(inFile, outFile):
+    '''Categorize whether the binary is in the lower mass gap
+    i.e., any component is between 3 and 5 solar mass
+
+    Parameters
+    ----------
+    inFile : str
+        input filename
+    outFile : str
+        output filename
+    '''
+    df = pd.read_table(inFile, delimiter='\t')
+    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
+    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
+    redshift_inj = df.inj_redshift.values
+    m1_inj_source = m1_inj / (1 + redshift_inj)
+    m2_inj_source = m2_inj / (1 + redshift_inj)
+
+    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
+    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
+    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
+        m1_inj, m2_inj, chi1_inj, chi2_inj
+    )
+    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
+        m1_rec, m2_rec, chi1_rec, chi2_rec
+    )
+    m1_inj_source, m2_inj_source, _, _ = regularize(
+        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
+    )  # spins regularized from previous step.
+    massgap_classified = (m1_inj_source > 3.0) & (m1_inj_source < 5.0)
+    massgap_classified += (m2_inj_source > 3.0) & (m2_inj_source < 5.0)
+    output = np.vstack(
+        (m1_inj_source, m2_inj_source, m1_inj, m2_inj, chi1_inj,
+         chi2_inj, redshift_inj, m1_rec, m2_rec, chi1_rec, chi2_rec,
+         df.cfar.values, df.snr.values, df.gpstime.values,
+         massgap_classified)
+    ).T
+
+    df_complete = pd.DataFrame(output, columns=[
+        'm1_inj_source', 'm2_inj_source', 'm1_inj', 'm2_inj', 'chi1_inj',
+        'chi2_inj', 'inj_redshift', 'm1_rec', 'm2_rec', 'chi1_rec',
+        'chi2_rec', 'cfar', 'snr', 'gpstime', 'mass_gap']
+    )
+    with open(outFile, 'wb') as f:
+        pickle.dump(df_complete, f)
+    return df_complete
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-i", "--input", action="store", type=str,
+                        help="Name of the input file")
+    parser.add_argument("-o", "--output", action="store", type=str,
+                        help="Name of the output file")
+    group = parser.add_mutually_exclusive_group()
+    group.add_argument(
+        "-e", "--eosname", default='2H',
+        help="Equation of state used compute remnant matter."
+    )
+    group.add_argument(
+        "--mass-gap", required=False, action="store_true",
+        default=False, help="Supply for mass gap categorization")
+
+    args = parser.parse_args()
+
+    if args.mass_gap:
+        mass_gap_categorization(args.input, args.output)
+    else:
+        embright_categorization(args.input, args.output,
+                                eosname=args.eosname)
+
+
+def main_all():
+    parser = argparse.ArgumentParser(
+        "Run categorization on all available EoSs: "
+        f"{EOS_BAYES_FACTORS.keys()}\n"
+        "Output will be tagged by EoS names."
+    )
+    parser.add_argument(
+        "-i", "--input", action="store", type=str,
+        help="Name of the input file"
+    )
+    parser.add_argument(
+        "-d", "--output-directory", type=str,
+        help="Output directory"
+    )
+    parser.add_argument(
+        "-o", "--output-prefix", action="store",
+        type=str, help="Input prefix "
+    )
+    parser.add_argument(
+        "-p", "--pool", default=1, type=int,
+        help="Pool size"
+    )
+    args = parser.parse_args()
+
+    from multiprocessing import Pool
+    eos_args = [
+        (
+            args.input, os.path.join(
+                args.output_directory,
+                f"{args.output_prefix}_{eosname}.pkl"
+            ),
+            EOS_MAX_MASS[eosname],
+            eosname
+        )
+        for eosname in EOS_BAYES_FACTORS
+    ]
+    with Pool(args.pool) as p:
+        p.map(embright_categorization, eos_args)
```

### Comparing `ligo_em_bright-1.1.4.post2/ligo/em_bright/computeDiskMass.py` & `ligo_em_bright-1.1.5/ligo/em_bright/computeDiskMass.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,69 +60,72 @@
     d1 = 0.619
     d2 = 0.1359
     BE = (d1*C_ns + d2*C_ns*C_ns) * m_ns  # arXiv:1601.06083 (Eq: 21)
     m2_b = m_ns + BE  # Baryonic mass - Gravitational mass = Binding Energy
     return [C_ns, m2_b]
 
 
-def computeCompactness(M_ns, eosname='2H', R_ns=None,
-                       max_mass=2.834648092299807):
+def max_mass_from_eosname(eosname):
+    if eosname == "2H":
+        max_mass = 2.834648092299807
+    else:
+        eos = lalsim.SimNeutronStarEOSByName(eosname)
+        fam = lalsim.CreateSimNeutronStarFamily(eos)
+        max_mass = lalsim.SimNeutronStarMaximumMass(fam)/c.M_sun.value
+    return max_mass
+
+
+def computeCompactness(M_ns, eosname='2H', max_mass=None):
     '''
     Return the neutron star compactness as a function of mass
     and equation of state or radius
 
     Parameters
     ----------
     M_ns : array_like
         Neutron star mass in solar masses
     eosname : str or interp1d
         Neutron star equation of state to be used
-    R_ns : array_like
-        Neutron star radius in m.
     max_mass : float
         Maximum mass of neutron star.
 
     Returns
     -------
     [C_ns, m2_b, max_mass]
         Compactness, baryon mass and maximum neutron star mass
         in solar masses.
 
     Notes
     -----
     The radius and maximum mass of the neutron star is
     inferred based on the equation of state supplied.
-    Supply explicitly if `eosname=None`.
+    Max mass only needs to be supplied for EoS marginalization.
 
     Examples
     --------
     >>> computeCompactness(2.8)
     [array(0.298), array(3.354), 2.834]
     >>> computeDiskMass.computeCompactness(2.9, eosname='AP4')
     [0.5, 0.0, 2.212]
     >>> m_ns = np.array([1.1, 1.2, 1.3])
     >>> computeDiskMass.computeCompactness(m_ns, eosname='AP4')
     [array([0.141, 0.154, 0.167]), array([1.199, 1.318, 1.439]), 2.212]
-    >>> computeCompactness(2.1, R_ns=16000, eosname=None, max_mass=2.5)
-    [0.193, 2.362, 2.5]
     '''
-    if R_ns:
-        C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
-    elif isinstance(eosname, interp1d):
+    if isinstance(eosname, interp1d):
         # find R as a function of M
         R_ns = eosname(M_ns)
         C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
     elif eosname != '2H':
         # infer radius and maximum mass based on lalsimulation EoS
         R_ns, max_mass = _r_ns_from_lal_simulation(M_ns, eosname)
         C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
     else:
         with open(PACKAGE_FILENAMES['equil_2H.dat'], 'rb') as f:
             M_g, M_b, Compactness = np.loadtxt(f, unpack=True)
-        max_mass = 2.834648092299807
+        max_mass = max_mass_from_eosname("2H")
         s = UnivariateSpline(M_g, Compactness, k=5)
         s_b = UnivariateSpline(M_g, M_b, k=5)
         C_ns = s(M_ns)
         m2_b = s_b(M_ns)
     try:
         C_ns[M_ns > max_mass] = 0.5  # BH compactness set to 0.5
         m2_b[M_ns > max_mass] = 0.0  # BH baryon mass set to 0.0
@@ -240,21 +243,20 @@
         else:
             m_primary = m2
             m_secondary = m1
             chi_primary = chi2
             chi_secondary = chi1
 
     [C_ns, m2_b, max_mass] = computeCompactness(m_secondary, eosname=eosname,
-                                                R_ns=R_ns, max_mass=max_mass)
+                                                max_mass=max_mass)
 
     eta = m_primary*m_secondary/(m_primary + m_secondary)**2
     BBH = m_secondary > max_mass
     BNS = m_primary < max_mass
-    # FIXME
-    if type(BNS) != np.ndarray:
+    if not isinstance(BNS, np.ndarray):
         if BNS or BBH:
             return float(not (BBH) or BNS)
 
     if not kerr:
         alpha = 0.406
         beta = 0.139
         gamma = 0.255
@@ -281,11 +283,11 @@
 
     if hasattr(combinedTerms, 'ndim') and combinedTerms.ndim >= 1:
         lessthanzero = combinedTerms < 0.0
         combinedTerms[lessthanzero] = 0.0
     else:
         combinedTerms = 0 if combinedTerms < 0 else combinedTerms
     M_rem = (combinedTerms**delta)*m2_b
-    if type(BNS) == np.ndarray:
+    if isinstance(BNS, np.ndarray):
         M_rem[BBH] = 0.0  # BBH is always EM-Dark
         M_rem[BNS] = 1.0  # Ad hoc value, assuming BNS is always EM-Bright
     return M_rem
```

### Comparing `ligo_em_bright-1.1.4.post2/ligo/em_bright/dag_writer.py` & `ligo_em_bright-1.1.5/ligo/em_bright/dag_writer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,381 +1,381 @@
-# Copyright(C) 2018-2022 Shaon Ghosh, Deep Chatterjee, Sushant Sharma Chaudhary
-#
-# This program is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by the
-# Free Software Foundation; either version 2 of the License, or (at your
-# option) any later version.
-#
-# This program is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-
-
-import os
-import re
-import shutil
-
-from argparse import ArgumentParser
-from configparser import ConfigParser
-from glob import glob
-
-from .data import EOS_BAYES_FACTORS
-
-try:
-    import htcondor
-    from htcondor import dags
-    _HTCONDOR_INSTALLED = True
-except ModuleNotFoundError:
-    _HTCONDOR_INSTALLED = False
-    import warnings
-    warnings.warn(
-        "HTCondor python bindings need to be installed to use this script. "
-        "This script is only used in training. When training new classifiers, "
-        "create a developmental version by cloning the git repository, "
-        "and installing from the lock file."
-    )
-
-
-def _add_common_workflow(condor_dag, args, common_submit_dict):
-    config = ConfigParser()
-    config.read(args.config)
-    config_path = os.path.abspath(args.config)
-    abs_work_dir = os.path.abspath(args.work_dir)
-    file_dir = args.file_dir
-    # Get injection directory
-    inj_file_pattern = config.get('core',
-                                  'inj_file_pattern')
-    sqlite_run_tag = config.get('core',
-                                'sqlite_run_tag')
-
-    # Get input and output file names prefixes
-    em_bright_extract_prefix = config.get('output_filenames',
-                                          'em_bright_extract_prefix')
-    em_bright_extract_suffix = config.get('output_filenames',
-                                          'em_bright_extract_suffix')
-    em_bright_join_prefix = config.get('output_filenames',
-                                       'em_bright_join_prefix')
-    em_bright_join_suffix = config.get('output_filenames',
-                                       'em_bright_join_suffix')
-    # Get executable names
-    em_bright_extract_executable = config.get('executables',
-                                              'em_bright_extract')
-    em_bright_join_executable = config.get('executables',
-                                           'em_bright_join')
-
-    # Define the executable arguments association
-    exec_arg_assoc = {
-        em_bright_extract_executable:
-            " --input $(macroinput) --output $(macrooutput)",
-        em_bright_join_executable:
-            " --input $(macroinput) --config $(macroconfig)"
-            " --output $(macrooutput)"
-    }
-    # create a dictionary of Submit instances
-    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
-    # create all sub files
-
-    for exect, arg_sub in exec_arg_assoc.items():
-        common_submit_dict["executable"] = exect
-        common_submit_dict["arguments"] = arg_sub
-        condor_sub_dict[exect] = htcondor.Submit(
-            common_submit_dict)
-    # Creating list of sqlite files to create the dag
-    inj_list = glob(
-        os.path.join(
-            os.path.abspath(file_dir), inj_file_pattern
-        )
-    )
-
-    # get vars for em_bright_extract layer
-    em_bright_extract_vars = []
-    for idx, injFilename in enumerate(inj_list):
-        match = re.search(sqlite_run_tag, os.path.basename(injFilename))
-        if match is None:
-            continue
-        prefix, startT, duration = match.groups()
-        # filename for INJCOINC files
-        output_fname = \
-            em_bright_extract_prefix + \
-            prefix + '-' + startT + '-' + duration + em_bright_extract_suffix
-        em_bright_extract_vars.append(
-            dict(
-                macroinput=injFilename,
-                macrooutput=output_fname
-            )
-        )
-    em_bright_extract_layer = condor_dag.layer(
-        name=em_bright_extract_executable,
-        submit_description=condor_sub_dict[em_bright_extract_executable],
-        vars=em_bright_extract_vars
-    )
-    # output for JOIN
-    join_output = \
-        em_bright_join_prefix + '-' + startT + '-' + \
-        duration + em_bright_join_suffix
-    join_output = os.path.join(abs_work_dir, join_output)
-
-    em_bright_join_vars = [
-        dict(
-            macroinput=abs_work_dir,
-            macrooutput=join_output,
-            macroconfig=config_path
-        )
-    ]
-    em_bright_join_layer = em_bright_extract_layer.child_layer(
-        name=em_bright_join_executable,
-        submit_description=condor_sub_dict[em_bright_join_executable],
-        vars=em_bright_join_vars
-    )
-    join_output_dict = {
-        "output": join_output,
-        "startT": startT,
-        "duration": duration
-    }
-    return em_bright_join_layer, join_output_dict
-
-
-def _add_knn_workflow(em_bright_join_layer, args,
-                      common_submit_dict,
-                      join_output_dict):
-    config = ConfigParser()
-    config.read(args.config)
-    config_path = os.path.abspath(args.config)
-    abs_work_dir = os.path.abspath(args.work_dir)
-
-    em_bright_categorize_prefix = config.get('output_filenames',
-                                             'em_bright_categorize_prefix')
-    em_bright_categorize_suffix = config.get('output_filenames',
-                                             'em_bright_categorize_suffix')
-    em_bright_train_prefix = config.get('output_filenames',
-                                        'em_bright_train_prefix')
-    em_bright_train_suffix = config.get('output_filenames',
-                                        'em_bright_train_suffix')
-    em_bright_categorize_executable = config.get('executables',
-                                                 'em_bright_categorize')
-    em_bright_train_executable = config.get('executables',
-                                            'em_bright_train')
-    em_bright_paramater_sweep_plot_executable = config.get(
-            'executables', 'em_bright_create_param_sweep_plot'
-    )
-    exec_arg_assoc = {
-        em_bright_train_executable:
-            " --input $(macroinput) --config $(macroconfig) "
-            "--output $(macrooutput) --param-sweep-plot-prefix $(macroeos)",
-        em_bright_paramater_sweep_plot_executable:
-            " --input $(macroinput) --config $(macroconfig)"
-            " --verbose",
-        em_bright_categorize_executable:
-            " --input $(macroinput) --output $(macrooutput)"
-            " --eosname $(macroeos) "
-    }
-    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
-
-    for exect, arg_sub in exec_arg_assoc.items():
-        common_submit_dict["executable"] = exect
-        common_submit_dict["arguments"] = arg_sub
-        condor_sub_dict[exect] = htcondor.Submit(
-            common_submit_dict)
-
-    # input and output for CATEGORIZE/TRAIN
-    em_bright_categorize_vars = list()
-    em_bright_train_vars = list()
-    categorize_input = join_output_dict["output"]
-
-    for em_bright_eos in EOS_BAYES_FACTORS:
-        categorize_output = \
-            em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
-            '-' + join_output_dict["duration"] + '-' + em_bright_eos + \
-            em_bright_categorize_suffix
-        categorize_output = os.path.join(abs_work_dir, categorize_output)
-
-        train_output = \
-            em_bright_train_prefix + '-' + join_output_dict["startT"] + \
-            '-' + join_output_dict["duration"] + \
-            '-' + em_bright_eos + em_bright_train_suffix
-        train_output = os.path.join(abs_work_dir, train_output)
-
-        em_bright_categorize_vars.append(
-            dict(
-                macroinput=categorize_input,
-                macrooutput=categorize_output,
-                macroeos=em_bright_eos,
-            )
-        )
-        em_bright_train_vars.append(
-                dict(
-                    macroinput=categorize_output,
-                    macrooutput=train_output,
-                    macroconfig=config_path,
-                    macroeos=em_bright_eos
-                )
-            )
-
-    em_bright_categorize_layer = em_bright_join_layer.child_layer(
-        name=em_bright_categorize_executable,
-        submit_description=condor_sub_dict[em_bright_categorize_executable],
-        vars=em_bright_categorize_vars
-    )
-
-    em_bright_train_layer = em_bright_categorize_layer.child_layer(
-            name=em_bright_train_executable,
-            submit_description=condor_sub_dict[em_bright_train_executable],
-            vars=em_bright_train_vars
-        )
-
-    em_bright_param_sweep_layer = em_bright_train_layer.child_layer(  # noqa: F841,E501
-            name=em_bright_paramater_sweep_plot_executable,
-            submit_description=condor_sub_dict[
-                em_bright_paramater_sweep_plot_executable],
-            vars=[
-                dict(
-                    macroinput=abs_work_dir,
-                    macroconfig=config_path
-                )
-            ]
-        )
-
-
-def _add_massgap_workflow(em_bright_join_layer, args,
-                          common_submit_dict,
-                          join_output_dict):
-    config = ConfigParser()
-    config.read(args.config)
-    config_path = os.path.abspath(args.config)
-    abs_work_dir = os.path.abspath(args.work_dir)
-
-    em_bright_categorize_prefix = config.get('output_filenames',
-                                             'em_bright_categorize_prefix')
-    em_bright_categorize_suffix = config.get('output_filenames',
-                                             'em_bright_categorize_suffix')
-    em_bright_train_suffix = config.get('output_filenames',
-                                        'em_bright_train_suffix')
-    em_bright_categorize_executable = config.get('executables',
-                                                 'em_bright_categorize')
-    em_bright_train_executable = config.get('executables',
-                                            'em_bright_train')
-    exec_arg_assoc = {
-        em_bright_categorize_executable:
-            " --input $(macroinput) --output $(macrooutput)"
-            " --mass-gap",
-        em_bright_train_executable:
-            " --input $(macroinput) --config $(macroconfig)"
-            " --output $(macrooutput) --mass-gap"
-    }
-    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
-    for exect, arg_sub in exec_arg_assoc.items():
-        common_submit_dict["executable"] = exect
-        common_submit_dict["arguments"] = arg_sub
-        condor_sub_dict[exect] = htcondor.Submit(
-            common_submit_dict)
-
-    categorize_input = join_output_dict["output"]
-    categorize_output = \
-        em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
-        '-' + join_output_dict["duration"] + \
-        em_bright_categorize_suffix
-    categorize_output = os.path.join(abs_work_dir, categorize_output)
-
-    em_bright_categorize_vars = [
-            dict(
-                macroinput=categorize_input,
-                macrooutput=categorize_output,
-            )
-    ]
-    em_bright_categorize_layer = em_bright_join_layer.child_layer(
-        name=em_bright_categorize_executable,
-        submit_description=condor_sub_dict[em_bright_categorize_executable],
-        vars=em_bright_categorize_vars
-    )
-
-    train_output = "mass_gap" + \
-        em_bright_train_suffix
-    train_output = os.path.join(abs_work_dir, train_output)
-
-    em_bright_train_vars = [
-         dict(
-                macroinput=categorize_output,
-                macrooutput=train_output,
-                macroconfig=config_path,
-            )
-    ]
-    em_bright_categorize_layer.child_layer(
-            name=em_bright_train_executable,
-            submit_description=condor_sub_dict[em_bright_train_executable],
-            vars=em_bright_train_vars
-        )
-
-
-def main():
-    parser = ArgumentParser("Condor DAG writer for workflow")
-    parser.add_argument("-d", "--dagname", required=True,
-                        help="Name of the dag file. Placed under --work-dir")
-    parser.add_argument("-w", "--work-dir", required=True,
-                        help="Working directory to store data outputs")
-    parser.add_argument(
-        "-i", "--file-dir", required=True,
-        help="File containing input injection sqlite databases"
-    )
-    parser.add_argument("-c", "--config", required=True,
-                        help="Name of the config file")
-    parser.add_argument("-e", "--executables-dir", required=True,
-                        help="Directory containing executables")
-    parser.add_argument("--mass-gap", action='store_true',
-                        help="use --random_forest for Random Forest Mode")
-    args = parser.parse_args()
-
-    assert _HTCONDOR_INSTALLED, "HTCondor python bindings missing."
-
-    config = ConfigParser()
-    config.read(args.config)
-    # Get path for the work directory
-    if not os.path.exists(args.work_dir):
-        os.makedirs(args.work_dir)
-    abs_work_dir = os.path.abspath(args.work_dir)
-    accounting_group = config.get('core',
-                                  'accounting_group')
-    # changes made here
-    common_submit_dict = {
-            'universe': 'vanilla',
-            'request_disk': '1GB',
-            'output': '$(executable).stdout',
-            'error': '$(executable).stderr',
-            'log': '$(executable).log',
-            'accounting_group': accounting_group
-    }
-
-    condor_dag = dags.DAG()
-    join_layer, join_output_dict = _add_common_workflow(
-                                                condor_dag,
-                                                args,
-                                                common_submit_dict)
-    if not args.mass_gap:
-        _add_knn_workflow(join_layer, args,
-                          common_submit_dict,
-                          join_output_dict)
-    else:
-        _add_massgap_workflow(join_layer, args,
-                              common_submit_dict,
-                              join_output_dict)
-
-    print("DAG desription:\n", condor_dag.describe())
-    dags.write_dag(condor_dag, abs_work_dir,
-                   dag_file_name=args.dagname)
-
-    # FIXME Condor refuses to carry over env vars
-    # remove when solution is found
-    for exe in config['executables']:
-        src = os.path.join(args.executables_dir, exe)
-        dst = os.path.join(abs_work_dir, exe)
-        if os.path.lexists(dst):
-            os.remove(dst)
-        shutil.copy(src, dst)
-    print('{} is written in {}'.format(args.dagname, abs_work_dir))
-
-
-if __name__ == "__main__":
-    main()
+# Copyright(C) 2018-2022 Shaon Ghosh, Deep Chatterjee, Sushant Sharma Chaudhary
+#
+# This program is free software; you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation; either version 2 of the License, or (at your
+# option) any later version.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
+# Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+
+
+import os
+import re
+import shutil
+
+from argparse import ArgumentParser
+from configparser import ConfigParser
+from glob import glob
+
+from .data import EOS_BAYES_FACTORS
+
+try:
+    import htcondor
+    from htcondor import dags
+    _HTCONDOR_INSTALLED = True
+except ModuleNotFoundError:
+    _HTCONDOR_INSTALLED = False
+    import warnings
+    warnings.warn(
+        "HTCondor python bindings need to be installed to use this script. "
+        "This script is only used in training. When training new classifiers, "
+        "create a developmental version by cloning the git repository, "
+        "and installing from the lock file."
+    )
+
+
+def _add_common_workflow(condor_dag, args, common_submit_dict):
+    config = ConfigParser()
+    config.read(args.config)
+    config_path = os.path.abspath(args.config)
+    abs_work_dir = os.path.abspath(args.work_dir)
+    file_dir = args.file_dir
+    # Get injection directory
+    inj_file_pattern = config.get('core',
+                                  'inj_file_pattern')
+    sqlite_run_tag = config.get('core',
+                                'sqlite_run_tag')
+
+    # Get input and output file names prefixes
+    em_bright_extract_prefix = config.get('output_filenames',
+                                          'em_bright_extract_prefix')
+    em_bright_extract_suffix = config.get('output_filenames',
+                                          'em_bright_extract_suffix')
+    em_bright_join_prefix = config.get('output_filenames',
+                                       'em_bright_join_prefix')
+    em_bright_join_suffix = config.get('output_filenames',
+                                       'em_bright_join_suffix')
+    # Get executable names
+    em_bright_extract_executable = config.get('executables',
+                                              'em_bright_extract')
+    em_bright_join_executable = config.get('executables',
+                                           'em_bright_join')
+
+    # Define the executable arguments association
+    exec_arg_assoc = {
+        em_bright_extract_executable:
+            " --input $(macroinput) --output $(macrooutput)",
+        em_bright_join_executable:
+            " --input $(macroinput) --config $(macroconfig)"
+            " --output $(macrooutput)"
+    }
+    # create a dictionary of Submit instances
+    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
+    # create all sub files
+
+    for exect, arg_sub in exec_arg_assoc.items():
+        common_submit_dict["executable"] = exect
+        common_submit_dict["arguments"] = arg_sub
+        condor_sub_dict[exect] = htcondor.Submit(
+            common_submit_dict)
+    # Creating list of sqlite files to create the dag
+    inj_list = glob(
+        os.path.join(
+            os.path.abspath(file_dir), inj_file_pattern
+        )
+    )
+
+    # get vars for em_bright_extract layer
+    em_bright_extract_vars = []
+    for idx, injFilename in enumerate(inj_list):
+        match = re.search(sqlite_run_tag, os.path.basename(injFilename))
+        if match is None:
+            continue
+        prefix, startT, duration = match.groups()
+        # filename for INJCOINC files
+        output_fname = \
+            em_bright_extract_prefix + \
+            prefix + '-' + startT + '-' + duration + em_bright_extract_suffix
+        em_bright_extract_vars.append(
+            dict(
+                macroinput=injFilename,
+                macrooutput=output_fname
+            )
+        )
+    em_bright_extract_layer = condor_dag.layer(
+        name=em_bright_extract_executable,
+        submit_description=condor_sub_dict[em_bright_extract_executable],
+        vars=em_bright_extract_vars
+    )
+    # output for JOIN
+    join_output = \
+        em_bright_join_prefix + '-' + startT + '-' + \
+        duration + em_bright_join_suffix
+    join_output = os.path.join(abs_work_dir, join_output)
+
+    em_bright_join_vars = [
+        dict(
+            macroinput=abs_work_dir,
+            macrooutput=join_output,
+            macroconfig=config_path
+        )
+    ]
+    em_bright_join_layer = em_bright_extract_layer.child_layer(
+        name=em_bright_join_executable,
+        submit_description=condor_sub_dict[em_bright_join_executable],
+        vars=em_bright_join_vars
+    )
+    join_output_dict = {
+        "output": join_output,
+        "startT": startT,
+        "duration": duration
+    }
+    return em_bright_join_layer, join_output_dict
+
+
+def _add_knn_workflow(em_bright_join_layer, args,
+                      common_submit_dict,
+                      join_output_dict):
+    config = ConfigParser()
+    config.read(args.config)
+    config_path = os.path.abspath(args.config)
+    abs_work_dir = os.path.abspath(args.work_dir)
+
+    em_bright_categorize_prefix = config.get('output_filenames',
+                                             'em_bright_categorize_prefix')
+    em_bright_categorize_suffix = config.get('output_filenames',
+                                             'em_bright_categorize_suffix')
+    em_bright_train_prefix = config.get('output_filenames',
+                                        'em_bright_train_prefix')
+    em_bright_train_suffix = config.get('output_filenames',
+                                        'em_bright_train_suffix')
+    em_bright_categorize_executable = config.get('executables',
+                                                 'em_bright_categorize')
+    em_bright_train_executable = config.get('executables',
+                                            'em_bright_train')
+    em_bright_paramater_sweep_plot_executable = config.get(
+            'executables', 'em_bright_create_param_sweep_plot'
+    )
+    exec_arg_assoc = {
+        em_bright_train_executable:
+            " --input $(macroinput) --config $(macroconfig) "
+            "--output $(macrooutput) --param-sweep-plot-prefix $(macroeos)",
+        em_bright_paramater_sweep_plot_executable:
+            " --input $(macroinput) --config $(macroconfig)"
+            " --verbose",
+        em_bright_categorize_executable:
+            " --input $(macroinput) --output $(macrooutput)"
+            " --eosname $(macroeos) "
+    }
+    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
+
+    for exect, arg_sub in exec_arg_assoc.items():
+        common_submit_dict["executable"] = exect
+        common_submit_dict["arguments"] = arg_sub
+        condor_sub_dict[exect] = htcondor.Submit(
+            common_submit_dict)
+
+    # input and output for CATEGORIZE/TRAIN
+    em_bright_categorize_vars = list()
+    em_bright_train_vars = list()
+    categorize_input = join_output_dict["output"]
+
+    for em_bright_eos in EOS_BAYES_FACTORS:
+        categorize_output = \
+            em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
+            '-' + join_output_dict["duration"] + '-' + em_bright_eos + \
+            em_bright_categorize_suffix
+        categorize_output = os.path.join(abs_work_dir, categorize_output)
+
+        train_output = \
+            em_bright_train_prefix + '-' + join_output_dict["startT"] + \
+            '-' + join_output_dict["duration"] + \
+            '-' + em_bright_eos + em_bright_train_suffix
+        train_output = os.path.join(abs_work_dir, train_output)
+
+        em_bright_categorize_vars.append(
+            dict(
+                macroinput=categorize_input,
+                macrooutput=categorize_output,
+                macroeos=em_bright_eos,
+            )
+        )
+        em_bright_train_vars.append(
+                dict(
+                    macroinput=categorize_output,
+                    macrooutput=train_output,
+                    macroconfig=config_path,
+                    macroeos=em_bright_eos
+                )
+            )
+
+    em_bright_categorize_layer = em_bright_join_layer.child_layer(
+        name=em_bright_categorize_executable,
+        submit_description=condor_sub_dict[em_bright_categorize_executable],
+        vars=em_bright_categorize_vars
+    )
+
+    em_bright_train_layer = em_bright_categorize_layer.child_layer(
+            name=em_bright_train_executable,
+            submit_description=condor_sub_dict[em_bright_train_executable],
+            vars=em_bright_train_vars
+        )
+
+    em_bright_param_sweep_layer = em_bright_train_layer.child_layer(  # noqa: F841,E501
+            name=em_bright_paramater_sweep_plot_executable,
+            submit_description=condor_sub_dict[
+                em_bright_paramater_sweep_plot_executable],
+            vars=[
+                dict(
+                    macroinput=abs_work_dir,
+                    macroconfig=config_path
+                )
+            ]
+        )
+
+
+def _add_massgap_workflow(em_bright_join_layer, args,
+                          common_submit_dict,
+                          join_output_dict):
+    config = ConfigParser()
+    config.read(args.config)
+    config_path = os.path.abspath(args.config)
+    abs_work_dir = os.path.abspath(args.work_dir)
+
+    em_bright_categorize_prefix = config.get('output_filenames',
+                                             'em_bright_categorize_prefix')
+    em_bright_categorize_suffix = config.get('output_filenames',
+                                             'em_bright_categorize_suffix')
+    em_bright_train_suffix = config.get('output_filenames',
+                                        'em_bright_train_suffix')
+    em_bright_categorize_executable = config.get('executables',
+                                                 'em_bright_categorize')
+    em_bright_train_executable = config.get('executables',
+                                            'em_bright_train')
+    exec_arg_assoc = {
+        em_bright_categorize_executable:
+            " --input $(macroinput) --output $(macrooutput)"
+            " --mass-gap",
+        em_bright_train_executable:
+            " --input $(macroinput) --config $(macroconfig)"
+            " --output $(macrooutput) --mass-gap"
+    }
+    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
+    for exect, arg_sub in exec_arg_assoc.items():
+        common_submit_dict["executable"] = exect
+        common_submit_dict["arguments"] = arg_sub
+        condor_sub_dict[exect] = htcondor.Submit(
+            common_submit_dict)
+
+    categorize_input = join_output_dict["output"]
+    categorize_output = \
+        em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
+        '-' + join_output_dict["duration"] + \
+        em_bright_categorize_suffix
+    categorize_output = os.path.join(abs_work_dir, categorize_output)
+
+    em_bright_categorize_vars = [
+            dict(
+                macroinput=categorize_input,
+                macrooutput=categorize_output,
+            )
+    ]
+    em_bright_categorize_layer = em_bright_join_layer.child_layer(
+        name=em_bright_categorize_executable,
+        submit_description=condor_sub_dict[em_bright_categorize_executable],
+        vars=em_bright_categorize_vars
+    )
+
+    train_output = "mass_gap" + \
+        em_bright_train_suffix
+    train_output = os.path.join(abs_work_dir, train_output)
+
+    em_bright_train_vars = [
+         dict(
+                macroinput=categorize_output,
+                macrooutput=train_output,
+                macroconfig=config_path,
+            )
+    ]
+    em_bright_categorize_layer.child_layer(
+            name=em_bright_train_executable,
+            submit_description=condor_sub_dict[em_bright_train_executable],
+            vars=em_bright_train_vars
+        )
+
+
+def main():
+    parser = ArgumentParser("Condor DAG writer for workflow")
+    parser.add_argument("-d", "--dagname", required=True,
+                        help="Name of the dag file. Placed under --work-dir")
+    parser.add_argument("-w", "--work-dir", required=True,
+                        help="Working directory to store data outputs")
+    parser.add_argument(
+        "-i", "--file-dir", required=True,
+        help="File containing input injection sqlite databases"
+    )
+    parser.add_argument("-c", "--config", required=True,
+                        help="Name of the config file")
+    parser.add_argument("-e", "--executables-dir", required=True,
+                        help="Directory containing executables")
+    parser.add_argument("--mass-gap", action='store_true',
+                        help="use --random_forest for Random Forest Mode")
+    args = parser.parse_args()
+
+    assert _HTCONDOR_INSTALLED, "HTCondor python bindings missing."
+
+    config = ConfigParser()
+    config.read(args.config)
+    # Get path for the work directory
+    if not os.path.exists(args.work_dir):
+        os.makedirs(args.work_dir)
+    abs_work_dir = os.path.abspath(args.work_dir)
+    accounting_group = config.get('core',
+                                  'accounting_group')
+    # changes made here
+    common_submit_dict = {
+            'universe': 'vanilla',
+            'request_disk': '1GB',
+            'output': '$(executable).stdout',
+            'error': '$(executable).stderr',
+            'log': '$(executable).log',
+            'accounting_group': accounting_group
+    }
+
+    condor_dag = dags.DAG()
+    join_layer, join_output_dict = _add_common_workflow(
+                                                condor_dag,
+                                                args,
+                                                common_submit_dict)
+    if not args.mass_gap:
+        _add_knn_workflow(join_layer, args,
+                          common_submit_dict,
+                          join_output_dict)
+    else:
+        _add_massgap_workflow(join_layer, args,
+                              common_submit_dict,
+                              join_output_dict)
+
+    print("DAG desription:\n", condor_dag.describe())
+    dags.write_dag(condor_dag, abs_work_dir,
+                   dag_file_name=args.dagname)
+
+    # FIXME Condor refuses to carry over env vars
+    # remove when solution is found
+    for exe in config['executables']:
+        src = os.path.join(args.executables_dir, exe)
+        dst = os.path.join(abs_work_dir, exe)
+        if os.path.lexists(dst):
+            os.remove(dst)
+        shutil.copy(src, dst)
+    print('{} is written in {}'.format(args.dagname, abs_work_dir))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ligo_em_bright-1.1.4.post2/ligo/em_bright/tests/test_em_bright.py` & `ligo_em_bright-1.1.5/ligo/em_bright/tests/test_em_bright.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,92 +11,104 @@
 
 from .. import em_bright, categorize, utils
 from ..data import EOS_MAX_MASS
 
 
 def test_version():
     from .. import __version__
-    assert __version__ == '1.1.4.post2'
+    assert __version__ == '1.1.5'
 
 
 @pytest.mark.parametrize(
-    'posteriors, dtype, result, result_eos',
+    'posteriors, dtype, result_2H, result_SLy, result_eos',
     [[[(1.2, 1.0, 0.0, 0.0, 0.0, 0.0, 100.0),
        (2.0, 0.5, 0.99, 0.99, 0.0, 0.0, 150.0)],
       [('chirp_mass', '<f8'), ('mass_ratio', '<f8'), ('a_1', '<f8'),
        ('a_2', '<f8'), ('tilt_1', '<f8'), ('tilt_2', '<f8'),
        ('luminosity_distance', '<f8')],
-      (1.0, 1.0, 0.5), (1.0, 1.0, 0.5)],
+      (1.0, 1.0, 0.5), (1.0, 1.0, 0.5), (1.0, 1.0, 0.5)],
      [[(1.2, 1.0, 0.0, 0.0, 100.0),
        (2.0, 0.5, 0.99, 0.99, 150.0)],
       [('chirp_mass', '<f8'), ('mass_ratio', '<f8'), ('a_1', '<f8'),
        ('a_2', '<f8'), ('luminosity_distance', '<f8')],
-      (1.0, 1.0, 0.5), (1.0, 0.5, 0.5)],
+      (1.0, 1.0, 0.5), (1.0, 0.5, 0.5), (1.0, 0.529, 0.5)],
      [[(1.4, 1.4, 0.0, 0.0, 100.0),
        (2.0, 0.5, 0.99, 0.99, 150.0)],
       [('mass_1', '<f8'), ('mass_2', '<f8'), ('a_1', '<f8'),
        ('a_2', '<f8'), ('luminosity_distance', '<f8')],
-      (1.0, 1.0, 0.0), (1.0, 1.0, 0.0)],
+      (1.0, 1.0, 0.0), (1.0, 1.0, 0.0), (1.0, 1.0, 0.0)],
      [[(1.4, 1.4, 100.0),
        (2.0, 0.5, 150.0)],
       [('mass_1', '<f8'), ('mass_2', '<f8'), ('luminosity_distance', '<f8')],
-      (1.0, 1.0, 0.0), (1.0, 1.0, 0.0)],
+      (1.0, 1.0, 0.0), (1.0, 1.0, 0.0), (1.0, 1.0, 0.0)],
      [[(1.4, 1.4, 1.4, 1.4, 0.0, 0.0, 100.0),
        (2.0, 0.5, 2.0, 0.5, 0.99, 0.99, 150.0)],
       [('mass_1_source', '<f8'), ('mass_2_source', '<f8'),
        ('mass_1', '<f8'), ('mass_2', '<f8'), ('a_1', '<f8'),
        ('a_2', '<f8'), ('luminosity_distance', '<f8')],
-      (1.0, 1.0, 0.0), (1.0, 1.0, 0.0)],
+      (1.0, 1.0, 0.0), (1.0, 1.0, 0.0), (1.0, 0.99985, 0.0)],
      [[(4.5, -0.1, 200.0, 100000, 1.4, 1.4),
        (1.6, 0.3, 201.0, 100000, 1.5, 1.3)],
      [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
       ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8')],
-     (1.0, 1.0, 0.0), (1.0, 1.0, 0.0)],
+     (1.0, 1.0, 0.0), (1.0, 1.0, 0.0), (1.0, 1.0, 0.0)],
      [[(4.5, -0.1, 200.0, 100000, 4.5, 4.4),
        (1.6, 0.3, 201.0, 100000, 4.3, 4.2)],
      [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
       ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8')],
-     (0.0, 0.0, 1.0), (0.0, 0.0, 1.0)],
+     (0.0, 0.0, 1.0), (0.0, 0.0, 1.0), (0.0, 0.0, 1.0)],
      [[(4.5, -0.1, 200.0, 100000, 40.5, 4.4),
        (1.6, 0.3, 201.0, 100000, 40.3, 4.2)],
      [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
       ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8')],
-     (0.0, 0.0, 1.0), (0.0, 0.0, 1.0)],
+     (0.0, 0.0, 1.0), (0.0, 0.0, 1.0), (0.0, 0.0, 1.0)],
      [[(4.5, -0.1, 200.0, 1.0, 2.0, 2.0, 0.0, 0.0),
        (1.6, 0.3, 201.0, 1.0, 5.0, 2.0, 0.0, 0.0)],
      [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
       ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8'),
       ('spin_1z', '<f8'), ('spin_2z', '<f8')],
-     (1.0, 0.5, 0.5), (1.0, 0.5, 0.5)],
+     (1.0, 0.5, 0.5), (1.0, 0.5, 0.5), (1.0, 0.50045, 0.5)],
      [[(4.5, -0.1, 200.0, 1.0, 2.0, 2.0, 0.99, 0.0),
        (1.6, 0.3, 201.0, 1.0, 5.0, 2.0, 0.99, 0.0)],
      [('ra', '<f8'), ('dec', '<f8'), ('luminosity_distance', '<f8'),
       ('time', '<f8'), ('mass_1', '<f8'), ('mass_2', '<f8'),
       ('spin_1z', '<f8'), ('spin_2z', '<f8')],
-     (1.0, 1.0, 0.5), (1.0, 1.0, 0.5)]]
+     (1.0, 1.0, 0.5), (1.0, 1.0, 0.5), (1.0, 1.0, 0.5)],
+     [[(3.0, 2.8, 0.0, 0.0, 100.0)],
+     [('mass_1_source', '<f8'), ('mass_2_source', '<f8'),
+      ('a_1', '<f8'), ('a_2', '<f8'), ('luminosity_distance', '<f8')],
+      (1.0, 0.0, 1.0), (0.0, 0.0, 1.0), (0.0034, 0.0, 1.0)],
+     [[(2.5, 1.8, 0.0, 0.0, 100.0)],
+     [('mass_1_source', '<f8'), ('mass_2_source', '<f8'),
+      ('a_1', '<f8'), ('a_2', '<f8'), ('luminosity_distance', '<f8')],
+      (1.0, 1.0, 0.0), (1.0, 0.0, 0.0), (1.0, 0.0426, 0.0)]]
 )
-def test_source_classification_pe(posteriors, dtype, result, result_eos):
+def test_source_classification_pe(posteriors, dtype, result_2H,
+                                  result_SLy, result_eos):
     """Test em_bright classification from posterior
     samples - both aligned and precessing cases.
     """
     with NamedTemporaryFile() as f:
         filename = f.name
         with h5py.File(f, 'w') as tmp_h5:
             data = np.array(
                 posteriors,
                 dtype=dtype
             )
             tmp_h5.create_dataset(
                 'posterior_samples',
                 data=data
             )
-        r = em_bright.source_classification_pe(filename, eosname='2H')
-        r_eos = em_bright.source_classification_pe(filename, num_eos_draws=5,
+        r_2H = em_bright.source_classification_pe(filename, eosname='2H')
+        r_SLy = em_bright.source_classification_pe(filename, eosname='SLy')
+        r_eos = em_bright.source_classification_pe(filename,
+                                                   num_eos_draws=10000,
                                                    eos_seed=0)
-    assert r == result
+    assert r_2H == result_2H
+    assert r_SLy == result_SLy
     assert r_eos == result_eos
 
 
 @pytest.mark.parametrize(
     'posteriors, dtype, has_xxx_target',
     [
      [[(5.5, 1.5, 0.0, 0.0)],
```

### Comparing `ligo_em_bright-1.1.4.post2/ligo/em_bright/utils.py` & `ligo_em_bright-1.1.5/ligo/em_bright/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,663 +1,663 @@
-# Copyright (C) 2018-2021 Shaon Ghosh, Shasvath Kapadia, Deep Chatterjee
-# 2021-2022 Andrew Toivonen
-#
-# This program is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by the
-# Free Software Foundation; either version 2 of the License, or (at your
-# option) any later version.
-#
-# This program is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-
-
-import os
-import pickle
-import re
-
-import h5py
-from argparse import ArgumentParser
-from configparser import ConfigParser
-import glob
-import sqlite3
-
-import numpy as np
-import pandas as pd
-from astropy.table import Column, Table, vstack
-from sklearn.model_selection import KFold
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.ensemble import RandomForestClassifier
-
-from . import computeDiskMass
-from .data import PACKAGE_FILENAMES, EOS_BAYES_FACTORS, EOS_MAX_MASS
-
-
-def join():
-    """
-    Joins the extracted sim-coinc data from GstLAL injection
-    campaigns into a single Astropy table
-    """
-    parser = ArgumentParser(
-        "Join extracted GstLAL sim-coinc parameters as astropy table")
-    parser.add_argument("-i", "--input", required=True,
-                        help="Directory storing extracted sim-coinc files")
-    parser.add_argument("-c", "--config", required=True,
-                        help="Name of the config file")
-    parser.add_argument("-o", "--output", required=True,
-                        help="Name of the output file")
-    args = parser.parse_args()
-
-    config = ConfigParser()
-    config.read(args.config)
-    extract_prefix = config.get('output_filenames',
-                                'em_bright_extract_prefix')
-    extract_suffix = config.get('output_filenames',
-                                'em_bright_extract_suffix')
-    cols = config.get('core',
-                      'sqlite_cols')
-    list_of_files = glob.glob(
-        os.path.join(args.input, '{}*{}'.format(extract_prefix,
-                                                extract_suffix)))
-    cols = cols.split(',')
-    # FIXME delimited '|' is a fragile piece
-    data = vstack(
-        [Table.read(f, format='ascii', delimiter='|', names=cols)
-         for f in list_of_files]
-    )
-    # FIXME need a better implementation
-    # convert injected detector frame mass to source frame masses
-    inj_mass1_source = Column(data['inj_m1']/(1.0 + data['inj_redshift']),
-                              name='inj_mass1_source_frame')
-    inj_mass2_source = Column(data['inj_m2']/(1.0 + data['inj_redshift']),
-                              name='inj_mass2_source_frame')
-    ID = Column(np.arange(len(data)), name='id')
-    data.add_column(ID, index=0)
-    data.add_column(inj_mass1_source, index=0)
-    data.add_column(inj_mass2_source, index=0)
-
-    data.write(args.output, format='ascii', delimiter='\t')
-
-
-def extract():
-    """
-    Ingests a GstLAL injection campaign sqlite database and
-    outputs the list of coinc parameters in a flat file
-    """
-    parser = ArgumentParser(
-        "Get sim-coinc maps for LIGO GstLAL injection sqlite database")
-    parser.add_argument("-i", "--input", required=True,
-                        help="sqlite database")
-    parser.add_argument("-o", "--output", required=True,
-                        help="Output file, stored as numpy array")
-    args = parser.parse_args()
-
-    cur = sqlite3.connect(args.input).cursor()
-    cur.execute(
-        """
-        CREATE TEMPORARY TABLE
-        sim_coinc_map_helper
-        AS
-        SELECT a.event_id as sid,
-        coinc_event.coinc_event_id as cid,
-        coinc_event.likelihood as lr
-        FROM coinc_event_map as a
-        JOIN coinc_event_map AS b ON (b.coinc_event_id == a.coinc_event_id)
-        JOIN coinc_event ON (coinc_event.coinc_event_id == b.event_id)
-        WHERE a.table_name == 'sim_inspiral'
-        AND b.table_name == 'coinc_event'
-        AND NOT EXISTS (
-            SELECT * FROM time_slide WHERE
-            time_slide.time_slide_id == coinc_event.time_slide_id
-            AND time_slide.offset != 0
-        )"""
-    )
-
-    cur.execute(
-        """
-        CREATE INDEX IF NOT EXISTS
-        sim_coinc_map_helper_index ON sim_coinc_map_helper (sid, cid)
-        """
-    )
-
-    cur.execute(
-        """
-        CREATE TEMPORARY TABLE
-            sim_coinc_map
-        AS
-            SELECT
-                sim_inspiral.simulation_id AS simulation_id,
-                (
-                    SELECT cid FROM
-                                sim_coinc_map_helper
-                    WHERE sid = simulation_id
-                    ORDER BY lr DESC
-                    LIMIT 1
-                ) AS coinc_event_id
-            FROM sim_inspiral
-            WHERE coinc_event_id IS NOT NULL
-        """
-    )
-
-    cur.execute("""DROP INDEX sim_coinc_map_helper_index""")
-
-    query = """
-    SELECT
-    sim_inspiral.mass1,
-    sim_inspiral.mass2,
-    sim_inspiral.spin1z,
-    sim_inspiral.spin2z,
-        sim_inspiral.alpha3,
-    sngl_inspiral.mass1,
-    sngl_inspiral.mass2,
-    sngl_inspiral.spin1z,
-    sngl_inspiral.spin2z,
-    sngl_inspiral.Gamma1,
-    coinc_inspiral.combined_far,
-    coinc_inspiral.snr,
-    coinc_inspiral.end_time
-    FROM
-    sim_coinc_map
-    JOIN
-    sim_inspiral
-    ON
-    sim_coinc_map.simulation_id==sim_inspiral.simulation_id
-    JOIN
-    coinc_event_map
-    ON
-    sim_coinc_map.coinc_event_id == coinc_event_map.coinc_event_id
-    JOIN
-    coinc_inspiral
-    ON
-    sim_coinc_map.coinc_event_id == coinc_inspiral.coinc_event_id
-    JOIN
-    sngl_inspiral
-    ON (
-        coinc_event_map.table_name == 'sngl_inspiral'
-        AND coinc_event_map.event_id == sngl_inspiral.event_id
-    )
-    WHERE
-    sngl_inspiral.ifo=='H1';
-    """
-    np.savetxt(args.output, np.array(cur.execute(query).fetchall()),
-               fmt='%f|%f|%f|%f|%f|%f|%f|%f|%f|%d|%e|%f|%f')
-
-
-def train():
-    parser = ArgumentParser(
-        description='Executable to train source classifier from injections')
-
-    parser.add_argument(
-        '-i', '--input',
-        help='Pickled dataframe containing source categorized data')
-    parser.add_argument(
-        '-o', '--output',
-        help='Pickled object storing the trained classifiers')
-    parser.add_argument(
-        '-d', '--param-sweep-plot-prefix', default=None,
-        help='Supply filename prefix to output a parameter sweep plot')
-    parser.add_argument(
-        '-c', '--config', required=True,
-        help='Config file with additional parameters')
-    parser.add_argument("--mass-gap", required=False, action="store_true",
-                        help="mode of categorization")
-
-    args = parser.parse_args()
-    if args.mass_gap:
-        settings = 'massgap'
-    else:
-        settings = 'em_bright'
-    config = ConfigParser()
-    config.read(args.config)
-    # compulsory sections in config
-    required_sections = ['core',
-                         'em_bright']
-    assert all(config.has_section(s) for s in required_sections), \
-        'Config file must have sections %s' % (required_sections,)
-
-    # get column names and values from config
-    feature_cols = config.get(settings,
-                              'feature_cols').split(',')
-    category_cols = config.get(settings,
-                               'category_cols').split(',')
-    threshold_cols = config.get(settings,
-                                'threshold_cols').split(',')
-    all_cols = feature_cols + category_cols + threshold_cols
-
-    threshold_values = map(
-        eval, config.get(
-            settings,
-            'threshold_values').split(',')
-        )
-    threshold_type = config.get(settings,
-                                'threshold_type').split(',')
-    # read dataframe, check sanity
-    with open(args.input, 'rb') as f:
-        df = pickle.load(f)
-
-    assert all(col in df.keys() for col in all_cols), \
-        'Dataframe must contain columns %s' % (all_cols,)
-
-    # create masked array based on threshold values,
-    # extract features and targets
-    mask = np.ones(len(df)).astype(bool)
-    for col, value, typ in zip(threshold_cols, threshold_values,
-                               threshold_type):
-        mask &= df[col] < value if typ == 'lesser' else \
-            df[col] > value if typ == 'greater' else True
-
-    features = df[feature_cols][mask]
-    targets = df[category_cols][mask]
-
-    if not args.mass_gap:
-        clf_kwargs = eval(config.get('em_bright',
-                                     'clf_kwargs'))
-        if clf_kwargs.get('metric') == 'mahalanobis':
-            clf_kwargs['metric_params'] = dict(
-                V=features.cov().values
-            )  # covariance matrix needed for mahalanobis metric
-        clfs = []
-        for category, target_value in targets.iteritems():
-            # run KFold cross-validation
-            res_predict, res_predict_proba = run_k_fold_split(
-                features, target_value,
-                training_task=run_KNN_classifier,
-                **clf_kwargs)
-            test_results = pd.DataFrame(
-                np.vstack((features.T, target_value,
-                           res_predict, res_predict_proba)).T,
-                columns=feature_cols + ['targets', 'predict', 'predict_proba']
-            )
-            test_results_filename = 'cross-val-res-' + category + '.csv'
-            test_results.to_csv(test_results_filename, index=False)
-            # train on the full dataset
-            clf = KNeighborsClassifier(**clf_kwargs)
-            clf.fit(features.values, target_value)
-            if args.param_sweep_plot_prefix:
-                _create_param_sweep_plot(
-                    clf, category,
-                    args.param_sweep_plot_prefix
-                )
-            clfs.append(clf)
-        # append the output filename of the classifier
-        clfs.extend([args.output])
-        with open(args.output, 'wb') as f:
-            pickle.dump(clfs, f)
-    else:
-        # train random forest classifier for massgap category
-        clf_kwargs = eval(config.get('massgap',
-                                     'clf_kwargs'))
-        res_predict, res_predict_proba = run_k_fold_split(
-            features, targets,
-            training_task=run_RF_classifier, **clf_kwargs
-        )
-        test_results = pd.DataFrame(
-            np.vstack((features.T, targets.squeeze().T,
-                       res_predict, res_predict_proba)).T,
-            columns=feature_cols + ['targets', 'predict', 'predict_proba']
-        )
-        test_results_filename = 'cross-val-res-' + 'mass-gap' + '.csv'
-        test_results.to_csv(test_results_filename, index=False)
-        clf = RandomForestClassifier(**clf_kwargs)
-        clf.fit(features.values, targets.squeeze())
-        _create_param_sweep_plot(
-            clf, 'mass_gap',
-            prefix='SLy'  # FIXME: ad-hoc prefix needed, not used for plotting
-        )
-        with open(args.output, 'wb') as f:
-            # append the filename of the classfier
-            pickle.dump([clf, args.output], f)
-
-
-def _open_and_return_clfs(filename):
-    """Unpack pickle files storing classifier and return.
-    If two classifiers exist, assume first argument is HasNS,
-    second HasRemnant. If single classifier exists, then assume
-    mass_gap classifier.
-    """
-    with open(filename, 'rb') as f:
-        content = pickle.load(f)
-        try:
-            clf_ns, clf_em, _filename = content
-            return clf_ns, clf_em
-        except ValueError:
-            clf_mass_gap, _filename = content
-            return clf_mass_gap
-
-
-def _get_mass_grid():
-    """Get a grid over mass1, mass2. Used for parameter sweep."""
-    mass1 = np.linspace(1, 20, 200)
-    mass2 = np.linspace(1, 20, 200)
-    t = Table(
-        data=np.vstack(
-            (np.repeat(mass1, mass2.size),
-             np.tile(mass2, mass1.size))
-        ).T, names=('mass1', 'mass2')
-    )
-    mask = t['mass1'] > t['mass2']
-    t = t[mask]
-    return t
-
-
-def _get_param_sweep(clf):
-    """Create a fake recovered parameter space return
-    the predictions for the classifier sweeping across
-    masses.
-    """
-    if hasattr(clf, 'metric') and clf.metric == "mahalanobis":
-        clf.n_jobs = 1  # issue with BallTree output
-    t = _get_mass_grid()
-    spins = Table(
-        data=np.vstack(
-            (np.repeat(np.linspace(0, 1, 2), 2),
-             np.tile(np.linspace(0, 1, 2), 2))
-        ).T,
-        names=('chi1', 'chi2')
-    )
-    SNR = 10.
-    res = list()
-    for spin_vals in spins:
-        SNR *= np.ones(len(t))
-        chi1 = spin_vals['chi1'] * np.ones(len(t))
-        chi2 = spin_vals['chi2'] * np.ones(len(t))
-        # make predictions and make plots
-        param_sweep_features = np.stack(
-            [t['mass1'], t['mass2'], chi1, chi2, SNR]
-        ).T
-        predictions = clf.predict_proba(param_sweep_features).T[1]
-        res.append((param_sweep_features, predictions))
-    return res
-
-
-def _create_param_sweep_plot(clf, category, prefix=None):
-    """Create a parameter sweep plot using the supplied classifer"""
-    import matplotlib.pyplot as plt
-    res = _get_param_sweep(clf)
-    fig = plt.figure(figsize=(14, 20))
-    for idx, r in enumerate(res):
-        features, predictions = r
-        # FIXME: Ugly, but works
-        title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
-            features[0][2], features[0][3],
-            features[0][4]
-        )
-        make_plots(
-            features, predictions, title,
-            (fig, idx+1), prefix=prefix, category=category
-        )
-    try:
-        plt.savefig(prefix+'_param_sweep_'+category+'.png')
-    except TypeError:
-        plt.savefig('param_sweep_'+category+'.png')
-
-
-def load_eos_posterior():
-    '''
-    Loads eos posterior draws (https://zenodo.org/record/6502467#.Yoa2EKjMI2z)
-
-    Returns
-    -------
-    draws: np.array
-        equally weighted eos draws from file
-    '''
-    eos_file = PACKAGE_FILENAMES['EOS_POSTERIOR_DRAWS.h5']
-    with h5py.File(eos_file, 'r') as f:
-        draws = np.array(f['EOS'])
-    return draws
-
-
-def param_sweep_plot():
-    """Create parameter sweep plot, weighting classifier
-    results using bayes factor
-    """
-    parser = ArgumentParser(
-        "Create a parameter sweep, EoS predictions based")
-    parser.add_argument("-i", "--input", required=True,
-                        help="Directory storing trained classifier files")
-    parser.add_argument("-c", "--config", required=True,
-                        help="Config file")
-    parser.add_argument("-v", "--verbose", action='store_true',
-                        help="show progress")
-    args = parser.parse_args()
-
-    config = ConfigParser()
-    config.read(args.config)
-
-    train_prefix = config.get('output_filenames', 'em_bright_train_prefix')
-    train_suffix = config.get('output_filenames', 'em_bright_train_suffix')
-    clf_filenames = glob.glob(
-        os.path.join(args.input, f'{train_prefix}*{train_suffix}'))
-    if args.verbose:
-        print("Trained classifers", clf_filenames)
-    assert clf_filenames, "No files found. Check directory."
-    reweight_ns = dict.fromkeys(EOS_BAYES_FACTORS)
-    reweight_em = dict.fromkeys(EOS_BAYES_FACTORS)
-    import matplotlib.pyplot as plt
-    for fname in clf_filenames:
-        if args.verbose:
-            print(fname)
-        clf_ns, clf_em = _open_and_return_clfs(fname)
-        eosname, *_ = filter(
-            lambda _: re.match(
-                ".*" + _ + config.get('output_filenames',
-                                      'em_bright_train_suffix'),
-                fname
-            ), EOS_BAYES_FACTORS
-        )
-        res_ns = _get_param_sweep(clf_ns)
-        res_em = _get_param_sweep(clf_em)
-        reweight_ns.update(
-            {
-                eosname: dict(
-                    features=np.array(
-                        [f for f, p in res_ns]
-                    ),
-                    predictions=np.array(
-                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_ns]
-                    )
-                )
-            }
-        )
-        reweight_em.update(
-            {
-                eosname: dict(
-                    features=np.array(
-                        [f for f, p in res_em]
-                    ),
-                    predictions=np.array(
-                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_em]
-                    )
-                )
-            }
-        )
-    assert all(reweight_ns.values()), "Missing some listed EOSs."
-    assert all(reweight_em.values()), "Missing some listed EOSs."
-    reweighted_score_ns = np.sum(
-        [v['predictions'] for v in reweight_ns.values()],
-        axis=0
-    )
-    reweighted_score_em = np.sum(
-        [v['predictions'] for v in reweight_em.values()],
-        axis=0
-    )
-    for category, score in zip(
-            ["NS", "EMB"], [reweighted_score_ns, reweighted_score_em]):
-        fig = plt.figure(figsize=(14, 20))
-        for idx, (f, p) in enumerate(
-                zip(reweight_ns['SLy']['features'], score)):
-            title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
-                f[0][2], f[0][3], f[0][4])
-            make_plots(
-                f, p, title, (fig, idx+1),
-                prefix='SLy', category=category
-            )
-        plt.savefig("reweighted_" + category + "_param_sweep.png")
-
-
-def make_plots(features, predictions, title, fig_idx,
-               prefix=None, category=None):
-    import matplotlib.pyplot as plt
-    fig_, idx = fig_idx
-    fig_.add_subplot(4, 1, idx)
-    # indices 0 and 1 correspond to mass1 and mass2 respectively
-    plt.scatter(features.T[0], features.T[1],
-                s=10, c=predictions)
-    plt.title(title)
-    plt.tight_layout()
-    plt.colorbar(label='Probability')
-    # plot chirp mass contours
-    m1 = np.linspace(1, 20, 1000)
-    m2 = np.linspace(1, 20, 1000)
-    M1, M2 = np.meshgrid(m1, m2)
-    s1z = np.unique(features.T[2])[0]*np.ones(M1.shape)
-    s2z = np.unique(features.T[3])[0]*np.ones(M2.shape)
-    rem_masses = list()
-    for _ in range(M1.shape[0]):
-        rem_masses.append(
-            computeDiskMass.computeDiskMass(
-                M1[_], M2[_], s1z[_], s2z[_],
-                eosname=prefix
-            )
-        )
-    rem_masses = np.array(rem_masses).reshape(M1.shape)
-    Mc = (M1*M2)**(3./5.)/(M1 + M2)**(1./5.)
-    mask = M1 > M2
-    M1 = np.ma.masked_array(M1, mask=mask)
-    M2 = np.ma.masked_array(M2, mask=mask)
-    s1z = np.ma.masked_array(s1z, mask=mask)
-    s2z = np.ma.masked_array(s2z, mask=mask)
-    Mc = np.ma.masked_array(Mc, mask=mask)
-    rem_masses = np.ma.masked_array(
-        rem_masses, mask=mask*(M2 > EOS_MAX_MASS[prefix])
-    )
-    CS = plt.contour(
-        M1, M2, Mc.T, levels=[2.01, 2.22, 2.99, 3.48, 4.73, 5.4],
-        # (m1, m2) = (4, 1.4) -> Mc = 2.01
-        # (m1, m2) = (5, 1.4) -> Mc = 2.22
-        # (m1, m2) = (10, 1.4) -> Mc = 2.99
-        # (m1, m2) = (4, 4)    -> Mc = 3.48
-        # (m1, m2) = (30, 1.4) -> Mc = 4.73
-        # (m1, m2) = (10, 4)  -> Mc = 5.4
-        # three different NSBH populations;
-        # three different mass-gap populations
-        colors='black', linewidths=1.0
-    )
-    plt.clabel(CS, inline=True, fontsize=16)
-    plt.xlim((1, 20))
-    plt.ylim((1, 12))
-    try:
-        max_mass = EOS_MAX_MASS[prefix]
-    except KeyError:
-        max_mass = 3.0
-    if 'NS' in category:
-        plt.axhline(y=max_mass, c='r', linewidth=1.2)
-    elif 'EM' in category:
-        CS = plt.contour(M1, M2, rem_masses.T,
-                         levels=[0., ], colors='red',
-                         linewidths=1.2)
-    plt.xlabel(r'$m_1$', fontsize=16)
-    plt.ylabel(r'$m_2$', fontsize=16)
-
-
-def run_k_fold_split(features, targets, n_splits=10, random_state=0,
-                     training_task=None, **kwargs):
-    """Split the `features` in `n_splits`, train on `n_splits - 1`
-    sets, test on the last fraction. This performed across the complete
-    dataset.
-
-    Parameters
-    ----------
-    features : numpy.ndarray
-        Feature set
-    targets : numpy.ndarray
-        Target set containing binary classification of `features`
-    n_splits : int
-        Number of splits for `features` and `targets`
-    random_state : int
-        Random seed for the split
-    training_task : callable
-        function with arguments (X_train, y_train, X_test, **kwargs) which
-        trains, and returns predictions on X_test.
-        E.g. :meth:`run_KNN_classifier`,
-        or :meth:`run_RF_classifier`.
-    **kwargs
-        Keyword arguments passed to `training_task`.
-
-    Returns
-    -------
-    tuple
-        (res_predict, res_predict_proba) - predictions and probabilities
-    """
-    res_predict_proba = np.empty(len(features))
-    res_predict = np.empty(len(features))
-    res_predict_proba[:] = np.nan
-    res_predict[:] = np.nan
-
-    sss = KFold(n_splits=n_splits, shuffle=True, random_state=random_state)
-    sss.get_n_splits(features, targets)
-    for train_index, test_index in sss.split(features, targets):
-        X_train, X_test, y_train = \
-            features.iloc[train_index], \
-            features.iloc[test_index], \
-            targets.iloc[train_index]
-
-        predict_proba, predict = training_task(X_train, y_train, X_test,
-                                               **kwargs)
-        # second column is the prob of NS/EMB
-        predict_proba = predict_proba.T[1]
-
-        res_predict_proba[test_index] = predict_proba
-        res_predict[test_index] = predict
-    return res_predict, res_predict_proba
-
-
-def run_KNN_classifier(X_train, y_train,
-                       X_test,
-                       **kwargs):
-    '''
-    Run KNearestNeighborClassifier classifier returns
-    `clf.predict_proba`
-
-    Parameters
-    ----------
-    X_train : numpy.ndarray
-        Feature training set, can be array or Dataframe
-    y_train : numpy.array
-        Target training set, 0 or 1 binary classification
-    X_test : numpy.ndarray
-        Feature testing set, can be array or DataFrame
-    '''
-    if kwargs.get('metric') == 'mahalanobis':
-        kwargs['n_jobs'] = 1  # issue with KDTree, BallTree with n_jobs > 1
-    clf = KNeighborsClassifier(**kwargs)
-    clf.fit(X_train.values, y_train)
-    predictions_proba = clf.predict_proba(X_test)
-    predict = clf.predict(X_test)
-    return predictions_proba, predict
-
-
-def run_RF_classifier(X_train, y_train, X_test,
-                      **kwargs):
-    '''
-    Run RandomForestClassifier; returns
-    `clf.predict_proba`
-
-    Parameters
-    ----------
-    X_train : numpy.ndarray
-        Feature training set, can be array or Dataframe
-    y_train : numpy.array
-        Target training set, 0 or 1 binary classification
-    X_test : numpy.ndarray
-        Feature testing set, can be array or DataFrame
-    '''
-    clf = RandomForestClassifier(**kwargs)
-    clf.fit(X_train.values, y_train)
-    predictions_proba = clf.predict_proba(X_test)
-    predict = clf.predict(X_test)
-    return predictions_proba, predict
+# Copyright (C) 2018-2021 Shaon Ghosh, Shasvath Kapadia, Deep Chatterjee
+# 2021-2022 Andrew Toivonen
+#
+# This program is free software; you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation; either version 2 of the License, or (at your
+# option) any later version.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
+# Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+
+
+import os
+import pickle
+import re
+
+import h5py
+from argparse import ArgumentParser
+from configparser import ConfigParser
+import glob
+import sqlite3
+
+import numpy as np
+import pandas as pd
+from astropy.table import Column, Table, vstack
+from sklearn.model_selection import KFold
+from sklearn.neighbors import KNeighborsClassifier
+from sklearn.ensemble import RandomForestClassifier
+
+from . import computeDiskMass
+from .data import PACKAGE_FILENAMES, EOS_BAYES_FACTORS, EOS_MAX_MASS
+
+
+def join():
+    """
+    Joins the extracted sim-coinc data from GstLAL injection
+    campaigns into a single Astropy table
+    """
+    parser = ArgumentParser(
+        "Join extracted GstLAL sim-coinc parameters as astropy table")
+    parser.add_argument("-i", "--input", required=True,
+                        help="Directory storing extracted sim-coinc files")
+    parser.add_argument("-c", "--config", required=True,
+                        help="Name of the config file")
+    parser.add_argument("-o", "--output", required=True,
+                        help="Name of the output file")
+    args = parser.parse_args()
+
+    config = ConfigParser()
+    config.read(args.config)
+    extract_prefix = config.get('output_filenames',
+                                'em_bright_extract_prefix')
+    extract_suffix = config.get('output_filenames',
+                                'em_bright_extract_suffix')
+    cols = config.get('core',
+                      'sqlite_cols')
+    list_of_files = glob.glob(
+        os.path.join(args.input, '{}*{}'.format(extract_prefix,
+                                                extract_suffix)))
+    cols = cols.split(',')
+    # FIXME delimited '|' is a fragile piece
+    data = vstack(
+        [Table.read(f, format='ascii', delimiter='|', names=cols)
+         for f in list_of_files]
+    )
+    # FIXME need a better implementation
+    # convert injected detector frame mass to source frame masses
+    inj_mass1_source = Column(data['inj_m1']/(1.0 + data['inj_redshift']),
+                              name='inj_mass1_source_frame')
+    inj_mass2_source = Column(data['inj_m2']/(1.0 + data['inj_redshift']),
+                              name='inj_mass2_source_frame')
+    ID = Column(np.arange(len(data)), name='id')
+    data.add_column(ID, index=0)
+    data.add_column(inj_mass1_source, index=0)
+    data.add_column(inj_mass2_source, index=0)
+
+    data.write(args.output, format='ascii', delimiter='\t')
+
+
+def extract():
+    """
+    Ingests a GstLAL injection campaign sqlite database and
+    outputs the list of coinc parameters in a flat file
+    """
+    parser = ArgumentParser(
+        "Get sim-coinc maps for LIGO GstLAL injection sqlite database")
+    parser.add_argument("-i", "--input", required=True,
+                        help="sqlite database")
+    parser.add_argument("-o", "--output", required=True,
+                        help="Output file, stored as numpy array")
+    args = parser.parse_args()
+
+    cur = sqlite3.connect(args.input).cursor()
+    cur.execute(
+        """
+        CREATE TEMPORARY TABLE
+        sim_coinc_map_helper
+        AS
+        SELECT a.event_id as sid,
+        coinc_event.coinc_event_id as cid,
+        coinc_event.likelihood as lr
+        FROM coinc_event_map as a
+        JOIN coinc_event_map AS b ON (b.coinc_event_id == a.coinc_event_id)
+        JOIN coinc_event ON (coinc_event.coinc_event_id == b.event_id)
+        WHERE a.table_name == 'sim_inspiral'
+        AND b.table_name == 'coinc_event'
+        AND NOT EXISTS (
+            SELECT * FROM time_slide WHERE
+            time_slide.time_slide_id == coinc_event.time_slide_id
+            AND time_slide.offset != 0
+        )"""
+    )
+
+    cur.execute(
+        """
+        CREATE INDEX IF NOT EXISTS
+        sim_coinc_map_helper_index ON sim_coinc_map_helper (sid, cid)
+        """
+    )
+
+    cur.execute(
+        """
+        CREATE TEMPORARY TABLE
+            sim_coinc_map
+        AS
+            SELECT
+                sim_inspiral.simulation_id AS simulation_id,
+                (
+                    SELECT cid FROM
+                                sim_coinc_map_helper
+                    WHERE sid = simulation_id
+                    ORDER BY lr DESC
+                    LIMIT 1
+                ) AS coinc_event_id
+            FROM sim_inspiral
+            WHERE coinc_event_id IS NOT NULL
+        """
+    )
+
+    cur.execute("""DROP INDEX sim_coinc_map_helper_index""")
+
+    query = """
+    SELECT
+    sim_inspiral.mass1,
+    sim_inspiral.mass2,
+    sim_inspiral.spin1z,
+    sim_inspiral.spin2z,
+        sim_inspiral.alpha3,
+    sngl_inspiral.mass1,
+    sngl_inspiral.mass2,
+    sngl_inspiral.spin1z,
+    sngl_inspiral.spin2z,
+    sngl_inspiral.Gamma1,
+    coinc_inspiral.combined_far,
+    coinc_inspiral.snr,
+    coinc_inspiral.end_time
+    FROM
+    sim_coinc_map
+    JOIN
+    sim_inspiral
+    ON
+    sim_coinc_map.simulation_id==sim_inspiral.simulation_id
+    JOIN
+    coinc_event_map
+    ON
+    sim_coinc_map.coinc_event_id == coinc_event_map.coinc_event_id
+    JOIN
+    coinc_inspiral
+    ON
+    sim_coinc_map.coinc_event_id == coinc_inspiral.coinc_event_id
+    JOIN
+    sngl_inspiral
+    ON (
+        coinc_event_map.table_name == 'sngl_inspiral'
+        AND coinc_event_map.event_id == sngl_inspiral.event_id
+    )
+    WHERE
+    sngl_inspiral.ifo=='H1';
+    """
+    np.savetxt(args.output, np.array(cur.execute(query).fetchall()),
+               fmt='%f|%f|%f|%f|%f|%f|%f|%f|%f|%d|%e|%f|%f')
+
+
+def train():
+    parser = ArgumentParser(
+        description='Executable to train source classifier from injections')
+
+    parser.add_argument(
+        '-i', '--input',
+        help='Pickled dataframe containing source categorized data')
+    parser.add_argument(
+        '-o', '--output',
+        help='Pickled object storing the trained classifiers')
+    parser.add_argument(
+        '-d', '--param-sweep-plot-prefix', default=None,
+        help='Supply filename prefix to output a parameter sweep plot')
+    parser.add_argument(
+        '-c', '--config', required=True,
+        help='Config file with additional parameters')
+    parser.add_argument("--mass-gap", required=False, action="store_true",
+                        help="mode of categorization")
+
+    args = parser.parse_args()
+    if args.mass_gap:
+        settings = 'massgap'
+    else:
+        settings = 'em_bright'
+    config = ConfigParser()
+    config.read(args.config)
+    # compulsory sections in config
+    required_sections = ['core',
+                         'em_bright']
+    assert all(config.has_section(s) for s in required_sections), \
+        'Config file must have sections %s' % (required_sections,)
+
+    # get column names and values from config
+    feature_cols = config.get(settings,
+                              'feature_cols').split(',')
+    category_cols = config.get(settings,
+                               'category_cols').split(',')
+    threshold_cols = config.get(settings,
+                                'threshold_cols').split(',')
+    all_cols = feature_cols + category_cols + threshold_cols
+
+    threshold_values = map(
+        eval, config.get(
+            settings,
+            'threshold_values').split(',')
+        )
+    threshold_type = config.get(settings,
+                                'threshold_type').split(',')
+    # read dataframe, check sanity
+    with open(args.input, 'rb') as f:
+        df = pickle.load(f)
+
+    assert all(col in df.keys() for col in all_cols), \
+        'Dataframe must contain columns %s' % (all_cols,)
+
+    # create masked array based on threshold values,
+    # extract features and targets
+    mask = np.ones(len(df)).astype(bool)
+    for col, value, typ in zip(threshold_cols, threshold_values,
+                               threshold_type):
+        mask &= df[col] < value if typ == 'lesser' else \
+            df[col] > value if typ == 'greater' else True
+
+    features = df[feature_cols][mask]
+    targets = df[category_cols][mask]
+
+    if not args.mass_gap:
+        clf_kwargs = eval(config.get('em_bright',
+                                     'clf_kwargs'))
+        if clf_kwargs.get('metric') == 'mahalanobis':
+            clf_kwargs['metric_params'] = dict(
+                V=features.cov().values
+            )  # covariance matrix needed for mahalanobis metric
+        clfs = []
+        for category, target_value in targets.iteritems():
+            # run KFold cross-validation
+            res_predict, res_predict_proba = run_k_fold_split(
+                features, target_value,
+                training_task=run_KNN_classifier,
+                **clf_kwargs)
+            test_results = pd.DataFrame(
+                np.vstack((features.T, target_value,
+                           res_predict, res_predict_proba)).T,
+                columns=feature_cols + ['targets', 'predict', 'predict_proba']
+            )
+            test_results_filename = 'cross-val-res-' + category + '.csv'
+            test_results.to_csv(test_results_filename, index=False)
+            # train on the full dataset
+            clf = KNeighborsClassifier(**clf_kwargs)
+            clf.fit(features.values, target_value)
+            if args.param_sweep_plot_prefix:
+                _create_param_sweep_plot(
+                    clf, category,
+                    args.param_sweep_plot_prefix
+                )
+            clfs.append(clf)
+        # append the output filename of the classifier
+        clfs.extend([args.output])
+        with open(args.output, 'wb') as f:
+            pickle.dump(clfs, f)
+    else:
+        # train random forest classifier for massgap category
+        clf_kwargs = eval(config.get('massgap',
+                                     'clf_kwargs'))
+        res_predict, res_predict_proba = run_k_fold_split(
+            features, targets,
+            training_task=run_RF_classifier, **clf_kwargs
+        )
+        test_results = pd.DataFrame(
+            np.vstack((features.T, targets.squeeze().T,
+                       res_predict, res_predict_proba)).T,
+            columns=feature_cols + ['targets', 'predict', 'predict_proba']
+        )
+        test_results_filename = 'cross-val-res-' + 'mass-gap' + '.csv'
+        test_results.to_csv(test_results_filename, index=False)
+        clf = RandomForestClassifier(**clf_kwargs)
+        clf.fit(features.values, targets.squeeze())
+        _create_param_sweep_plot(
+            clf, 'mass_gap',
+            prefix='SLy'  # FIXME: ad-hoc prefix needed, not used for plotting
+        )
+        with open(args.output, 'wb') as f:
+            # append the filename of the classfier
+            pickle.dump([clf, args.output], f)
+
+
+def _open_and_return_clfs(filename):
+    """Unpack pickle files storing classifier and return.
+    If two classifiers exist, assume first argument is HasNS,
+    second HasRemnant. If single classifier exists, then assume
+    mass_gap classifier.
+    """
+    with open(filename, 'rb') as f:
+        content = pickle.load(f)
+        try:
+            clf_ns, clf_em, _filename = content
+            return clf_ns, clf_em
+        except ValueError:
+            clf_mass_gap, _filename = content
+            return clf_mass_gap
+
+
+def _get_mass_grid():
+    """Get a grid over mass1, mass2. Used for parameter sweep."""
+    mass1 = np.linspace(1, 20, 200)
+    mass2 = np.linspace(1, 20, 200)
+    t = Table(
+        data=np.vstack(
+            (np.repeat(mass1, mass2.size),
+             np.tile(mass2, mass1.size))
+        ).T, names=('mass1', 'mass2')
+    )
+    mask = t['mass1'] > t['mass2']
+    t = t[mask]
+    return t
+
+
+def _get_param_sweep(clf):
+    """Create a fake recovered parameter space return
+    the predictions for the classifier sweeping across
+    masses.
+    """
+    if hasattr(clf, 'metric') and clf.metric == "mahalanobis":
+        clf.n_jobs = 1  # issue with BallTree output
+    t = _get_mass_grid()
+    spins = Table(
+        data=np.vstack(
+            (np.repeat(np.linspace(0, 1, 2), 2),
+             np.tile(np.linspace(0, 1, 2), 2))
+        ).T,
+        names=('chi1', 'chi2')
+    )
+    SNR = 10.
+    res = list()
+    for spin_vals in spins:
+        SNR *= np.ones(len(t))
+        chi1 = spin_vals['chi1'] * np.ones(len(t))
+        chi2 = spin_vals['chi2'] * np.ones(len(t))
+        # make predictions and make plots
+        param_sweep_features = np.stack(
+            [t['mass1'], t['mass2'], chi1, chi2, SNR]
+        ).T
+        predictions = clf.predict_proba(param_sweep_features).T[1]
+        res.append((param_sweep_features, predictions))
+    return res
+
+
+def _create_param_sweep_plot(clf, category, prefix=None):
+    """Create a parameter sweep plot using the supplied classifer"""
+    import matplotlib.pyplot as plt
+    res = _get_param_sweep(clf)
+    fig = plt.figure(figsize=(14, 20))
+    for idx, r in enumerate(res):
+        features, predictions = r
+        # FIXME: Ugly, but works
+        title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
+            features[0][2], features[0][3],
+            features[0][4]
+        )
+        make_plots(
+            features, predictions, title,
+            (fig, idx+1), prefix=prefix, category=category
+        )
+    try:
+        plt.savefig(prefix+'_param_sweep_'+category+'.png')
+    except TypeError:
+        plt.savefig('param_sweep_'+category+'.png')
+
+
+def load_eos_posterior():
+    '''
+    Loads eos posterior draws (https://zenodo.org/record/6502467#.Yoa2EKjMI2z)
+
+    Returns
+    -------
+    draws: np.array
+        equally weighted eos draws from file
+    '''
+    eos_file = PACKAGE_FILENAMES['EOS_POSTERIOR_DRAWS.h5']
+    with h5py.File(eos_file, 'r') as f:
+        draws = np.array(f['EOS'])
+    return draws
+
+
+def param_sweep_plot():
+    """Create parameter sweep plot, weighting classifier
+    results using bayes factor
+    """
+    parser = ArgumentParser(
+        "Create a parameter sweep, EoS predictions based")
+    parser.add_argument("-i", "--input", required=True,
+                        help="Directory storing trained classifier files")
+    parser.add_argument("-c", "--config", required=True,
+                        help="Config file")
+    parser.add_argument("-v", "--verbose", action='store_true',
+                        help="show progress")
+    args = parser.parse_args()
+
+    config = ConfigParser()
+    config.read(args.config)
+
+    train_prefix = config.get('output_filenames', 'em_bright_train_prefix')
+    train_suffix = config.get('output_filenames', 'em_bright_train_suffix')
+    clf_filenames = glob.glob(
+        os.path.join(args.input, f'{train_prefix}*{train_suffix}'))
+    if args.verbose:
+        print("Trained classifers", clf_filenames)
+    assert clf_filenames, "No files found. Check directory."
+    reweight_ns = dict.fromkeys(EOS_BAYES_FACTORS)
+    reweight_em = dict.fromkeys(EOS_BAYES_FACTORS)
+    import matplotlib.pyplot as plt
+    for fname in clf_filenames:
+        if args.verbose:
+            print(fname)
+        clf_ns, clf_em = _open_and_return_clfs(fname)
+        eosname, *_ = filter(
+            lambda _: re.match(
+                ".*" + _ + config.get('output_filenames',
+                                      'em_bright_train_suffix'),
+                fname
+            ), EOS_BAYES_FACTORS
+        )
+        res_ns = _get_param_sweep(clf_ns)
+        res_em = _get_param_sweep(clf_em)
+        reweight_ns.update(
+            {
+                eosname: dict(
+                    features=np.array(
+                        [f for f, p in res_ns]
+                    ),
+                    predictions=np.array(
+                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_ns]
+                    )
+                )
+            }
+        )
+        reweight_em.update(
+            {
+                eosname: dict(
+                    features=np.array(
+                        [f for f, p in res_em]
+                    ),
+                    predictions=np.array(
+                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_em]
+                    )
+                )
+            }
+        )
+    assert all(reweight_ns.values()), "Missing some listed EOSs."
+    assert all(reweight_em.values()), "Missing some listed EOSs."
+    reweighted_score_ns = np.sum(
+        [v['predictions'] for v in reweight_ns.values()],
+        axis=0
+    )
+    reweighted_score_em = np.sum(
+        [v['predictions'] for v in reweight_em.values()],
+        axis=0
+    )
+    for category, score in zip(
+            ["NS", "EMB"], [reweighted_score_ns, reweighted_score_em]):
+        fig = plt.figure(figsize=(14, 20))
+        for idx, (f, p) in enumerate(
+                zip(reweight_ns['SLy']['features'], score)):
+            title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
+                f[0][2], f[0][3], f[0][4])
+            make_plots(
+                f, p, title, (fig, idx+1),
+                prefix='SLy', category=category
+            )
+        plt.savefig("reweighted_" + category + "_param_sweep.png")
+
+
+def make_plots(features, predictions, title, fig_idx,
+               prefix=None, category=None):
+    import matplotlib.pyplot as plt
+    fig_, idx = fig_idx
+    fig_.add_subplot(4, 1, idx)
+    # indices 0 and 1 correspond to mass1 and mass2 respectively
+    plt.scatter(features.T[0], features.T[1],
+                s=10, c=predictions)
+    plt.title(title)
+    plt.tight_layout()
+    plt.colorbar(label='Probability')
+    # plot chirp mass contours
+    m1 = np.linspace(1, 20, 1000)
+    m2 = np.linspace(1, 20, 1000)
+    M1, M2 = np.meshgrid(m1, m2)
+    s1z = np.unique(features.T[2])[0]*np.ones(M1.shape)
+    s2z = np.unique(features.T[3])[0]*np.ones(M2.shape)
+    rem_masses = list()
+    for _ in range(M1.shape[0]):
+        rem_masses.append(
+            computeDiskMass.computeDiskMass(
+                M1[_], M2[_], s1z[_], s2z[_],
+                eosname=prefix
+            )
+        )
+    rem_masses = np.array(rem_masses).reshape(M1.shape)
+    Mc = (M1*M2)**(3./5.)/(M1 + M2)**(1./5.)
+    mask = M1 > M2
+    M1 = np.ma.masked_array(M1, mask=mask)
+    M2 = np.ma.masked_array(M2, mask=mask)
+    s1z = np.ma.masked_array(s1z, mask=mask)
+    s2z = np.ma.masked_array(s2z, mask=mask)
+    Mc = np.ma.masked_array(Mc, mask=mask)
+    rem_masses = np.ma.masked_array(
+        rem_masses, mask=mask*(M2 > EOS_MAX_MASS[prefix])
+    )
+    CS = plt.contour(
+        M1, M2, Mc.T, levels=[2.01, 2.22, 2.99, 3.48, 4.73, 5.4],
+        # (m1, m2) = (4, 1.4) -> Mc = 2.01
+        # (m1, m2) = (5, 1.4) -> Mc = 2.22
+        # (m1, m2) = (10, 1.4) -> Mc = 2.99
+        # (m1, m2) = (4, 4)    -> Mc = 3.48
+        # (m1, m2) = (30, 1.4) -> Mc = 4.73
+        # (m1, m2) = (10, 4)  -> Mc = 5.4
+        # three different NSBH populations;
+        # three different mass-gap populations
+        colors='black', linewidths=1.0
+    )
+    plt.clabel(CS, inline=True, fontsize=16)
+    plt.xlim((1, 20))
+    plt.ylim((1, 12))
+    try:
+        max_mass = EOS_MAX_MASS[prefix]
+    except KeyError:
+        max_mass = 3.0
+    if 'NS' in category:
+        plt.axhline(y=max_mass, c='r', linewidth=1.2)
+    elif 'EM' in category:
+        CS = plt.contour(M1, M2, rem_masses.T,
+                         levels=[0., ], colors='red',
+                         linewidths=1.2)
+    plt.xlabel(r'$m_1$', fontsize=16)
+    plt.ylabel(r'$m_2$', fontsize=16)
+
+
+def run_k_fold_split(features, targets, n_splits=10, random_state=0,
+                     training_task=None, **kwargs):
+    """Split the `features` in `n_splits`, train on `n_splits - 1`
+    sets, test on the last fraction. This performed across the complete
+    dataset.
+
+    Parameters
+    ----------
+    features : numpy.ndarray
+        Feature set
+    targets : numpy.ndarray
+        Target set containing binary classification of `features`
+    n_splits : int
+        Number of splits for `features` and `targets`
+    random_state : int
+        Random seed for the split
+    training_task : callable
+        function with arguments (X_train, y_train, X_test, **kwargs) which
+        trains, and returns predictions on X_test.
+        E.g. :meth:`run_KNN_classifier`,
+        or :meth:`run_RF_classifier`.
+    **kwargs
+        Keyword arguments passed to `training_task`.
+
+    Returns
+    -------
+    tuple
+        (res_predict, res_predict_proba) - predictions and probabilities
+    """
+    res_predict_proba = np.empty(len(features))
+    res_predict = np.empty(len(features))
+    res_predict_proba[:] = np.nan
+    res_predict[:] = np.nan
+
+    sss = KFold(n_splits=n_splits, shuffle=True, random_state=random_state)
+    sss.get_n_splits(features, targets)
+    for train_index, test_index in sss.split(features, targets):
+        X_train, X_test, y_train = \
+            features.iloc[train_index], \
+            features.iloc[test_index], \
+            targets.iloc[train_index]
+
+        predict_proba, predict = training_task(X_train, y_train, X_test,
+                                               **kwargs)
+        # second column is the prob of NS/EMB
+        predict_proba = predict_proba.T[1]
+
+        res_predict_proba[test_index] = predict_proba
+        res_predict[test_index] = predict
+    return res_predict, res_predict_proba
+
+
+def run_KNN_classifier(X_train, y_train,
+                       X_test,
+                       **kwargs):
+    '''
+    Run KNearestNeighborClassifier classifier returns
+    `clf.predict_proba`
+
+    Parameters
+    ----------
+    X_train : numpy.ndarray
+        Feature training set, can be array or Dataframe
+    y_train : numpy.array
+        Target training set, 0 or 1 binary classification
+    X_test : numpy.ndarray
+        Feature testing set, can be array or DataFrame
+    '''
+    if kwargs.get('metric') == 'mahalanobis':
+        kwargs['n_jobs'] = 1  # issue with KDTree, BallTree with n_jobs > 1
+    clf = KNeighborsClassifier(**kwargs)
+    clf.fit(X_train.values, y_train)
+    predictions_proba = clf.predict_proba(X_test)
+    predict = clf.predict(X_test)
+    return predictions_proba, predict
+
+
+def run_RF_classifier(X_train, y_train, X_test,
+                      **kwargs):
+    '''
+    Run RandomForestClassifier; returns
+    `clf.predict_proba`
+
+    Parameters
+    ----------
+    X_train : numpy.ndarray
+        Feature training set, can be array or Dataframe
+    y_train : numpy.array
+        Target training set, 0 or 1 binary classification
+    X_test : numpy.ndarray
+        Feature testing set, can be array or DataFrame
+    '''
+    clf = RandomForestClassifier(**kwargs)
+    clf.fit(X_train.values, y_train)
+    predictions_proba = clf.predict_proba(X_test)
+    predict = clf.predict(X_test)
+    return predictions_proba, predict
```

### Comparing `ligo_em_bright-1.1.4.post2/pyproject.toml` & `ligo_em_bright-1.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ligo.em-bright"
-version = "1.1.4.post2"
+version = "1.1.5"
 description = "Possibility and properties of Electromagnetically-bright sources of gravitational-wave events"
 readme = "README.md"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Shaon Ghosh <shaon.ghosh@ligo.org>"]
 packages = [
     { include = "ligo" },
```

### Comparing `ligo_em_bright-1.1.4.post2/PKG-INFO` & `ligo_em_bright-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-em-bright
-Version: 1.1.4.post2
+Version: 1.1.5
 Summary: Possibility and properties of Electromagnetically-bright sources of gravitational-wave events
 License: MIT
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

