# Comparing `tmp/noisepy_seis-0.9.3.tar.gz` & `tmp/noisepy_seis-0.9.4.tar.gz`

## Comparing `noisepy_seis-0.9.3.tar` & `noisepy_seis-0.9.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35007 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/pnwstore.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/scheduler.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/LICENSE
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/README.md
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/pyproject.toml
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 noisepy_seis-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35007 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/pnwstore.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/zarrstore.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/LICENSE
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/README.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    10601 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/PKG-INFO
```

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.9.4/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.9.4/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.9.4/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,19 @@
             not all(map(lambda c: c.station.valid(), all_channels)),
             "The stations don't have their lat/lon/elev properties populated. Problem with the ChannelCatalog used?",
         )
 
         tlog.log("get channels")
         ch_data_tuples = _read_channels(executor, ts, raw_store, all_channels, fft_params.samp_freq)
         # only the channels we are using
+
+        if len(ch_data_tuples) == 0:
+            logger.warning(f"No data available for {ts}")
+            continue
+
         channels = list(zip(*ch_data_tuples))[0]
         tlog.log("read channel data")
 
         ch_data_tuples = preprocess_all(executor, ch_data_tuples, raw_store, fft_params, ts)
         tlog.log("preprocess")
 
         nchannels = len(ch_data_tuples)
@@ -287,16 +292,20 @@
     return _filter_channel_data(tuples, samp_freq)
 
 
 def _filter_channel_data(
     tuples: List[Tuple[Channel, ChannelData]], samp_freq: int
 ) -> List[Tuple[Channel, ChannelData]]:
     frequencies = set(t[1].sampling_rate for t in tuples)
+    frequencies = list(filter(lambda f: f >= samp_freq, frequencies))
+    if len(frequencies) == 0:
+        logging.warning(f"No data available with sampling frequency >= {samp_freq}")
+        return []
     closest_freq = min(
-        filter(lambda f: f >= samp_freq, frequencies),
+        frequencies,
         key=lambda f: max(f - samp_freq, 0),
     )
     filtered_tuples = list(filter(lambda tup: tup[1].sampling_rate == closest_freq, tuples))
     logger.info(
         f"Picked {closest_freq} as the closest sampling frequence to {samp_freq}. "
         f"Filtered to {len(filtered_tuples)}/{len(tuples)} channels"
     )
```

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.9.4/src/noisepy/seis/S2_stacking.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     rtz_components = ["ZR", "ZT", "ZZ", "RR", "RT", "RZ", "TR", "TT", "TZ"]
 
     #######################################
     # #########PROCESSING SECTION##########
     #######################################
     def initializer():
         timespans = cc_store.get_timespans()
-        pairs_all = list(set(pair for ts in timespans for pair in cc_store.get_station_pairs(ts)))
+        pairs_all = cc_store.get_station_pairs()
         logger.info(f"Station pairs: {pairs_all}")
 
         if len(timespans) == 0 or len(pairs_all) == 0:
             raise IOError("Abort! no available CCF data for stacking")
         return timespans, pairs_all
 
     timespans, pairs_all = scheduler.initialize(initializer, 2)
