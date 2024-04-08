# Comparing `tmp/ms2rescore_rs-0.1.0.tar.gz` & `tmp/ms2rescore_rs-0.2.0.tar.gz`

## Comparing `ms2rescore_rs-0.1.0.tar` & `ms2rescore_rs-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 ms2rescore_rs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     2767 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/.github/workflows/release.yml
--rw-r--r--   0     1001      127      852 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127      453 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/.gitignore
--rw-r--r--   0     1001      127    11357 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/LICENSE
--rw-r--r--   0     1001      127       63 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/README.md
--rw-r--r--   0     1001      127     1281 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/src/file_types.rs
--rw-r--r--   0     1001      127     1309 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     5499 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/src/parse_mzdata.rs
--rw-r--r--   0     1001      127     1165 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/src/parse_timsrust.rs
--rw-r--r--   0     1001      127      671 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/src/precursor.rs
--rw-r--r--   0     1001      127      389 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/README.md
--rw-r--r--   0     1001      127    20480 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/data/dda_test.d/analysis.tdf
--rw-r--r--   0     1001      127      377 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/data/dda_test.d/analysis.tdf_bin
--rw-r--r--   0     1001      127      183 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/data/test.mgf
--rw-r--r--   0     1001      127     3054 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/data/test.ms2/converter.GlobalMetaData.ms2.parquet
--rw-r--r--   0     1001      127       99 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/data/test.ms2/converter.ms2spectrum.bin
--rw-r--r--   0     1001      127    10560 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/data/test.ms2/converter.ms2spectrum.parquet
--rw-r--r--   0     1001      127   316728 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/data/test.mzML
--rw-r--r--   0     1001      127     1369 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/tests/test.py
--rw-r--r--   0     1001      127    41052 2024-04-05 15:06:27.000000 ms2rescore_rs-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      445 2024-04-05 15:06:21.000000 ms2rescore_rs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 ms2rescore_rs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 ms2rescore_rs-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     2767 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      852 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      453 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/LICENSE
+-rw-r--r--   0     1001      127       63 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/README.md
+-rw-r--r--   0     1001      127     1281 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/src/file_types.rs
+-rw-r--r--   0     1001      127     2256 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127      781 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/src/ms2_spectrum.rs
+-rw-r--r--   0     1001      127     6909 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/src/parse_mzdata.rs
+-rw-r--r--   0     1001      127     2203 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/src/parse_timsrust.rs
+-rw-r--r--   0     1001      127      678 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/src/precursor.rs
+-rw-r--r--   0     1001      127      389 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/README.md
+-rw-r--r--   0     1001      127    20480 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/data/dda_test.d/analysis.tdf
+-rw-r--r--   0     1001      127      377 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/data/dda_test.d/analysis.tdf_bin
+-rw-r--r--   0     1001      127      183 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/data/test.mgf
+-rw-r--r--   0     1001      127     3054 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/data/test.ms2/converter.GlobalMetaData.ms2.parquet
+-rw-r--r--   0     1001      127       99 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/data/test.ms2/converter.ms2spectrum.bin
+-rw-r--r--   0     1001      127    10560 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/data/test.ms2/converter.ms2spectrum.parquet
+-rw-r--r--   0     1001      127   316728 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/data/test.mzML
+-rw-r--r--   0     1001      127     1369 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/tests/test.py
+-rw-r--r--   0     1001      127    41052 2024-04-08 13:54:16.000000 ms2rescore_rs-0.2.0/Cargo.lock
+-rw-r--r--   0     1001      127      445 2024-04-08 13:54:11.000000 ms2rescore_rs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 ms2rescore_rs-0.2.0/PKG-INFO
```

### Comparing `ms2rescore_rs-0.1.0/.github/workflows/release.yml` & `ms2rescore_rs-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/.github/workflows/test.yml` & `ms2rescore_rs-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/LICENSE` & `ms2rescore_rs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/src/file_types.rs` & `ms2rescore_rs-0.2.0/src/file_types.rs`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/src/lib.rs` & `ms2rescore_rs-0.2.0/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 mod file_types;
 mod parse_mzdata;
 mod parse_timsrust;
 mod precursor;
+mod ms2_spectrum;
 
 use std::collections::HashMap;
 
 use pyo3::exceptions::PyOSError;
 use pyo3::prelude::*;
 
 use file_types::{match_file_type, SpectrumFileType};
 use precursor::Precursor;
+use ms2_spectrum::MS2Spectrum;
 
 /// Get mapping of spectrum identifiers to precursor information.
 #[pyfunction]
 pub fn get_precursor_info(spectrum_path: String) -> PyResult<HashMap<String, Precursor>> {
     let file_type = match_file_type(&spectrum_path);
 
     let precursors = match file_type {
@@ -27,15 +29,37 @@
 
     match precursors {
         Ok(precursors) => Ok(precursors),
         Err(e) => Err(PyOSError::new_err(e.to_string())),
     }
 }
 
+/// Get MS2 spectra from a spectrum file.
+#[pyfunction]
+pub fn get_ms2_spectra(spectrum_path: String) -> PyResult<Vec<ms2_spectrum::MS2Spectrum>> {
+    let file_type = match_file_type(&spectrum_path);
+
+    let spectra = match file_type {
+        SpectrumFileType::MascotGenericFormat | SpectrumFileType::MzML => {
+            parse_mzdata::read_ms2_spectra(&spectrum_path, file_type)
+        }
+        SpectrumFileType::BrukerRaw => parse_timsrust::read_ms2_spectra(&spectrum_path),
+        // SpectrumFileType::ThermoRaw => parse_with_mzdata_thermo(&spectrum_path, file_type),
+        SpectrumFileType::Unknown => return Err(PyOSError::new_err("Unsupported file type")),
+    };
+
+    match spectra {
+        Ok(spectra) => Ok(spectra),
+        Err(e) => Err(PyOSError::new_err(e.to_string())),
+    }
+}
+
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn ms2rescore_rs(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<Precursor>()?;
+    m.add_class::<MS2Spectrum>()?;
     m.add_function(wrap_pyfunction!(get_precursor_info, m)?)?;
+    m.add_function(wrap_pyfunction!(get_ms2_spectra, m)?)?;
     Ok(())
 }
```

