# Comparing `tmp/chemcoord-2.0.5.tar.gz` & `tmp/chemcoord-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemcoord-2.0.5.tar", last modified: Sun Jan  9 20:53:00 2022, max compression
+gzip compressed data, was "chemcoord-2.1.0.tar", last modified: Fri Aug  4 14:13:29 2023, max compression
```

## Comparing `chemcoord-2.0.5.tar` & `chemcoord-2.1.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.351935 chemcoord-2.0.5/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      230 2019-01-20 11:04:12.000000 chemcoord-2.0.5/CHANGELOG.md
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     7644 2019-01-20 11:04:11.000000 chemcoord-2.0.5/LICENSE.md
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2019-01-20 11:04:11.000000 chemcoord-2.0.5/MANIFEST.in
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5149 2022-01-09 20:53:00.351935 chemcoord-2.0.5/PKG-INFO
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4057 2022-01-09 20:46:02.000000 chemcoord-2.0.5/README.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.327935 chemcoord-2.0.5/docs/
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.331935 chemcoord-2.0.5/docs/source/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      546 2021-07-11 14:54:23.000000 chemcoord-2.0.5/docs/source/bugs.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      965 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/cartesian_coordinates.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     1081 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/configuration.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/documentation.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      275 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/exceptions.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     2349 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      844 2021-07-11 14:54:23.000000 chemcoord-2.0.5/docs/source/installation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      690 2022-01-09 18:25:06.000000 chemcoord-2.0.5/docs/source/internal_coordinates.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     7445 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/license.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1381 2022-01-09 18:25:06.000000 chemcoord-2.0.5/docs/source/references.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.331935 chemcoord-2.0.5/docs/source/src_AsymmetricUnitCartesian/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      258 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.331935 chemcoord-2.0.5/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.get_cartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.331935 chemcoord-2.0.5/docs/source/src_Cartesian/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     3039 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/chemcoord.Cartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.339935 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.__init__.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._divide_et_impera.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      152 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._preserve_bonds.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.add_data.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.align.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.append.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.basistransform.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.change_numbering.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_absolute_refs.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_dihedral.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.columns.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.copy.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_absolute_refs.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_dihedral.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_cuboid.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_sphere.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.fragmentate.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_ase_atoms.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      173 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_pymatgen_molecule.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      158 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_angle_degrees.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      146 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_ase_atoms.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_asymmetric_unit.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_barycenter.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      155 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bond_lengths.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bonds.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      141 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_centroid.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      173 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_construction_table.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      176 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_coordination_sphere.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      167 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_dihedral_degrees.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      152 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_distance_to.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_electron_number.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      167 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_equivalent_atoms.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      141 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_fragment.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_grad_zmat.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_inertia.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pointgroup.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pymatgen_molecule.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_shortest_distance.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_total_mass.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_without.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_zmat.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.iloc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.index.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.insert.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.loc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      161 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.partition_chem_env.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_cjson.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_xyz.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.reindex_similar.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.replace.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      161 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.restrict_bond_dict.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.set_index.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_index.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_values.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.subs.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.symmetrize.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_cjson.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_latex.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_string.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_xyz.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_zmat.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.view.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.write_xyz.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.339935 chemcoord-2.0.5/docs/source/src_PointGroupOperations/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.339935 chemcoord-2.0.5/docs/source/src_Zmat/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     1204 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/chemcoord.Zmat.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.343935 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.__init__.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      114 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.add_data.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.change_numbering.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.columns.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.copy.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      109 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.dtypes.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_cartesian.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_electron_number.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_grad_cartesian.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      134 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_total_mass.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.has_same_sumformula.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      103 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iloc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.index.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.insert.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iupacify.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.loc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      144 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.minimize_dihedrals.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.read_zmat.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_iloc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_loc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.shape.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_index.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_values.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.subs.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      114 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_latex.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_string.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      108 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_xyz.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      111 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_zmat.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_iloc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_loc.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      103 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.write.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.347935 chemcoord-2.0.5/docs/source/src_configuration/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      182 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_configuration/chemcoord.configuration.read_configuration_file.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      185 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_configuration/chemcoord.configuration.write_configuration_file.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.347935 chemcoord-2.0.5/docs/source/src_exceptions/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_exceptions/chemcoord.exceptions.IllegalArgumentCombination.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_exceptions/chemcoord.exceptions.InvalidReference.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_exceptions/chemcoord.exceptions.PhysicalMeaning.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_exceptions/chemcoord.exceptions.UndefinedCoordinateSystem.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.347935 chemcoord-2.0.5/docs/source/src_xyz_functions/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      143 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.allclose.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      179 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.apply_grad_zmat_tensor.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      137 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.concat.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      128 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.dot.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      140 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.isclose.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      154 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.read_molden.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.to_molden.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      131 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.view.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_xyz_functions/chemcoord.xyz_functions.write_molden.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.347935 chemcoord-2.0.5/docs/source/src_zmat_functions/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_zmat_functions/chemcoord.zmat_functions.DummyManipulation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      176 2022-01-09 18:25:06.000000 chemcoord-2.0.5/docs/source/src_zmat_functions/chemcoord.zmat_functions.PureInternalMovement.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      158 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_zmat_functions/chemcoord.zmat_functions.TestOperators.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      197 2019-01-20 11:04:11.000000 chemcoord-2.0.5/docs/source/src_zmat_functions/chemcoord.zmat_functions.apply_grad_cartesian_tensor.rst
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)      896 2022-01-09 19:33:50.000000 chemcoord-2.0.5/docs/source/tutorial.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       38 2022-01-09 20:53:00.351935 chemcoord-2.0.5/setup.cfg
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1978 2022-01-09 19:13:07.000000 chemcoord-2.0.5/setup.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.327935 chemcoord-2.0.5/src/
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.347935 chemcoord-2.0.5/src/chemcoord/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1141 2021-07-11 14:55:04.000000 chemcoord-2.0.5/src/chemcoord/__init__.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.347935 chemcoord-2.0.5/src/chemcoord/_generic_classes/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/_generic_classes/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      490 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/_generic_classes/generic_IO.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3052 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/_generic_classes/generic_core.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.351935 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    49226 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cart_transformation.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    52210 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    31689 2021-10-13 09:09:19.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    14387 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    11428 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4671 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     1270 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_indexers.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1411 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3277 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/cartesian_class_main.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      989 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/point_group.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    16332 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/xyz_functions.py
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     3385 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/configuration.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    67997 2021-07-11 14:55:04.000000 chemcoord-2.0.5/src/chemcoord/constants.py
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     2257 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/exceptions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.351935 chemcoord-2.0.5/src/chemcoord/internal_coordinates/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2922 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/_indexers.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    30240 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_class_core.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7486 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_class_io.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3027 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4352 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_transformation.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3182 2021-07-11 14:54:23.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/zmat_class_main.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4390 2022-01-09 18:25:06.000000 chemcoord-2.0.5/src/chemcoord/internal_coordinates/zmat_functions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.351935 chemcoord-2.0.5/src/chemcoord/utilities/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/utilities/__init__.py
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     3365 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/utilities/_decorators.py
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     4591 2019-01-20 11:04:11.000000 chemcoord-2.0.5/src/chemcoord/utilities/_print_versions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2022-01-09 20:53:00.347935 chemcoord-2.0.5/src/chemcoord.egg-info/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5149 2022-01-09 20:53:00.000000 chemcoord-2.0.5/src/chemcoord.egg-info/PKG-INFO
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10517 2022-01-09 20:53:00.000000 chemcoord-2.0.5/src/chemcoord.egg-info/SOURCES.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        1 2022-01-09 20:53:00.000000 chemcoord-2.0.5/src/chemcoord.egg-info/dependency_links.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       78 2022-01-09 20:53:00.000000 chemcoord-2.0.5/src/chemcoord.egg-info/requires.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       10 2022-01-09 20:53:00.000000 chemcoord-2.0.5/src/chemcoord.egg-info/top_level.txt
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      905 2023-08-04 13:10:33.000000 chemcoord-2.1.0/CHANGELOG.md
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7644 2023-06-19 10:17:01.000000 chemcoord-2.1.0/LICENSE.md
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2023-06-19 10:17:01.000000 chemcoord-2.1.0/MANIFEST.in
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5858 2023-08-04 14:13:29.989633 chemcoord-2.1.0/PKG-INFO
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4766 2023-08-02 12:14:08.000000 chemcoord-2.1.0/README.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      546 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/bugs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      965 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/cartesian_coordinates.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1081 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/configuration.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/documentation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      275 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/exceptions.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2349 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      844 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/installation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      690 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/internal_coordinates.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7445 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/license.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1381 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/references.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      258 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.get_cartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/docs/source/src_Cartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3039 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/chemcoord.Cartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.981633 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.__init__.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._divide_et_impera.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      152 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._preserve_bonds.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.add_data.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.align.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.append.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.basistransform.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.change_numbering.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_absolute_refs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_dihedral.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.columns.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.copy.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_absolute_refs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_dihedral.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_cuboid.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_sphere.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.fragmentate.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_ase_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      173 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_pymatgen_molecule.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      158 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_angle_degrees.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      146 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_ase_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_asymmetric_unit.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_barycenter.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      155 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bond_lengths.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bonds.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      141 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_centroid.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      173 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_construction_table.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      176 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_coordination_sphere.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      167 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_dihedral_degrees.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      152 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_distance_to.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      164 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_electron_number.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      167 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_equivalent_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      141 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_fragment.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_grad_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_inertia.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pointgroup.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pymatgen_molecule.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_shortest_distance.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_total_mass.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_without.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.insert.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      161 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.partition_chem_env.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_cjson.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.reindex_similar.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.replace.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      161 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.restrict_bond_dict.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.set_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_values.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.subs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.symmetrize.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_cjson.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_latex.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_string.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.view.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.write_xyz.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.981633 chemcoord-2.1.0/docs/source/src_PointGroupOperations/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.981633 chemcoord-2.1.0/docs/source/src_Zmat/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1204 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/chemcoord.Zmat.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.__init__.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      114 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.add_data.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.change_numbering.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.columns.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.copy.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      109 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.dtypes.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_cartesian.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_electron_number.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      138 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_grad_cartesian.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      134 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_total_mass.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      149 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.has_same_sumformula.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      103 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.insert.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iupacify.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      144 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.minimize_dihedrals.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.read_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      106 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.shape.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      120 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_values.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      100 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.subs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      114 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_latex.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      117 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_string.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      108 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      111 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      123 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      103 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.write.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_configuration/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      182 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_configuration/chemcoord.configuration.read_configuration_file.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      185 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_configuration/chemcoord.configuration.write_configuration_file.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_exceptions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.IllegalArgumentCombination.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.InvalidReference.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.PhysicalMeaning.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_exceptions/chemcoord.exceptions.UndefinedCoordinateSystem.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_xyz_functions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      143 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.allclose.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      179 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.apply_grad_zmat_tensor.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      137 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.concat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      128 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.dot.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      140 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.isclose.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      154 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.read_molden.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.to_molden.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      131 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.view.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_xyz_functions/chemcoord.xyz_functions.write_molden.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/docs/source/src_zmat_functions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.DummyManipulation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      176 2023-08-02 12:14:08.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.PureInternalMovement.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      158 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.TestOperators.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      197 2023-06-19 10:17:01.000000 chemcoord-2.1.0/docs/source/src_zmat_functions/chemcoord.zmat_functions.apply_grad_cartesian_tensor.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      896 2023-08-04 13:10:33.000000 chemcoord-2.1.0/docs/source/tutorial.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       38 2023-08-04 14:13:29.989633 chemcoord-2.1.0/setup.cfg
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1978 2023-08-04 13:10:33.000000 chemcoord-2.1.0/setup.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.973633 chemcoord-2.1.0/src/
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/src/chemcoord/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1187 2023-08-04 14:06:41.000000 chemcoord-2.1.0/src/chemcoord/__init__.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/src/chemcoord/_generic_classes/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/_generic_classes/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      490 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/_generic_classes/generic_IO.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3058 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/_generic_classes/generic_core.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    49583 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cart_transformation.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    52210 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    32040 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    14387 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10567 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4671 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1641 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_indexers.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1411 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3277 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/cartesian_class_main.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      989 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/point_group.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    16332 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/xyz_functions.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3385 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/configuration.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    67997 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/constants.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2257 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/exceptions.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/src/chemcoord/internal_coordinates/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2922 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_indexers.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    30873 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_core.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7487 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_io.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3027 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5573 2023-08-04 12:49:57.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_transformation.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3182 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_class_main.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4390 2023-08-02 12:14:08.000000 chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_functions.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.989633 chemcoord-2.1.0/src/chemcoord/utilities/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/utilities/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3365 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/utilities/_decorators.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4591 2023-06-19 10:17:01.000000 chemcoord-2.1.0/src/chemcoord/utilities/_print_versions.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-08-04 14:13:29.985633 chemcoord-2.1.0/src/chemcoord.egg-info/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5858 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/PKG-INFO
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10517 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        1 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/requires.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       10 2023-08-04 14:13:29.000000 chemcoord-2.1.0/src/chemcoord.egg-info/top_level.txt
```

### Comparing `chemcoord-2.0.5/LICENSE.md` & `chemcoord-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/PKG-INFO` & `chemcoord-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemcoord
-Version: 2.0.5
+Version: 2.1.0
 Summary: Python module for dealing with chemical coordinates.
 Home-page: https://github.com/mcocdawc/chemcoord
 Author: Oskar Weser
 Author-email: oskar.weser@gmail.com
 License: LGPLv3
 Keywords: chemcoord,transformation,cartesian,internal,chemistry,zmatrix,xyz,zmat,coordinates,coordinate system
 Platform: UNKNOWN