```

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.4/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.9.4/src/noisepy/seis/asdfstore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-import datetime
 import glob
 import logging
 import os
 from pathlib import Path
 from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, TypeVar
 
 import numpy as np
 import obspy
 import pyasdf
 from datetimerange import DateTimeRange
 
 from . import noise_module
-from .constants import DATE_FORMAT, DONE_PATH, PROGRESS_DATATYPE
+from .constants import DONE_PATH, PROGRESS_DATATYPE
 from .datatypes import Channel, ChannelData, ChannelType, Station
-from .stores import CrossCorrelationDataStore, RawDataStore, StackStore
+from .stores import (
+    CrossCorrelationDataStore,
+    RawDataStore,
+    StackStore,
+    parse_station_pair,
+    parse_timespan,
+    timespan_str,
+)
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class ASDFDirectory(Generic[T]):
@@ -74,28 +80,28 @@
     """
     A data store implementation to read from a directory of ASDF files. Each file is considered
     a timespan with the naming convention: 2019_02_01_00_00_00T2019_02_02_00_00_00.h5
     """
 
     def __init__(self, directory: str, mode: str = "r"):
         super().__init__()
-        self.datasets = ASDFDirectory(directory, mode, _filename_from_timespan, _parse_timespan)
+        self.datasets = ASDFDirectory(directory, mode, _filename_from_timespan, parse_timespan)
 
     def get_channels(self, timespan: DateTimeRange) -> List[Channel]:
         with self.datasets[timespan] as ds:
             stations = [self._create_station(timespan, sta) for sta in ds.waveforms.list() if sta is not None]
             channels = [
                 Channel(ChannelType(tag), sta) for sta in stations for tag in ds.waveforms[str(sta)].get_waveform_tags()
             ]
             return channels
 
     def get_timespans(self) -> List[DateTimeRange]:
         return self.datasets.get_keys()
 
-    def read_data(self, timespan: DateTimeRange, chan: Channel) -> np.ndarray:
+    def read_data(self, timespan: DateTimeRange, chan: Channel) -> ChannelData:
         with self.datasets[timespan] as ds:
             stream = ds.waveforms[str(chan.station)][str(chan.type)]
         return ChannelData(stream)
 
     def get_inventory(self, timespan: DateTimeRange, station: Station) -> obspy.Inventory:
         with self.datasets[timespan] as ds:
             return ds.waveforms[str(station)]["StationXML"]
@@ -112,15 +118,15 @@
             return None
 
 
 class ASDFCCStore(CrossCorrelationDataStore):
     def __init__(self, directory: str, mode: str = "a") -> None:
         super().__init__()
         Path(directory).mkdir(exist_ok=True)
-        self.datasets = ASDFDirectory(directory, mode, _filename_from_timespan, _parse_timespan)
+        self.datasets = ASDFDirectory(directory, mode, _filename_from_timespan, parse_timespan)
 
     # CrossCorrelationDataStore implementation
     def contains(self, timespan: DateTimeRange, src_chan: Channel, rec_chan: Channel) -> bool:
         station_pair = self._get_station_pair(src_chan.station, rec_chan.station)
         channel_pair = self._get_channel_pair(src_chan.type, rec_chan.type)
         logger.debug(f"station pair {station_pair} channel pair {channel_pair}")
         contains = self.datasets.contains(timespan, station_pair, channel_pair)
@@ -147,49 +153,48 @@
 
     def is_done(self, timespan: DateTimeRange):
         return self.datasets.is_done(timespan)
 
     def get_timespans(self) -> List[DateTimeRange]:
         return self.datasets.get_keys()
 
-    def get_station_pairs(self, timespan: DateTimeRange) -> List[Tuple[Station, Station]]:
-        with self.datasets[timespan] as ccf_ds:
-            data = ccf_ds.auxiliary_data.list()
-            return [_parse_station_pair(p) for p in data if p != PROGRESS_DATATYPE]
+    def get_station_pairs(self) -> List[Tuple[Station, Station]]:
+        timespans = self.get_timespans()
+        pairs_all = set()
+        for timespan in timespans:
+            with self.datasets[timespan] as ccf_ds:
+                data = ccf_ds.auxiliary_data.list()
+                pairs_all.update(parse_station_pair(p) for p in data if p != PROGRESS_DATATYPE)
+        return list(pairs_all)
 
     def get_channeltype_pairs(
         self, timespan: DateTimeRange, src_sta: Station, rec_sta: Station
     ) -> List[Tuple[Channel, Channel]]:
         with self.datasets[timespan] as ccf_ds:
             dtype = self._get_station_pair(src_sta, rec_sta)
+            if dtype not in ccf_ds.auxiliary_data:
+                logging.warning(f"No data available for {timespan}/{dtype}")
+                return []
             ch_pairs = ccf_ds.auxiliary_data[dtype].list()
             return [tuple(map(ChannelType, ch.split("_"))) for ch in ch_pairs]
 
     def read(
         self, timespan: DateTimeRange, src_sta: Station, rec_sta: Station, src_ch: ChannelType, rec_ch: ChannelType
     ) -> Tuple[Dict, np.ndarray]:
         dtype = self._get_station_pair(src_sta, rec_sta)
         path = self._get_channel_pair(src_ch, rec_ch)
         with self.datasets[timespan] as ds:
             stream = ds.auxiliary_data[dtype][path]
             return (stream.parameters, stream.data[:])
 
-    # private helper methods
-
-    def _get_station_pair(self, src_sta: Station, rec_sta: Station) -> str:
-        return f"{src_sta}_{rec_sta}"
-
-    def _get_channel_pair(self, src_chan: ChannelType, rec_chan: ChannelType) -> str:
-        return f"{src_chan.name}_{rec_chan.name}"
-
 
 class ASDFStackStore(StackStore):
     def __init__(self, directory: str, mode: str = "a"):
         super().__init__()
-        self.datasets = ASDFDirectory(directory, mode, _filename_from_stations, _parse_station_pair)
+        self.datasets = ASDFDirectory(directory, mode, _filename_from_stations, parse_station_pair)
 
     def mark_done(self, src: Station, rec: Station):
         self.datasets.mark_done((src, rec))
 
     def is_done(self, src: Station, rec: Station):
         return self.datasets.is_done((src, rec))
 
@@ -206,28 +211,13 @@
     elif mode == "r":
         return None
     else:  # create new file
         Path(filename).parent.mkdir(exist_ok=True, parents=True)
         return pyasdf.ASDFDataSet(filename, mode=mode, mpi=False, compression=None)
 
 
-def _parse_timespan(filename: str) -> DateTimeRange:
-    parts = os.path.splitext(os.path.basename(filename))[0].split("T")
-    dates = [obspy.UTCDateTime(p).datetime.replace(tzinfo=datetime.timezone.utc) for p in parts]
-    return DateTimeRange(dates[0], dates[1])
-
-
-def _filename_from_timespan(timespan: DateTimeRange) -> str:
-    return f"{timespan.start_datetime.strftime(DATE_FORMAT)}T{timespan.end_datetime.strftime(DATE_FORMAT)}.h5"
-
-
 def _filename_from_stations(pair: Tuple[Station, Station]) -> str:
     return f"{pair[0]}/{pair[0]}_{pair[1]}.h5"
 
 
-def _parse_station_pair(pair: str) -> Tuple[Station, Station]:
-    # Parse from:'CI.ARV_CI.BAK
-    def station(sta: str) -> Station:
-        net, name = sta.split(".")
-        return Station(net, name)
-
-    return tuple(map(station, pair.split("_")))
+def _filename_from_timespan(timespan: DateTimeRange) -> str:
+    return f"{timespan_str(timespan)}.h5"
```

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.9.4/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.9.4/src/noisepy/seis/datatypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import sys
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
+from typing import List, Optional
 
 import numpy as np
 import obspy