### Comparing `ms2rescore_rs-0.1.0/src/parse_mzdata.rs` & `ms2rescore_rs-0.2.0/src/parse_mzdata.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,108 @@
 use std::collections::HashMap;
 use std::fs::File;
 
 use mzdata::io::{MGFReader, MzMLReader};
 
 use crate::file_types::SpectrumFileType;
+use crate::ms2_spectrum::MS2Spectrum;
 use crate::precursor::Precursor;
 
-impl From<mzdata::spectrum::MultiLayerSpectrum> for Precursor {
-    fn from(spectrum: mzdata::spectrum::MultiLayerSpectrum) -> Self {
+impl From<&mzdata::spectrum::MultiLayerSpectrum> for Precursor {
+    fn from(spectrum: &mzdata::spectrum::MultiLayerSpectrum) -> Self {
         let precursor = &spectrum.description.precursor;
         match precursor {
             Some(precursor) => Precursor {
                 mz: precursor.ions[0].mz,
                 rt: spectrum
                     .description
                     .acquisition
                     .first_scan()
                     .map(|s| s.start_time)
                     .unwrap_or(0.0),
-                im: get_im_from_spectrum_description(&spectrum)
-                    .or(get_im_from_selected_ion(&spectrum))
-                    .or(get_im_from_first_scan(&spectrum))
+                im: get_im_from_spectrum_description(spectrum)
+                    .or(get_im_from_selected_ion(spectrum))
+                    .or(get_im_from_first_scan(spectrum))
                     .unwrap_or(0.0),
-                charge: get_charge_from_spectrum(&spectrum).unwrap_or(0),
+                charge: get_charge_from_spectrum(spectrum).unwrap_or(0),
                 intensity: precursor.ions[0].intensity as f64,
             },
             None => Precursor::default(),
         }
     }
 }
 
+impl From<mzdata::spectrum::MultiLayerSpectrum> for MS2Spectrum {
+    fn from(spectrum: mzdata::spectrum::MultiLayerSpectrum) -> Self {
+        let identifier: String = spectrum.description.id.to_string();
+        let precursor = Precursor::from(&spectrum);
+        let mzdata_centroid_spectrum = spectrum.into_centroid().unwrap();
+        let (mz, intensity): (Vec<f32>, Vec<f32>) = mzdata_centroid_spectrum
+            .peaks
+            .iter()
+            .map(|peak| (peak.mz as f32, peak.intensity))
+            .unzip();
+
+        MS2Spectrum::new(identifier, mz, intensity, Some(precursor))
+    }
+}
+
 /// Parse precursor info from spectrum files with mzdata
 pub fn parse_precursor_info(
     spectrum_path: &str,
     file_type: SpectrumFileType,
 ) -> Result<HashMap<String, Precursor>, std::io::Error> {
     let file = File::open(spectrum_path)?;
     match file_type {
         SpectrumFileType::MascotGenericFormat => Ok(MGFReader::new(file)
             .filter_map(|spectrum| {
                 spectrum.description.precursor.as_ref()?;
-                Some((spectrum.description.id.clone(), Precursor::from(spectrum)))
+                Some((spectrum.description.id.clone(), Precursor::from(&spectrum)))
             })
             .collect::<HashMap<String, Precursor>>()),
 
         SpectrumFileType::MzML => Ok(MzMLReader::new(file)
             .filter_map(|spectrum| {
                 if spectrum.description.ms_level != 2 {
                     return None;
                 }
                 spectrum.description.precursor.as_ref()?;
-                Some((spectrum.description.id.clone(), Precursor::from(spectrum)))
+                Some((spectrum.description.id.clone(), Precursor::from(&spectrum)))
             })
             .collect::<HashMap<String, Precursor>>()),
 
         _ => Err(std::io::Error::new(
             std::io::ErrorKind::InvalidInput,
             "Unsupported file type for mzdata",
         )),
     }
 }
+
+/// Read MS2 spectra from spectrum files with mzdata
+pub fn read_ms2_spectra(
+    spectrum_path: &str,
+    file_type: SpectrumFileType,
+) -> Result<Vec<MS2Spectrum>, std::io::Error> {
+    let file = File::open(spectrum_path)?;
+    match file_type {
+        SpectrumFileType::MascotGenericFormat => Ok(MGFReader::new(file)
+            .map(MS2Spectrum::from)
+            .collect::<Vec<MS2Spectrum>>()),
+
+        SpectrumFileType::MzML => Ok(MzMLReader::new(file)
+            .filter(|spectrum| spectrum.description.ms_level == 2)
+            .map(MS2Spectrum::from)
+            .collect::<Vec<MS2Spectrum>>()),
+
+        _ => Err(std::io::Error::new(
+            std::io::ErrorKind::InvalidInput,
+            "Unsupported file type for mzdata",
+        )),
+    }
+}
 
 // pub fn parse_precursor_info_thermo(
 //     spectrum_path: &str,
 //     file_type: SpectrumFileType,
 // ) -> Result<HashMap<String, Precursor>, std::io::Error> {
 //     let reader = mzdata::io::ThermoRawReader::open_path(spectrum_path)?;
 //     Ok(reader
```

### Comparing `ms2rescore_rs-0.1.0/src/parse_timsrust.rs` & `ms2rescore_rs-0.2.0/src/parse_timsrust.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 use std::collections::HashMap;
 
+use crate::ms2_spectrum::MS2Spectrum;
 use crate::precursor::Precursor;
 
 impl From<timsrust::Precursor> for Precursor {
     fn from(precursor: timsrust::Precursor) -> Self {
         Precursor {
             mz: precursor.mz,
             rt: precursor.rt,
             im: precursor.im,
             charge: precursor.charge,
             intensity: precursor.intensity,
         }
     }
 }
 
+impl From<timsrust::Spectrum> for MS2Spectrum {
+    fn from(spectrum: timsrust::Spectrum) -> Self {
+        MS2Spectrum::new(
+            spectrum.index.to_string(),
+            spectrum.mz_values.iter().map(|mz| *mz as f32).collect(),
+            spectrum
+                .intensities
+                .iter()
+                .map(|intensity| *intensity as f32)
+                .collect(),
+            match spectrum.precursor {
+                timsrust::QuadrupoleEvent::Precursor(precursor) => Some(Precursor::from(precursor)),
+                _ => None,
+            },
+        )
+    }
+}
+
 /// Parse precursor info from spectrum files with timsrust
 pub fn parse_precursor_info(
     spectrum_path: &str,
 ) -> Result<HashMap<String, Precursor>, std::io::Error> {
     let reader = timsrust::FileReader::new(spectrum_path)
         .map_err(|e| std::io::Error::new(std::io::ErrorKind::Other, e.to_string()))?;
 
@@ -34,7 +53,19 @@
             (
                 spectrum.index.to_string(),
                 Precursor::from(spectrum.precursor.unwrap_as_precursor()),
             )
         })
         .collect::<HashMap<String, Precursor>>())
 }