@@ -52,40 +52,39 @@
      - .. image:: https://codecov.io/gh/mcocdawc/chemcoord/branch/master/graph/badge.svg
             :target: https://codecov.io/gh/mcocdawc/chemcoord
 
 
 Website
 -------
 
-The project’s website with documentation is:
+The project's website with documentation is:
 http://chemcoord.readthedocs.org/
 
 Features
 --------
 
 -  Molecules are reliably transformed between cartesian space and non
    redundant internal coordinates (Zmatrices). Dummy atoms are inserted
    and removed automatically on the fly if necessary.
 -  The created Zmatrix is not only a structure expressed in internal
-   coordinates, it is a “chemical” Zmatrix. “Chemical” Zmatrix means,
-   that e.g. distances are along bonds or dihedrals are defined as they
+   coordinates, it is a "chemical" Zmatrix. "Chemical" Zmatrix means,
+   that e.g. distances are along bonds or dihedrals are defined as they
    are drawn in chemical textbooks (Newman projections).
 -  Analytical gradients for the transformations between the different
    coordinate systems are implemented.
 -  Performance intensive functions/methods are implemented with
    Fortran/C like speed using `numba <http://numba.pydata.org/>`__.
 -  Geometries may be defined with symbolic expressions using
    `sympy <http://www.sympy.org/en/index.html>`__.
 -  Built on top of `pandas <http://pandas.pydata.org/>`__ with very
    similar syntax. This allows for example distinct label or row based
    indexing.
 -  It derived from my own work and I heavily use it during the day. So
    all functions are tested and tailored around the work flow in
    theoretical chemistry.
--  The classes are safe to inherit from and can easily be customized.
 -  `It as a python module ;) <https://xkcd.com/353/>`__
 
 Installation guide
 ------------------
 
 A working python 3 installation is required (>=3.7 are possible).
 