-from pydantic import Field, root_validator
-from pydantic_yaml import YamlModel
+from pydantic import BaseModel, ConfigDict, Field
+from pydantic.functional_validators import model_validator
+from pydantic_yaml import parse_yaml_raw_as, to_yaml_str
 
 INVALID_COORD = -sys.float_info.max
 
 
 @dataclass
 class ChannelType:
     """
@@ -95,30 +97,32 @@
     ROBUST = "robust"
     AUTO_COVARIANCE = "auto_covariance"
     NROOT = "nroot"
     SELECTIVE = "selective"
     ALL = "all"
 
 
-class ConfigParameters(YamlModel):
+class ConfigParameters(BaseModel):
+    model_config = ConfigDict(validate_default=True)
+
     client_url_key: str = "SCEDC"
     start_date: datetime = Field(default=datetime(2019, 1, 1))
     end_date: datetime = Field(default=datetime(2019, 1, 2))
-    samp_freq: float = Field(default=20)  # TODO: change this samp_freq for the obspy "sampling_rate"
+    samp_freq: float = Field(default=20.0)  # TODO: change this samp_freq for the obspy "sampling_rate"
     cc_len: float = Field(default=1800.0, description="basic unit of data length for fft (sec)")
     # download params.
     # Targeted region/station information: only needed when down_list is False
-    lamin: float = Field(default=31, description="Download: minimum latitude")
-    lamax: float = Field(default=36, description="Download: maximum latitude")
-    lomin: float = Field(default=-122, description="Download: minimum longitude")
-    lomax: float = Field(default=-115, description="Download: maximum longitude")
-    down_list = Field(default=False, description="download stations from a pre-compiled list or not")
-    net_list = Field(default=["CI"], description="network list")
-    stations = Field(default=["*"], description="station list")
-    channels = Field(default=["BHE", "BHN", "BHZ"], description="channel list")
+    lamin: float = Field(default=31.0, description="Download: minimum latitude")
+    lamax: float = Field(default=36.0, description="Download: maximum latitude")
+    lomin: float = Field(default=-122.0, description="Download: minimum longitude")
+    lomax: float = Field(default=-115.0, description="Download: maximum longitude")
+    down_list: bool = Field(default=False, description="download stations from a pre-compiled list or not")
+    net_list: List[str] = Field(default=["CI"], description="network list")
+    stations: List[str] = Field(default=["*"], description="station list")
+    channels: List[str] = Field(default=["BHE", "BHN", "BHZ"], description="channel list")
     # pre-processing parameters
     step: float = Field(default=450.0, description="overlapping between each cc_len (sec)")
     freqmin: float = Field(default=0.05)
     freqmax: float = Field(default=2.0)
     freq_norm: str = Field(
         default="rma", description="choose between 'rma' for a soft whitenning or 'no' for no whitening"
     )
@@ -154,52 +158,55 @@
     ncomp: int = Field(default=3, description="1 or 3 component data (needed to decide whether to do rotation)")
     # station/instrument info for input_fmt=='sac' or 'mseed'
     stationxml: bool = Field(
         default=False, description="station.XML file used to remove instrument response for SAC/miniseed data"
     )
     rm_resp: str = Field(default="no", description="select 'no' to not remove response and use 'inv','spectrum',")
     rm_resp_out: str = Field(default="VEL", description="output location from response removal")
-    respdir: str = Field(default=None, description="response directory")
+    respdir: Optional[str] = Field(default=None, description="response directory")
     # some control parameters
     acorr_only: bool = Field(default=False, description="only perform auto-correlation")
     xcorr_only: bool = Field(default=True, description="only perform cross-correlation or not")
     # Stacking parameters:
     stack_method: StackMethod = Field(default=StackMethod.LINEAR)
     keep_substack: bool = Field(default=False, description="keep all sub-stacks in final ASDF file")
     # new rotation para
     rotation: bool = Field(default=True, description="rotation from E-N-Z to R-T-Z")
     correction: bool = Field(default=False, description="angle correction due to mis-orientation")
-    correction_csv: str = Field(default=None, description="Path to e.g. meso_angles.csv")
+    correction_csv: Optional[str] = Field(default=None, description="Path to e.g. meso_angles.csv")
     # 'RESP', or 'polozeros' to remove response
 
-    class Config:
-        use_enum_values = True
-
     @property
     def dt(self) -> float:
         return 1.0 / self.samp_freq
 
-    @root_validator
-    def validate(cld, values) -> dict:
-        assert values.get("substack_len") % values.get("cc_len") == 0
-        return values
+    @model_validator(mode="after")
+    def validate(cls, m: ConfigParameters) -> ConfigParameters:
+        if m.substack_len % m.cc_len != 0:
+            raise ValueError(f"substack_len ({m.substack_len}) must be a multiple of cc_len ({m.cc_len})")
+        return m
 
     # TODO: Remove once all uses of ConfigParameters have been converted to use strongly typed access
     def __getitem__(self, key):
         # Hack since pydantic model properties are nor part of the object's __dict__
         if key == "dt":
             return self.dt
         return self.__dict__[key]
 
     def save_yaml(self, filename: str):
-        # yaml_str = yaml.dump(self.__dict__)
-        yaml_str = self.yaml()
+        yaml_str = to_yaml_str(self)
         with open(filename, "w") as f:
             f.write(yaml_str)
 
+    def load_yaml(filename: str) -> ConfigParameters:
+        with open(filename, "r") as f:
+            yaml_str = f.read()
+            config = parse_yaml_raw_as(ConfigParameters, yaml_str)
+            return config
+
 
 @dataclass
 class Channel:
     """
     A channel instance belonging to a station. E.g. CI.ARV.BHN
     """
```

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/main.py` & `noisepy_seis-0.9.4/src/noisepy/seis/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,33 +57,33 @@
         return True
     elif bstr.upper() == "FALSE":
         return False
     raise ValueError(f"Invalid boolean value: '{bstr}'")
 
 
 def get_arg_type(arg_type):
-    if arg_type == list:
+    if arg_type == List[str]:
         return list_str
     if arg_type == datetime:
         return dateutil.parser.isoparse
     if arg_type == bool:
         return parse_bool
     return arg_type
 
 
 def add_model(parser: argparse.ArgumentParser, model: ConfigParameters):
     # Add config model to the parser
-    fields = model.__fields__
+    fields = model.model_fields
     for name, field in fields.items():
         parser.add_argument(
             f"--{name}",
             dest=name,
-            type=get_arg_type(field.type_),
+            type=get_arg_type(field.annotation),
             default=argparse.SUPPRESS,
-            help=field.field_info.description,
+            help=field.description,
         )
 
 
 def initialize_params(args, data_dir: str) -> ConfigParameters:
     """
     Loads initial parameters from 3 options:
     - --config_path option