+
+/// Read MS2 spectra from spectrum files with timsrust
+pub fn read_ms2_spectra(spectrum_path: &str) -> Result<Vec<MS2Spectrum>, std::io::Error> {
+    let reader = timsrust::FileReader::new(spectrum_path)
+        .map_err(|e| std::io::Error::new(std::io::ErrorKind::Other, e.to_string()))?;
+
+    Ok(reader
+        .read_all_spectra()
+        .into_iter()
+        .map(MS2Spectrum::from)
+        .collect())
+}
```

### Comparing `ms2rescore_rs-0.1.0/src/precursor.rs` & `ms2rescore_rs-0.2.0/src/precursor.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use pyo3::prelude::*;
 
 /// Precursor information.
 #[pyclass(get_all, set_all)]
-#[derive(Debug)]
+#[derive(Debug, Clone)]
 pub struct Precursor {
     pub mz: f64,
     pub rt: f64,
     pub im: f64,
     pub charge: usize,
     pub intensity: f64,
 }
```

### Comparing `ms2rescore_rs-0.1.0/tests/data/dda_test.d/analysis.tdf` & `ms2rescore_rs-0.2.0/tests/data/dda_test.d/analysis.tdf`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/tests/data/test.ms2/converter.GlobalMetaData.ms2.parquet` & `ms2rescore_rs-0.2.0/tests/data/test.ms2/converter.GlobalMetaData.ms2.parquet`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/tests/data/test.ms2/converter.ms2spectrum.parquet` & `ms2rescore_rs-0.2.0/tests/data/test.ms2/converter.ms2spectrum.parquet`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/tests/data/test.mzML` & `ms2rescore_rs-0.2.0/tests/data/test.mzML`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/tests/test.py` & `ms2rescore_rs-0.2.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `ms2rescore_rs-0.1.0/Cargo.lock` & `ms2rescore_rs-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -247,17 +247,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "1fd97381a8cc6493395a5afc4c691c1084b3768db713b73aa215217aa245d153"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
@@ -445,28 +445,28 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
@@ -753,15 +753,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "ms2rescore-rs"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "mzdata",
  "pyo3",
  "timsrust",
 ]
 
 [[package]]
```