@@ -93,25 +92,19 @@
 `Ipython <http://ipython.org/>`__ and `jupyter <http://jupyter.org/>`__.
 They come shipped by default with the `anaconda3
 installer <https://www.continuum.io/downloads/>`__
 
 Unix
 ~~~~
 
-For the packaged versions, the following commands have to be executed in
+For the packaged version, the following commands have to be executed in
 the terminal:
 
 ::
 
-   conda install -c mcocdawc chemcoord
-
-or
-
-::
-
    pip install chemcoord
 
 For the up to date development version (experimental):
 
 ::
 
    git clone https://github.com/mcocdawc/chemcoord.git
@@ -121,24 +114,49 @@
 Windows
 ~~~~~~~
 
 Neither installation nor running the module are tested on windows. To
 the best of my knowledge it should work there as well. Just use the same
 steps as for UNIX.
 
-Changelog
-~~~~~~~~~
-
-The changelog can be found
-`here <https://github.com/mcocdawc/chemcoord/blob/master/CHANGELOG.md>`__.
 
 Citation and mathematical background
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If chemcoord is used in a project that leads to a scientific
-publication, please acknowledge this fact by citing `this preprint <https://chemrxiv.org/engage/chemrxiv/article-details/615c0ae97d3da5630aed6dc0>`__.
+The theory behind chemcoord is described in `this paper <https://onlinelibrary.wiley.com/doi/full/10.1002/jcc.27029>`__.
+If this package is used in a project that leads to a scientific
+publication, please acknowledge it by citing.
+
+::
+
+    @article{https://doi.org/10.1002/jcc.27029,
+        author = {Weser, Oskar and Hein-Janke, Björn and Mata, Ricardo A.},
+        title = {Automated handling of complex chemical structures in Z-matrix coordinates—The chemcoord library},
+        journal = {Journal of Computational Chemistry},
+        volume = {44},
+        number = {5},
+        pages = {710-726},
+        keywords = {analytical gradients, geometry optimization, non-linear constraints, transition state search, Z-matrix},
+        doi = {10.1002/jcc.27029},
+        year = {2023}
+    }
 
-My (Oskar Weser) master thesis including the derivation of implemented equations and
+
+My (Oskar Weser) master thesis including a more detailed derivation of implemented equations and
 the mathematical background can be found
 `here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/files/master_thesis_oskar_weser_chemcoord.pdf>`__.
 
 
+
+Acknowledgement
+~~~~~~~~~~~~~~~
+
+
+.. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
+   :width: 80
+   :align: left
+   :target: https://zulip.com/
+
+Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
+that supports the development of chemcoord with a free plan.
+
+
```

### Comparing `chemcoord-2.0.5/README.rst` & `chemcoord-2.1.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -26,40 +26,39 @@
      - .. image:: https://codecov.io/gh/mcocdawc/chemcoord/branch/master/graph/badge.svg
             :target: https://codecov.io/gh/mcocdawc/chemcoord
 
 
 Website
 -------
 
-The project’s website with documentation is:
+The project's website with documentation is:
 http://chemcoord.readthedocs.org/
 
 Features
 --------
 
 -  Molecules are reliably transformed between cartesian space and non
    redundant internal coordinates (Zmatrices). Dummy atoms are inserted
    and removed automatically on the fly if necessary.
 -  The created Zmatrix is not only a structure expressed in internal
-   coordinates, it is a “chemical” Zmatrix. “Chemical” Zmatrix means,
-   that e.g. distances are along bonds or dihedrals are defined as they
+   coordinates, it is a "chemical" Zmatrix. "Chemical" Zmatrix means,
+   that e.g. distances are along bonds or dihedrals are defined as they
    are drawn in chemical textbooks (Newman projections).
 -  Analytical gradients for the transformations between the different
    coordinate systems are implemented.
 -  Performance intensive functions/methods are implemented with
    Fortran/C like speed using `numba <http://numba.pydata.org/>`__.
 -  Geometries may be defined with symbolic expressions using
    `sympy <http://www.sympy.org/en/index.html>`__.
 -  Built on top of `pandas <http://pandas.pydata.org/>`__ with very
    similar syntax. This allows for example distinct label or row based
    indexing.
 -  It derived from my own work and I heavily use it during the day. So
    all functions are tested and tailored around the work flow in
    theoretical chemistry.
--  The classes are safe to inherit from and can easily be customized.
 -  `It as a python module ;) <https://xkcd.com/353/>`__
 
 Installation guide
 ------------------
 
 A working python 3 installation is required (>=3.7 are possible).
 
@@ -67,25 +66,19 @@
 `Ipython <http://ipython.org/>`__ and `jupyter <http://jupyter.org/>`__.
 They come shipped by default with the `anaconda3
 installer <https://www.continuum.io/downloads/>`__
 
 Unix
 ~~~~
 
-For the packaged versions, the following commands have to be executed in
+For the packaged version, the following commands have to be executed in
 the terminal:
 
 ::
 
-   conda install -c mcocdawc chemcoord
-
-or
-
-::
-
    pip install chemcoord
 
 For the up to date development version (experimental):
 
 ::
 
    git clone https://github.com/mcocdawc/chemcoord.git
@@ -95,22 +88,47 @@
 Windows
 ~~~~~~~
 
 Neither installation nor running the module are tested on windows. To
 the best of my knowledge it should work there as well. Just use the same
 steps as for UNIX.
 
-Changelog
-~~~~~~~~~
-
-The changelog can be found
-`here <https://github.com/mcocdawc/chemcoord/blob/master/CHANGELOG.md>`__.
 
 Citation and mathematical background
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If chemcoord is used in a project that leads to a scientific
-publication, please acknowledge this fact by citing `this preprint <https://chemrxiv.org/engage/chemrxiv/article-details/615c0ae97d3da5630aed6dc0>`__.
+The theory behind chemcoord is described in `this paper <https://onlinelibrary.wiley.com/doi/full/10.1002/jcc.27029>`__.
+If this package is used in a project that leads to a scientific
+publication, please acknowledge it by citing.
+
+::
+
+    @article{https://doi.org/10.1002/jcc.27029,
+        author = {Weser, Oskar and Hein-Janke, Björn and Mata, Ricardo A.},
+        title = {Automated handling of complex chemical structures in Z-matrix coordinates—The chemcoord library},
+        journal = {Journal of Computational Chemistry},
+        volume = {44},
+        number = {5},
+        pages = {710-726},
+        keywords = {analytical gradients, geometry optimization, non-linear constraints, transition state search, Z-matrix},
+        doi = {10.1002/jcc.27029},
+        year = {2023}
+    }
 
-My (Oskar Weser) master thesis including the derivation of implemented equations and
+
+My (Oskar Weser) master thesis including a more detailed derivation of implemented equations and
 the mathematical background can be found
 `here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/files/master_thesis_oskar_weser_chemcoord.pdf>`__.
+
+
+
+Acknowledgement
+~~~~~~~~~~~~~~~
+
+
+.. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
+   :width: 80
+   :align: left
+   :target: https://zulip.com/
+
+Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
+that supports the development of chemcoord with a free plan.
```

### Comparing `chemcoord-2.0.5/docs/source/bugs.rst` & `chemcoord-2.1.0/docs/source/bugs.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/cartesian_coordinates.rst` & `chemcoord-2.1.0/docs/source/cartesian_coordinates.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/configuration.rst` & `chemcoord-2.1.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/index.rst` & `chemcoord-2.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/installation.rst` & `chemcoord-2.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/internal_coordinates.rst` & `chemcoord-2.1.0/docs/source/internal_coordinates.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/license.rst` & `chemcoord-2.1.0/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/references.rst` & `chemcoord-2.1.0/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/src_Cartesian/chemcoord.Cartesian.rst` & `chemcoord-2.1.0/docs/source/src_Cartesian/chemcoord.Cartesian.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/src_Zmat/chemcoord.Zmat.rst` & `chemcoord-2.1.0/docs/source/src_Zmat/chemcoord.Zmat.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/docs/source/tutorial.rst` & `chemcoord-2.1.0/docs/source/tutorial.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Tutorial
 ==================
 
 Just follow the link to the example notebooks.
 
 