@@ -93,15 +93,15 @@
     Then overrides with values passed in the command line
     """
     config_path = args.config
     if config_path is None and data_dir is not None:
         config_path = fs_join(data_dir, CONFIG_FILE)
     if config_path is not None and os.path.isfile(config_path):
         logger.info(f"Loading parameters from {config_path}")
-        params = ConfigParameters.parse_file(config_path)
+        params = ConfigParameters.load_yaml(config_path)
     else:
         logger.warning(f"Config file {config_path if config_path else ''} not found. Using default parameters.")
         params = ConfigParameters()
     cpy = params.copy(update={k: v for (k, v) in vars(args).items() if k in params.__fields__})
     return cpy
```

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.4/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.9.4/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/pnwstore.py` & `noisepy_seis-0.9.4/src/noisepy/seis/pnwstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.9.4/src/noisepy/seis/scedc_s3store.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/scheduler.py` & `noisepy_seis-0.9.4/src/noisepy/seis/scheduler.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/utils.py` & `noisepy_seis-0.9.4/src/noisepy/seis/utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/.gitignore` & `noisepy_seis-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/LICENSE` & `noisepy_seis-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/README.md` & `noisepy_seis-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.3/pyproject.toml` & `noisepy_seis-0.9.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,18 @@
     "numpy>=1.22.0",
     "pandas>=1.5.3",
     "pyasdf>=0.7.5",
     "pycwt>=0.3.0a22",
     "diskcache>=5.5",
     "fsspec>=2023.4.0",
     "s3fs>=2023.4.0",
-    "pydantic>=1.10.0",
+    "pydantic>=2.0.0",
     "PyYAML>=6.0",
-    "pydantic-yaml>=0.11",
+    "pydantic-yaml>=1.0",
+     "zarr>=2.14.2",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/mdenolle/NoisePy"
 
 [tool.hatch.version]
```

### Comparing `noisepy_seis-0.9.3/PKG-INFO` & `noisepy_seis-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.9.3
+Version: 0.9.4
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -38,18 +38,19 @@
 Requires-Dist: fsspec>=2023.4.0
 Requires-Dist: h5py>=3.8.0
 Requires-Dist: numba>=0.57.0
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: pyasdf>=0.7.5
 Requires-Dist: pycwt>=0.3.0a22
-Requires-Dist: pydantic-yaml>=0.11
-Requires-Dist: pydantic>=1.10.0
+Requires-Dist: pydantic-yaml>=1.0
+Requires-Dist: pydantic>=2.0.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: s3fs>=2023.4.0
+Requires-Dist: zarr>=2.14.2
 Provides-Extra: dev
 Requires-Dist: memory-profiler>=0.61; extra == 'dev'
 Requires-Dist: pre-commit>=3.2; extra == 'dev'
 Requires-Dist: pytest>=7.2.2; extra == 'dev'
 Provides-Extra: mpi
 Requires-Dist: mpi4py>=3.1.4; extra == 'mpi'
 Provides-Extra: sql
```