-  * `Cartesian <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.0.5/Tutorial/Cartesian.ipynb>`_
-  * `Zmat <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.0.5/Tutorial/Zmat.ipynb>`_
-  * `Transformation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.0.5/Tutorial/Transformation.ipynb>`_
-  * `Gradients <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.0.5/Tutorial/Gradients.ipynb>`_
-  * `Advanced customisation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.0.5/Tutorial/Advanced_customisation.ipynb>`_
+  * `Cartesian <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Cartesian.ipynb>`_
+  * `Zmat <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Zmat.ipynb>`_
+  * `Transformation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Transformation.ipynb>`_
+  * `Gradients <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Gradients.ipynb>`_
+  * `Advanced customisation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.0/Tutorial/Advanced_customisation.ipynb>`_
 
 If you want to have an interactive session, just download the following
-`zip file <https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/mcocdawc/chemcoord/tree/v2.0.5/Tutorial>`_,
+`zip file <https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/mcocdawc/chemcoord/tree/v2.1.0/Tutorial>`_,
 which contains all notebooks and coordinates.
```

### Comparing `chemcoord-2.0.5/setup.py` & `chemcoord-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 MAIN_PACKAGE = 'chemcoord'
 DESCRIPTION = "Python module for dealing with chemical coordinates."
 LICENSE = 'LGPLv3'
 AUTHOR = 'Oskar Weser'
 EMAIL = 'oskar.weser@gmail.com'
 URL = 'https://github.com/mcocdawc/chemcoord'
-INSTALL_REQUIRES = ['numpy>=1.21', 'scipy', 'pandas>=1.0', 'numba>=0.35',
+INSTALL_REQUIRES = ['numpy>=1.0', 'scipy', 'pandas>=1.0', 'numba>=0.35',
                     'sortedcontainers', 'sympy', 'six', 'pymatgen']
 KEYWORDS = ['chemcoord', 'transformation', 'cartesian', 'internal',
             'chemistry', 'zmatrix', 'xyz', 'zmat', 'coordinates',
             'coordinate system']
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
@@ -29,15 +29,15 @@
     'Natural Language :: English',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Topic :: Scientific/Engineering :: Chemistry',
     'Topic :: Scientific/Engineering :: Physics']
-VERSION = '2.0.5'
+VERSION = '2.1.0'
 
 
 def readme():
     '''Return the contents of the README.md file.'''
     with open('README.rst') as freadme:
         return freadme.read()
 
@@ -59,7 +59,8 @@
         package_dir={'': 'src'},
         install_requires=INSTALL_REQUIRES,
     )
 
 
 if __name__ == "__main__":
     setup_package()
+
```

### Comparing `chemcoord-2.0.5/src/chemcoord/__init__.py` & `chemcoord-2.1.0/src/chemcoord/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
 
-import pkg_resources  # part of setuptools
-__version__ = pkg_resources.get_distribution("chemcoord").version
+try:
+    from importlib.metadata import version
+except ModuleNotFoundError:
+    from importlib_metadata import version
+
+__version__ = version("chemcoord")
 _git_branch = "master"
 
 
 def export(func):
     if callable(func) and hasattr(func, '__name__'):
         globals()[func.__name__] = func
     try:
```

### Comparing `chemcoord-2.0.5/src/chemcoord/_generic_classes/generic_core.py` & `chemcoord-2.1.0/src/chemcoord/_generic_classes/generic_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         data = constants.elements
         if pd.api.types.is_list_like(new_cols):
             new_cols = set(new_cols)
         elif new_cols is None:
             new_cols = set(data.columns)
         else:
             new_cols = [new_cols]
-        new_frame = data.loc[atoms, set(new_cols) - set(self.columns)]
+        new_frame = data.loc[atoms, list(set(new_cols) - set(self.columns))]
         new_frame.index = self.index
         return self.__class__(pd.concat([self._frame, new_frame], axis=1))
 
     def get_total_mass(self):
         """Returns the total mass in g/mol.
 
         Args:
```

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cart_transformation.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cart_transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # -*- coding: utf-8 -*-
+import warnings
+
 import numba as nb
+from numba.core.errors import NumbaDeprecationWarning
+from numba import jit, generated_jit
 import numpy as np
-from numba import generated_jit, jit
 from numpy import arccos, arctan2, sqrt
 
 import chemcoord.constants as constants
 from chemcoord.cartesian_coordinates.xyz_functions import (_jit_cross,
                                                            _jit_isclose,
                                                            _jit_normalize)
 from chemcoord.exceptions import ERR_CODE_OK, ERR_CODE_InvalidReference
 
 
-@generated_jit(nopython=True)
-def get_ref_pos(X, indices):  # pylint:disable=unused-argument
-    if isinstance(indices, nb.types.Array):
-        def f(X, indices):
-            ref_pos = np.empty((3, len(indices)))
-            for col, i in enumerate(indices):
+with warnings.catch_warnings():
+    # This has to be fixed in the near-future
+    # https://github.com/mcocdawc/chemcoord/issues/76
+    warnings.simplefilter("ignore", category=NumbaDeprecationWarning)
+    @generated_jit(nopython=True)
+    def get_ref_pos(X, indices):  # pylint:disable=unused-argument
+        if isinstance(indices, nb.types.Array):
+            def f(X, indices):
+                ref_pos = np.empty((3, len(indices)))
+                for col, i in enumerate(indices):
+                    if i < constants.keys_below_are_abs_refs:
+                        ref_pos[:, col] = constants._jit_absolute_refs(i)
+                    else:
+                        ref_pos[:, col] = X[:, i]
+                return ref_pos
+            return f
+        elif isinstance(indices, nb.types.Integer):
+            def f(X, indices):
+                i = indices
                 if i < constants.keys_below_are_abs_refs:
-                    ref_pos[:, col] = constants._jit_absolute_refs(i)
+                    ref_pos = constants._jit_absolute_refs(i)
                 else:
-                    ref_pos[:, col] = X[:, i]
-            return ref_pos
-        return f
-    elif isinstance(indices, nb.types.Integer):
-        def f(X, indices):
-            i = indices
-            if i < constants.keys_below_are_abs_refs:
-                ref_pos = constants._jit_absolute_refs(i)
-            else:
-                ref_pos = X[:, i]
-            return ref_pos
-        return f
+                    ref_pos = X[:, i]
+                return ref_pos
+            return f
 
 
 @jit(nopython=True, cache=True)
 def get_B(X, c_table, j):
     B = np.empty((3, 3))
     ref_pos = get_ref_pos(X, c_table[:, j])
     BA = ref_pos[:, 1] - ref_pos[:, 0]
```

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import warnings
 from collections import OrderedDict
 from functools import partial
 from itertools import permutations
 
 import numpy as np
 import pandas as pd
+from numba.core.errors import NumbaPerformanceWarning
 
 import chemcoord.cartesian_coordinates._cart_transformation as transformation
 import chemcoord.cartesian_coordinates.xyz_functions as xyz_functions
 import chemcoord.constants as constants
 from chemcoord.cartesian_coordinates._cartesian_class_core import CartesianCore
 from chemcoord.configuration import settings
 from chemcoord.exceptions import (ERR_CODE_OK, ERR_CODE_InvalidReference,
@@ -230,20 +231,20 @@
         else:
             fragments = fragment_list
 
         def prepend_missing_parts_of_molecule(fragment_list):
             for fragment in fragment_list:
                 if pd.api.types.is_list_like(fragment):
                     try:
-                        full_index = full_index.union(fragment[0].index)
+                        full_index = set(full_index).union(fragment[0].index)
                     except NameError:
                         full_index = fragment[0].index
                 else:
                     try:
-                        full_index = full_index.union(fragment.index)
+                        full_index = set(full_index).union(fragment.index)
                     except NameError:
                         full_index = fragment.index
 
             if not self.index.difference(full_index).empty:
                 missing_part = self.get_without(self.loc[full_index],
                                                 use_lookup=use_lookup)
                 fragment_list = missing_part + fragment_list
@@ -693,15 +694,20 @@
         c_table = c_table.replace(constants.int_label)
         c_table = c_table.replace({k: v for v, k in enumerate(c_table.index)})
         c_table = c_table.values.T
         X = self.loc[:, ['x', 'y', 'z']].values.T
         if X.dtype == np.dtype('i8'):
             X = X.astype('f8')
 
-        err, row, grad_C = transformation.get_grad_C(X, c_table)
+        with warnings.catch_warnings():
+            # There were some performance warnings about non-contiguos arrays.
+            # Unfortunately we cannot do anything about it, on a conceptional level.
+            warnings.simplefilter("ignore", category=NumbaPerformanceWarning)
+            err, row, grad_C = transformation.get_grad_C(X, c_table)
+
         if err == ERR_CODE_InvalidReference:
             rename = dict(enumerate(self.index))
             i = rename[row]
             b, a, d = construction_table.loc[i, ['b', 'a', 'd']]
             raise InvalidReference(i=i, b=b, a=a, d=d)
 
         if as_function:
```

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,14 +111,31 @@
 
     def __setitem__(self, key, value):
         if isinstance(key, tuple):
             self._frame[key[0], key[1]] = value
         else:
             self._frame[key] = value
 
+    def __getattr__(self, name: str):
+        """
+        After regular attribute access, try looking up the name
+        This allows simpler access to columns for interactive use.
+        """
+        # Note: obj.x will always call obj.__getattribute__('x') prior to
+        # calling obj.__getattr__('x').
+
+        if name.startswith('__'):
+            # See here, why we do this
+            # https://stackoverflow.com/questions/47299243/recursionerror-when-python-copy-deepcopy
+            raise AttributeError()
+        if (name in self._frame.columns):
+            return self[name]
+        return object.__getattribute__(self, name)
+
+
     @property
     def index(self):
         """Returns the index.
 
         Assigning a value to it changes the index.
         """
         return self._frame.index
@@ -241,49 +258,14 @@
 
     def reset_index(self):
         """Resets the index to 0...n
         """
         return self.__class__(self._frame.reset_index(drop=True))
 
 
-    def append(self, other, ignore_index=False):
-        """Append rows of `other` to the end of this frame, returning a new object.
-
-        Wrapper around the :meth:`pandas.DataFrame.append` method.
-
-        Args:
-            other (Cartesian):
-            ignore_index (sequence, bool, int): If it is a boolean, it
-                behaves like in the description of
-                :meth:`pandas.DataFrame.append`.
-                If it is a sequence, it becomes the new index.
-                If it is an integer,
-                ``range(ignore_index, ignore_index + len(new))``
-                becomes the new index.
-
-        Returns:
-            Cartesian:
-        """
-        if not isinstance(other, self.__class__):
-            raise ValueError('May only append instances of same type.')
-        if type(ignore_index) is bool:
-            new_frame = self._frame.append(other._frame,
-                                           ignore_index=ignore_index,
-                                           verify_integrity=True)
-        else:
-            new_frame = self._frame.append(other._frame,
-                                           ignore_index=True,
-                                           verify_integrity=True)
-            if type(ignore_index) is int:
-                new_frame.index = range(ignore_index,
-                                        ignore_index + len(new_frame))
-            else:
-                new_frame.index = ignore_index
-        return self.__class__(new_frame)
-
     def insert(self, loc, column, value, allow_duplicates=False,
                inplace=False):
         """Insert column into molecule at specified location.
 
         Wrapper around the :meth:`pandas.DataFrame.insert` method.
         """
         out = self if inplace else self.copy()
```

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/cartesian_class_main.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/cartesian_class_main.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/point_group.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/point_group.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/cartesian_coordinates/xyz_functions.py` & `chemcoord-2.1.0/src/chemcoord/cartesian_coordinates/xyz_functions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/configuration.py` & `chemcoord-2.1.0/src/chemcoord/configuration.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/constants.py` & `chemcoord-2.1.0/src/chemcoord/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 Lu,,71.0,175.0,17.8,d,3668.0,9.8404,"Silvery-white rare-earth metal which is relatively stable in air. It happens to be the most expensive rare-earth metal. Its found with almost all rare-earth metals, but is very difficult to separate from other elements. Least abundant of all natural elements. Used in metal alloys, and as a catalyst in various processes. There are two natural, stable isotopes, and seven radioisotopes, the most stable being Lu-174 with a half-life of 3.3 years. The separation of lutetium from Ytterbium was described by Georges Urbain in 1907. It was discovered at approximately the same time by Carl Auer von Welsbach. The name comes from the Greek word lutetia which means Paris.",148.0,0.34,[Xe] 4f14 5d 6s2,414.0,,3.0,3.51,HEX,174.967,1936.0,Lutetium,6.0,8.0,0.155,,224.00000000000003,187.0,162.0,1.0,6.455,#00ab24,#ff1493,992.0,970.6,427.6,,,175.0,,,,,,364.0,265.0,0.8,1.5e-07,1.6,8.0,1.055,#00ab24,1.6
 Hf,,72.0,167.0,13.6,d,5470.0,13.31,"Silvery lustrous metallic transition element. Used in tungsten alloys in filaments and electrodes, also acts as a neutron absorber. First reported by Urbain in 1911, existence was finally established in 1923 by D. Coster, G.C. de Hevesy in 1923.",109.0,0.013999999999999999,[Xe] 4f14 5d2 6s2,575.0,25.1,4.0,3.2,HEX,178.49,2503.0,Hafnium,6.0,8.0,0.146,23.0,223.0,175.0,152.0,1.3,6.83,#4dc2ff,#ff1493,,,618.4,,,155.0,,,,225.0,,314.1,253.0,3.0,7.000000000000003e-06,1.5,8.0,1.06,#4dc2ff,1.5
 Ta,,73.0,149.0,10.9,d,5698.0,16.654,"Heavy blue-grey metallic transition element. Ta-181 is a stable isotope, and Ta-180 is a radioactive isotope, with a half-life in excess of 10^7 years. Used in surgery as it is unreactive. Forms a passive oxide layer in air. Identified in 1802 by Ekeberg and isolated in 1820 by Jons J. Berzelius.",88.0,0.322,[Xe] 4f14 5d3 6s2,758.0,24.7,5.0,3.31,BCC,180.9479,3269.0,Tantalum,6.0,8.0,0.14,57.5,222.00000000000003,170.0,146.0,1.5,7.93,#4da6ff,#ff1493,,,782.0,,,145.0,,,,220.00000000000003,,317.0,243.00000000000003,2.0,2e-06,1.38,8.0,1.065,#4da6ff,1.38
 W,,74.0,141.0,9.53,d,5930.0,19.3,"White or grey metallic transition element,formerly called Wolfram. Forms a protective oxide in air and can be oxidized at high temperature. First isolated by Jose and Fausto de Elhuyer in 1783.",75.0,0.81626,[Xe] 4f14 5d4 6s2,824.0,35.0,6.0,3.16,BCC,183.84,3680.0,Tungsten,6.0,8.0,0.133,173.0,218.00000000000003,162.0,137.0,1.7,8.67,#2194d6,#ff1493,,,851.0,,,135.0,,,,210.0,,309.6,239.0,1.25,0.0001,1.46,8.0,1.07,#2194d6,1.46
 Re,,75.0,137.0,8.85,d,5900.0,21.02,Silvery-white metallic transition element. Obtained as a by-product of molybdenum refinement. Rhenium-molybdenum alloys are superconducting.,65.0,0.15,[Xe] 4f14 5d5 6s2,704.0,34.0,7.0,2.76,HEX,186.207,3453.0,Rhenium,6.0,8.0,0.138,48.0,216.0,151.0,131.0,1.9,9.46,#267dab,#ff1493,,,774.0,,,135.0,,,,205.0,,295.4,237.0,0.0007,4e-06,1.59,8.0,1.073,#267dab,1.59
 Os,,76.0,135.0,8.43,d,5300.0,22.57,Hard blue-white metallic transition element. Found with platinum and used in some alloys with platinum and iridium.,57.0,1.1,[Xe] 4f14 5d6 6s2,738.0,31.7,8.0,2.74,HEX,190.23,3327.0,Osmium,6.0,8.0,0.131,,216.0,144.0,129.0,2.2,9.78,#266696,#ff1493,,,787.0,,,130.0,,,,200.0,,312.0,235.0,0.0015,,1.28,8.0,1.08,#266696,1.28
 Ir,,77.0,136.0,8.54,d,4403.0,22.42,"Very hard and brittle, silvery metallic transition element. It has a yellowish cast to it. Salts of iridium are highly colored. It is the most corrosion resistant metal known, not attacked by any acid, but is attacked by molten salts. There are two natural isotopes of iridium, and 4 radioisotopes, the most stable being Ir-192 with a half-life of 73.83 days. Ir-192 decays into Platinum, while the other radioisotopes decay into Osmium. Iridium is used in high temperature apparatus, electrical contacts, and as a hardening agent for platinumpy. Discovered in 1803 by Smithson Tennant in England. The name comes from the Greek word iris, which means rainbow. Iridium metal is generally non-toxic due to its relative unreactivity, but iridium compounds should be considered highly toxic.",51.0,1.5638,[Xe] 4f14 5d7 6s2,604.0,27.61,9.0,3.84,FCC,192.22,2683.0,Iridium,6.0,8.0,0.133,147.0,213.0,141.0,122.0,2.2,9.96,#175487,#ff1493,,,669.0,,,135.0,,,,200.0,,284.0,236.0,0.001,,1.37,8.0,1.083,#175487,1.37
-Pt,,78.0,139.0,9.1,d,4100.0,21.45,"Attractive greyish-white metal. When pure, it is malleable and ductile. Does not oxidize in air, insoluble in hydrochloric and nitric acid. Corroded by halogens, cyandies, sulphur and alkalis. Hydrogen and Oxygen react explosively in the presence of platinumpy. There are six stable isotopes and three radioisotopes, the most stable being Pt-193 with a half-life of 60 years. Platinum is used in jewelry, laboratory equipment, electrical contacts, dentistry, and anti-pollution devices in cars. PtCl2(NH3)2 is used to treat some forms of cancer. Platinum-Cobalt alloys have magnetic properties. It is also used in the definition of the Standard Hydrogen Electrode. Discovered by Antonio de Ulloa in South America in 1735. The name comes from the Spanish word platina which means silver. Platinum metal is generally not a health concern due to its unreactivity, however platinum compounds should be considered highly toxic.",44.0,2.128,[Xe] 4f14 5d9 6s,470.0,21.76,10.0,3.92,FCC,195.08,2045.0,Platinum,6.0,8.0,0.133,71.6,213.0,136.0,123.0,2.2,10.16,#d0d0e0,#ff1493,,,565.7,,,135.0,,,,205.0,,275.4,239.0,0.005,,1.28,8.0,1.088,#d0d0e0,1.28
+Pt,,78.0,139.0,9.1,d,4100.0,21.45,"Attractive greyish-white metal. When pure, it is malleable and ductile. Does not oxidize in air, insoluble in hydrochloric and nitric acid. Corroded by halogens, cyandies, sulphur and alkalis. Hydrogen and Oxygen react explosively in the presence of platinumpy. There are six stable isotopes and three radioisotopes, the most stable being Pt-193 with a half-life of 60 years. Platinum is used in jewelry, laboratory equipment, electrical contacts, dentistry, and anti-pollution devices in cars. PtCl2(NH3)2 is used to treat some forms of cancer. Platinum-Cobalt alloys have magnetic properties. It is also used in the definition of the Standard Hydrogen Electrode. Discovered by Antonio de Ulloa in South America in 1735. The name comes from the Spanish word platina which means silver. Platinum metal is generally not a health concern due to its unreactivity, however platinum compounds should be considered highly toxic.",44.0,2.128,[Xe] 4f14 5d9 6s,470.0,21.76,10.0,3.92,FCC,195.08,2045.0,Platinum,6.0,8.0,0.133,71.6,213.0,136.0,123.0,2.2,10.16,#d0d0e0,#ff1493,,,565.7,,,135.0,,,,205.0,,275.4,239.0,0.005,,1.28,8.0,1.088,#d0d0e0,1.33
 Au,,79.0,146.0,10.2,d,3080.0,19.3,"Gold is gold colored. It is the most malleable and ductile metal known. There is only one stable isotope of gold, and five radioisotopes of gold, Au-195 being the most stable with a half-life of 186 days. Gold is used as a monetary standard, in jewelry, dentistry, electronics. Au-198 is used in treating cancer and some other medical conditions. Gold has been known to exist as far back as 2600 BC. Gold comes from the Anglo-Saxon word gold. Its symbol, Au, comes from the Latin word aurum, which means gold. Gold is not particularly toxic, however it is known to cause damage to the liver and kidneys in some.",36.1,2.30863,[Xe] 4f14 5d10 6s,340.0,12.68,11.0,4.08,FCC,196.96654,1337.58,Gold,6.0,8.0,0.129,318.0,214.0,136.0,124.0,2.4,11.33,#ffd123,#daa520,,,368.2,,,135.0,,,,210.0,,329.3,243.00000000000003,0.004,4e-06,1.44,8.0,1.091,#ffd123,1.44
 Hg,"density(@ +20C), ",80.0,157.0,14.8,d,629.73,13.546,"Heavy silvery liquid metallic element, belongs to the zinc group. Used in thermometers, barometers and other scientific apparatus. Less reactive than zinc and cadmium, does not displace hydrogen from acids. Forms a number of complexes and organomercury compounds.",33.91,,[Xe] 4f14 5d10 6s2,58.5,2.295,12.0,2.99,RHL,200.59,234.28,Mercury,6.0,8.0,0.138,8.3,223.0,132.0,133.0,1.9,10.44,#b8b8d0,#ff1493,,,61.38,,,150.0,,,,205.0,,270.5,253.0,0.085,2.9999999999999997e-05,1.49,8.0,1.097,#b8b8d0,1.49
 Tl,,81.0,171.0,17.2,p,1730.0,11.85,"Pure, unreacted thallium appears silvery-white and exhibits a metallic lustre. Upon reacting with air, it begins to turn bluish-grey and looks like lead. It is very malleable, and can be cut with a knife. There are two stable isotopes, and four radioisotopes, Tl-204 being the most stable with a half-life of 3.78 years. Thallium sulphate was used as a rodenticide. Thallium sulphine's conductivity changes with exposure to infrared light, this gives it a use in infrared detectors. Discovered by Sir William Crookes via spectroscopy. Its name comes from the Greek word thallos, which means green twig. Thallium and its compounds are toxic and can cause cancer.",51.7,0.377,[Xe] 4f14 5d10 6s2 6p,162.4,4.31,13.0,3.46,HEX,204.3833,576.6,Thallium,6.0,7.0,0.128,46.1,196.0,145.0,144.0,1.8,,#a6544d,#ff1493,,,182.2,,190.0,190.0,196.0,,,220.00000000000003,,434.69999999999993,259.0,0.85,1.9e-05,1.48,8.0,1.103,#a6544d,1.48
 Pb,,82.0,175.0,18.3,p,2013.0,11.35,"Heavy dull grey ductile metallic element, belongs to group 14. Used in building construction, lead-place accumulators, bullets and shot, and is part of solder, pewter, bearing metals, type metals and fusible alloys.",47.1,0.364,[Xe] 4f14 5d10 6s2 6p2,177.8,4.77,14.0,4.95,FCC,207.2,600.65,Lead,6.0,7.0,0.159,35.3,202.0,146.0,144.0,1.8,10.97,#575961,#ff1493,,,195.2,,,,202.0,,,230.0,,429.7,274.0,14.0,2.9999999999999997e-05,1.47,8.0,1.107,#575961,1.47
 Bi,,83.0,170.0,21.3,p,1883.0,9.747,"White crystalline metal with a pink tinge, belongs to group 15. Most diamagnetic of all metals and has the lowest thermal conductivity of all the elements except mercury. Lead-free bismuth compounds are used in cosmetics and medical procedures. Burns in the air and produces a blue flame. In 1753, C.G. Junine first demonstrated that it was different from lead.",50.0,0.942362,[Xe] 4f14 5d10 6s2 6p3,172.0,11.0,15.0,4.75,RHL,208.98037,544.5,Bismuth,6.0,7.0,0.124,7.9,207.0,148.0,151.0,1.9,11.9,#9e4fb5,#ff1493,,,209.6,,148.0,160.0,,207.0,,230.0,,437.0,266.0,0.0085,2e-05,1.46,8.0,1.109,#9e4fb5,1.46
 Po,,84.0,176.0,22.7,p,1235.0,9.32,"Rare radioactive metallic element, belongs to group 16 of the periodic table. Over 30 known isotopes exist, the most of all elements. Po-209 has a half-life of 103 years. Possible uses in heating spacecraft. Discovered by Marie Curie in 1898 in a sample of pitchblende.",46.0,1.9,[Xe] 4f14 5d10 6s2 6p4,102.9,10.0,16.0,3.35,SC,208.9824,527.0,Polonium,6.0,5.0,0.125,,197.0,140.0,145.0,2.0,13.0,#ab5c00,#ff1493,,,,,,190.0,,197.0,,,,470.9,259.0,2e-10,1.5e-14,1.9,8.0,1.111,#ab5c00,1.9
 At,,85.0,,,p,610.0,,"Radioactive halogen element. Occurs naturally from uranium and thorium decay. At least 20 known isotopes. At-210, the most stable, has a half-life of 8.3 hours. Synthesized by nuclear bombardment in 1940 by D.R. Corson, K.R. MacKenzie and E. Segre at the University of California.",43.0,2.8,[Xe] 4f14 5d10 6s2 6p5,,,17.0,,,209.9871,575.0,Astatine,6.0,6.0,,,202.0,150.0,147.0,2.2,14.1,#754f45,#ff1493,,,,,,,,202.0,,,,475.0,251.0,,,1.9,8.0,1.111,#754f45,1.9
```

### Comparing `chemcoord-2.0.5/src/chemcoord/exceptions.py` & `chemcoord-2.1.0/src/chemcoord/exceptions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/internal_coordinates/_indexers.py` & `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_indexers.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_class_core.py` & `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,30 @@
     def __getitem__(self, key):
         if isinstance(key, tuple):
             selected = self._frame[key[0], key[1]]
         else:
             selected = self._frame[key]
         return selected
 
+    def __getattr__(self, name: str):
+        """
+        After regular attribute access, try looking up the name
+        This allows simpler access to columns for interactive use.
+        """
+        # Note: obj.x will always call obj.__getattribute__('x') prior to
+        # calling obj.__getattr__('x').
+
+        if name.startswith('__'):
+            # See here, why we do this
+            # https://stackoverflow.com/questions/47299243/recursionerror-when-python-copy-deepcopy
+            raise AttributeError()
+        if (name in self._frame.columns):
+            return self[name]
+        return object.__getattribute__(self, name)
+
     @property
     @append_indexer_docstring
     def loc(self):
         """Label based indexing for obtaining elements.
         """
         return indexers._Loc(self)
 
@@ -417,15 +433,15 @@
                 return x
             return subs_function
 
         for col in cols:
             if out.loc[:, col].dtype is np.dtype('O'):
                 out.unsafe_loc[:, col] = out.loc[:, col].map(get_subs_f(*args))
                 try:
-                    out.unsafe_loc[:, col] = out.loc[:, col].astype('f8')
+                    out._frame[col] = out.loc[:, col].astype('f8')
                 except (SystemError, TypeError):
                     pass
         if perform_checks:
             try:
                 new_cartesian = out.get_cartesian()
             except (AttributeError, TypeError):
                 # Unevaluated symbolic expressions are remaining.
```

### Comparing `chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_class_io.py` & `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if format_as != 'raw':
             out._frame.replace(
                 to_replace={col: rename for col in ['b', 'a', 'd']},
                 inplace=True)
         return out
 
     def _repr_html_(self):
-        out = self._sympy_formatter()._abs_ref_formatter(format_as='latex')
+        out = self._sympy_formatter()._abs_ref_formatter(format_as='string')
 
         def insert_before_substring(insert_txt, substr, txt):
             """Under the assumption that substr only appears once.
             """
             return (insert_txt + substr).join(txt.split(substr))
         html_txt = out._frame._repr_html_()
         insert_txt = '<caption>{}</caption>\n'.format(self.__class__.__name__)
```

### Comparing `chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py` & `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/internal_coordinates/_zmat_transformation.py` & `chemcoord-2.1.0/src/chemcoord/internal_coordinates/_zmat_transformation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # -*- coding: utf-8 -*-
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals, with_statement)
+
+
 import numba as nb
 import numpy as np
 from numpy import sin, cos, cross
 from numpy.linalg import inv
 from numba import jit
 
 import chemcoord.constants as constants
@@ -53,45 +57,75 @@
 def get_X(C, c_table):
     X = np.empty_like(C)
     n_atoms = X.shape[1]
     for j in range(n_atoms):
         err, B = get_B(X, c_table, j)
         if err == ERR_CODE_InvalidReference:
             return (err, j, X)
-        X[:, j] = (np.dot(B, get_S(C, j))
-                   + get_ref_pos(X, c_table[0, j]))
+        X[:, j] = B @ get_S(C, j) + get_ref_pos(X, c_table[0, j])
     return (ERR_CODE_OK, j, X)  # pylint:disable=undefined-loop-variable
 
 
 @jit(nopython=True, cache=True)
 def chain_grad(X, grad_X, C, c_table, j, l):
+    """Chain the gradients.
+
+    Args:
+        X (:class:`numpy.ndarray`): A ``3 * n`` numpy array.
+            ``X[i, j]`` is the i-th cartesian coordinate of the
+            j-th atom.
+
+        grad_X (:class:`numpy.ndarray`): A ``3, n, n, 3`` numpy array.
+            ``grad_X[i, j, l, k]`` is the derivative of the
+            i-th cartesian coordinate of the j-th atom
+            after the k-th Z-matrix coordinate of the l-th atom.
+
+        C (:class:`numpy.ndarray`): A ``3 * n`` numpy array.
+            ``C[k, l]`` is the k-th Z-matrix coordinate of the
+            l-th atom.
+
+        c_table (:class:`numpy.ndarray`): A ``3 * n`` numpy array.
+            ``c_table[i, j]`` is the i-th reference atom of the
+            j-th atom. They are given in the order ``'b', 'a', 'd'``.
+
+        j (int): The index of the atom in cartesian coordinates, whose
+            position we are deriving.
+
+        l (int): The index of the atom in Z-matrix coordinates,
+            after which we are deriving.
+            Note that ``l < j``.
+    Returns:
+        Zmat: A new zmat instance.
+    """
     if j < constants.keys_below_are_abs_refs:
         new_grad_X = np.zeros((3, 3))
     else:
         grad_B = get_grad_B(X, c_table, j)
         S = get_S(C, j)
-        new_grad_X = grad_X[:, c_table[0, j], l, :].copy()
+        new_grad_X = np.zeros((3, 3))
+
+        assert l < j
+        for k in range(3):
+            change_of_B = np.zeros((3, 3))
+            for m2 in range(3):
+                if c_table[m2, j] > constants.keys_below_are_abs_refs:
+                    for m1 in range(3):
+                        change_of_B += (grad_B[:, :, m2, m1] * grad_X[m1, c_table[m2, j], l, k])
 
-        for m_2 in range(3):
-            for m_1 in range(3):
-                for k in range(3):
-                    if c_table[k, j] > constants.keys_below_are_abs_refs:
-                        new_grad_X += (S[m_2]
-                                       * grad_B[:, m_2, k, m_1]
-                                       * grad_X[m_1, c_table[k, j], l, :])
+            new_grad_X[:, k] = change_of_B @ S + grad_X[:, c_table[0, j], l, k]
     return new_grad_X
 
 
 @jit(nopython=True, cache=True)
 def get_grad_X(C, c_table, chain=True):
     n_atoms = C.shape[1]
     grad_X = np.zeros((3, n_atoms, n_atoms, 3))
     X = get_X(C, c_table)[2]
     for j in range(n_atoms):
-        grad_X[:, j, j, :] = np.dot(get_B(X, c_table, j)[1], get_grad_S(C, j))
+        grad_X[:, j, j, :] = get_B(X, c_table, j)[1] @ get_grad_S(C, j)
         if chain:
             for l in range(j):
                 grad_X[:, j, l, :] = chain_grad(X, grad_X, C, c_table, j, l)
     return grad_X
 
 
 @jit(nopython=True, cache=True)
```

### Comparing `chemcoord-2.0.5/src/chemcoord/internal_coordinates/zmat_class_main.py` & `chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_class_main.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/internal_coordinates/zmat_functions.py` & `chemcoord-2.1.0/src/chemcoord/internal_coordinates/zmat_functions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/utilities/_decorators.py` & `chemcoord-2.1.0/src/chemcoord/utilities/_decorators.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord/utilities/_print_versions.py` & `chemcoord-2.1.0/src/chemcoord/utilities/_print_versions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.0.5/src/chemcoord.egg-info/PKG-INFO` & `chemcoord-2.1.0/src/chemcoord.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemcoord
-Version: 2.0.5
+Version: 2.1.0
 Summary: Python module for dealing with chemical coordinates.
 Home-page: https://github.com/mcocdawc/chemcoord
 Author: Oskar Weser
 Author-email: oskar.weser@gmail.com
 License: LGPLv3
 Keywords: chemcoord,transformation,cartesian,internal,chemistry,zmatrix,xyz,zmat,coordinates,coordinate system
 Platform: UNKNOWN
@@ -52,40 +52,39 @@
      - .. image:: https://codecov.io/gh/mcocdawc/chemcoord/branch/master/graph/badge.svg
             :target: https://codecov.io/gh/mcocdawc/chemcoord
 
 
 Website
 -------
 
-The project’s website with documentation is:
+The project's website with documentation is:
 http://chemcoord.readthedocs.org/
 
 Features
 --------
 
 -  Molecules are reliably transformed between cartesian space and non
    redundant internal coordinates (Zmatrices). Dummy atoms are inserted
    and removed automatically on the fly if necessary.
 -  The created Zmatrix is not only a structure expressed in internal
-   coordinates, it is a “chemical” Zmatrix. “Chemical” Zmatrix means,
-   that e.g. distances are along bonds or dihedrals are defined as they
+   coordinates, it is a "chemical" Zmatrix. "Chemical" Zmatrix means,
+   that e.g. distances are along bonds or dihedrals are defined as they
    are drawn in chemical textbooks (Newman projections).
 -  Analytical gradients for the transformations between the different
    coordinate systems are implemented.
 -  Performance intensive functions/methods are implemented with
    Fortran/C like speed using `numba <http://numba.pydata.org/>`__.
 -  Geometries may be defined with symbolic expressions using
    `sympy <http://www.sympy.org/en/index.html>`__.
 -  Built on top of `pandas <http://pandas.pydata.org/>`__ with very
    similar syntax. This allows for example distinct label or row based
    indexing.
 -  It derived from my own work and I heavily use it during the day. So
    all functions are tested and tailored around the work flow in
    theoretical chemistry.
--  The classes are safe to inherit from and can easily be customized.
 -  `It as a python module ;) <https://xkcd.com/353/>`__
 
 Installation guide
 ------------------
 
 A working python 3 installation is required (>=3.7 are possible).
 
@@ -93,25 +92,19 @@
 `Ipython <http://ipython.org/>`__ and `jupyter <http://jupyter.org/>`__.
 They come shipped by default with the `anaconda3
 installer <https://www.continuum.io/downloads/>`__
 
 Unix
 ~~~~
 
-For the packaged versions, the following commands have to be executed in
+For the packaged version, the following commands have to be executed in
 the terminal:
 
 ::
 
-   conda install -c mcocdawc chemcoord
-
-or
-
-::
-
    pip install chemcoord
 
 For the up to date development version (experimental):
 
 ::
 
    git clone https://github.com/mcocdawc/chemcoord.git
@@ -121,24 +114,49 @@
 Windows
 ~~~~~~~
 
 Neither installation nor running the module are tested on windows. To
 the best of my knowledge it should work there as well. Just use the same
 steps as for UNIX.
 
-Changelog
-~~~~~~~~~
-
-The changelog can be found
-`here <https://github.com/mcocdawc/chemcoord/blob/master/CHANGELOG.md>`__.
 
 Citation and mathematical background
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If chemcoord is used in a project that leads to a scientific
-publication, please acknowledge this fact by citing `this preprint <https://chemrxiv.org/engage/chemrxiv/article-details/615c0ae97d3da5630aed6dc0>`__.
+The theory behind chemcoord is described in `this paper <https://onlinelibrary.wiley.com/doi/full/10.1002/jcc.27029>`__.
+If this package is used in a project that leads to a scientific
+publication, please acknowledge it by citing.
+
+::
+
+    @article{https://doi.org/10.1002/jcc.27029,
+        author = {Weser, Oskar and Hein-Janke, Björn and Mata, Ricardo A.},
+        title = {Automated handling of complex chemical structures in Z-matrix coordinates—The chemcoord library},
+        journal = {Journal of Computational Chemistry},
+        volume = {44},
+        number = {5},
+        pages = {710-726},
+        keywords = {analytical gradients, geometry optimization, non-linear constraints, transition state search, Z-matrix},
+        doi = {10.1002/jcc.27029},
+        year = {2023}
+    }
 
-My (Oskar Weser) master thesis including the derivation of implemented equations and
+
+My (Oskar Weser) master thesis including a more detailed derivation of implemented equations and
 the mathematical background can be found
 `here <https://github.com/mcocdawc/chemcoord/blob/master/docs/source/files/master_thesis_oskar_weser_chemcoord.pdf>`__.
 
 
+
+Acknowledgement
+~~~~~~~~~~~~~~~
+
+
+.. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
+   :width: 80
+   :align: left
+   :target: https://zulip.com/
+
+Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
+that supports the development of chemcoord with a free plan.
+
+
```

### Comparing `chemcoord-2.0.5/src/chemcoord.egg-info/SOURCES.txt` & `chemcoord-2.1.0/src/chemcoord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

