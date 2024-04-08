# Comparing `tmp/bert_schemas-2.6.0.tar.gz` & `tmp/bert_schemas-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_schemas-2.6.0.tar", max compression
+gzip compressed data, was "bert_schemas-2.8.0.tar", max compression
```

## Comparing `bert_schemas-2.6.0.tar` & `bert_schemas-2.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      481 2023-09-15 22:26:41.753240 bert_schemas-2.6.0/README.md
--rw-r--r--   0        0        0      664 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/__init__.py
--rw-r--r--   0        0        0    36897 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/job.py
--rw-r--r--   0        0        0     1408 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/message.py
--rw-r--r--   0        0        0     7175 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/projected.py
--rw-r--r--   0        0        0     2087 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/qpu.py
--rw-r--r--   0        0        0     1420 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/qpu_access.py
--rw-r--r--   0        0        0     2494 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/questionnaire.py
--rw-r--r--   0        0        0      736 2024-02-07 20:43:29.153374 bert_schemas-2.6.0/bert_schemas/report.py
--rw-r--r--   0        0        0      618 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/testing/__init__.py
--rw-r--r--   0        0        0      575 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/testing/factories/__init__.py
--rw-r--r--   0        0        0     1006 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/testing/factories/helpers.py
--rw-r--r--   0        0        0     6291 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/testing/factories/job.py
--rw-r--r--   0        0        0     1983 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/testing/fixtures/__init__.py
--rw-r--r--   0        0        0     4136 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/testing/fixtures/job.py
--rw-r--r--   0        0        0        0 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/tests/__init__.py
--rw-r--r--   0        0        0    11105 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/tests/test_job_schemas.py
--rw-r--r--   0        0        0     1114 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/tests/test_projected.py
--rw-r--r--   0        0        0     5676 2024-02-07 20:43:29.156707 bert_schemas-2.6.0/bert_schemas/user.py
--rw-r--r--   0        0        0     1277 2024-02-07 21:17:46.685145 bert_schemas-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     1245 1970-01-01 00:00:00.000000 bert_schemas-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0      481 2023-07-27 14:24:40.167019 bert_schemas-2.8.0/README.md
+-rw-r--r--   0        0        0      664 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/__init__.py
+-rw-r--r--   0        0        0    40286 2024-02-20 19:59:23.747966 bert_schemas-2.8.0/bert_schemas/job.py
+-rw-r--r--   0        0        0     1408 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/message.py
+-rw-r--r--   0        0        0     7329 2024-02-20 19:59:23.747966 bert_schemas-2.8.0/bert_schemas/projected.py
+-rw-r--r--   0        0        0     2087 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/qpu.py
+-rw-r--r--   0        0        0     1420 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/qpu_access.py
+-rw-r--r--   0        0        0     2494 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/questionnaire.py
+-rw-r--r--   0        0        0      736 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/report.py
+-rw-r--r--   0        0        0      618 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/testing/__init__.py
+-rw-r--r--   0        0        0      575 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/testing/factories/__init__.py
+-rw-r--r--   0        0        0     1006 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/testing/factories/helpers.py
+-rw-r--r--   0        0        0     6291 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/testing/factories/job.py
+-rw-r--r--   0        0        0     1983 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0     4136 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/testing/fixtures/job.py
+-rw-r--r--   0        0        0        0 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/tests/__init__.py
+-rw-r--r--   0        0        0    12730 2024-02-20 19:59:23.747966 bert_schemas-2.8.0/bert_schemas/tests/test_job_schemas.py
+-rw-r--r--   0        0        0     1114 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/tests/test_projected.py
+-rw-r--r--   0        0        0     5676 2024-02-07 22:05:43.727648 bert_schemas-2.8.0/bert_schemas/user.py
+-rw-r--r--   0        0        0     1277 2024-02-20 20:37:54.883120 bert_schemas-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1245 1970-01-01 00:00:00.000000 bert_schemas-2.8.0/PKG-INFO
```

### Comparing `bert_schemas-2.6.0/bert_schemas/__init__.py` & `bert_schemas-2.8.0/bert_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/job.py` & `bert_schemas-2.8.0/bert_schemas/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -259,15 +259,14 @@
     ] = [0.0, 0.0]
     positions_um: Annotated[
         list[Annotated[float, Field(ge=-60.0, le=60.0)]],
         Field(min_length=2, max_length=121),
     ] = [-1.0, 1.0]
     spatial_interpolation: InterpolationType = InterpolationType.LINEAR
 
-    @computed_field
     @property
     def interpolation_kind(self) -> str:
         if self.spatial_interpolation == InterpolationType.OFF:
             kind = "zero"
         else:
             kind = InterpolationType[self.spatial_interpolation].name.lower()
         return kind
@@ -336,15 +335,14 @@
 
 
 class OpticalLandscape(BaseModel):
     interpolation: InterpolationType = InterpolationType.LINEAR
     landscapes: Annotated[list[Landscape], Field(min_length=1, max_length=5)]
     model_config = ConfigDict(validate_assignment=True)
 
-    @computed_field
     @property
     def interpolation_kind(self) -> str:
         if self.interpolation == "OFF":
             kind = "zero"
         else:
             kind = InterpolationType[self.interpolation].name.lower()
         return kind
@@ -789,58 +787,93 @@
         return amplitudes
 
 
 class Pulse(BaseModel):
     # times_ms upper range can be no larger than end_time_ms of job (80.0 ms is upper default)
     times_ms: Annotated[
         list[Annotated[float, Field(ge=0.0, le=80.0)]],
-        Field(min_length=1, max_length=10),
-    ]
+        Field(min_length=2, max_length=2),
+    ] = [0, 1]
     intensities_mw_per_cm2: Annotated[
-        list[Annotated[float, Field(ge=0.0, le=1000.0)]],
-        Field(min_length=1, max_length=10),
-    ]
-    detuning_mhz: Annotated[float, Field(ge=-100.0, le=100.0)]
-    interpolation: InterpolationType
+        list[Annotated[float, Field(ge=1.0, le=1.0)]], Field(min_length=2, max_length=2)
+    ] = [1, 1]
+    detuning_mhz: Annotated[float, Field(ge=0, le=0)] = 0
+    interpolation: InterpolationType = InterpolationType.OFF
     model_config = ConfigDict(validate_assignment=True, extra="forbid")
 
     @model_validator(mode="before")
     @classmethod
     def cross_validate(cls, values):
         if not len(values["times_ms"]) == len(values["intensities_mw_per_cm2"]):
             raise ValueError("Pulse data lists must have the same length.")
         return values
 
-    @field_validator("times_ms")
+    @field_validator("detuning_mhz", mode="before")
     @classmethod
-    def naturally_order_times(cls, v):
+    def resonant_detuning_check(cls, v):
+        if not v == 0:
+            raise ValueError("Only resonant (detuning=0) pulses are supported.")
+        return v
+
+    @field_validator("intensities_mw_per_cm2", mode="before")
+    @classmethod
+    def default_intensity(cls, v):
+        for i in v:
+            if not i == 1:
+                raise ValueError("Intensity control is not supported.")
+        return v
+
+    @field_validator("times_ms", mode="before")
+    @classmethod
+    def pulse_timing(cls, v):
+        if not len(v) == 2:
+            raise ValueError("Pulses must be defined by 2 times.")
+        if np.abs(np.abs(v[1]) - np.abs(v[0])) < 1:
+            raise ValueError("Pulse length must be an integer and >= 1ms")
         if not v == sorted(v):
             raise ValueError("Pulse times must be naturally ordered.")
         return v
 
+    @field_validator("interpolation", mode="before")
+    @classmethod
+    def no_interpolation(cls, v):
+        if not v == InterpolationType.OFF:
+            raise ValueError("Interpolation not supported for laser pulses.")
+        return v
+
     def __lt__(self, other):
         return min(self.times_ms) < min(other.times_ms)
 
 
 class Laser(BaseModel):
-    type: LaserType
-    position_um: float
-    pulses: Annotated[list[Pulse], Field(min_length=1, max_length=10)]
+    type: LaserType = LaserType.TERMINATOR
+    position_um: float = projected.TERMINATOR_POSITION
+    pulses: Annotated[list[Pulse], Field(min_length=1, max_length=1)]
     model_config = ConfigDict(validate_assignment=True)
 
-    @field_validator("pulses")
+    @field_validator("pulses", mode="before")
     @classmethod
-    def pulses_overlap(cls, v):
+    def pulse_timing(cls, v):
         for index, _ in enumerate(v):
             if index < len(v) - 1:
                 dt_ms = min(v[index + 1].times_ms) - max(v[index].times_ms)
                 if not dt_ms >= 1:
                     raise ValueError(
-                        f"Distinct pulses features too close together in time (< 1 ms)"
+                        "Distinct pulses features too close together in time (< 1 ms)"
                     )
+        if len(v) > 1:
+            raise ValueError("Only a single laser pulse is supported.")
+
+        return v
+
+    @field_validator("position_um", mode="before")
+    @classmethod
+    def default_position(cls, v):
+        if not v == projected.TERMINATOR_POSITION:
+            raise ValueError("Setting position for laser pulses is not supported.")
         return v
 
     def get_intensity_waveform(
         self, tstart_ms: float, tend_ms: float, sample_rate_hz: float
     ) -> np.ndarray:
         intensities = []
         time_ms = tstart_ms
@@ -873,28 +906,32 @@
             # jump current time to the end of the pulse
             time_ms += len(times_ms) * dt_ms
         # extend intensities list to the desired end time
         n_zeros = int(np.floor(((tend_ms - time_ms) / 1000.0) * sample_rate_hz))
         intensities.extend(np.zeros(n_zeros))
         return np.array(intensities)
 
-    @computed_field
     @property
     def detunings(self) -> list[float]:
         return [pulse.detuning_mhz for pulse in self.pulses]
 
-    @computed_field
     @property
     def detuning_triggers(self) -> list[float]:
         trigger_times_ms = [
             pulse.times_ms[-1] for pulse in self.pulses
         ]  # get last pulse
         trigger_times_ms.insert(0, 0)
         return trigger_times_ms[: len(self.pulses)]
 
+    def is_on(self, time_ms) -> bool:
+        for pulse in self.pulses:
+            if (time_ms >= pulse.times_ms[0]) & (time_ms <= pulse.times_ms[-1]):
+                return True
+        return False
+
 
 class NonPlotOutput(BaseModel):
     mot_fluorescence_image: Image
     tof_image: Image
     tof_fit_image: Image
     tof_fit: TofFit
     tof_x_slice: LineChart
@@ -915,19 +952,18 @@
         from_attributes=True, validate_assignment=True, extra="forbid"
     )
 
 
 class Output(BaseModel):
     input_id: int | None = None
     values: PlotOutput | NonPlotOutput
-    model_config = ConfigDict(validate_assignment=True, extra="forbid")
+    model_config = ConfigDict(validate_assignment=True)
 
 
-class JobOutput(Output):
-    ...
+class JobOutput(Output): ...
 
 
 class BecOutput(Output):
     values: NonPlotOutput
 
 
 class BarrierOutput(Output):
@@ -983,26 +1019,91 @@
                         )
                     ):
                         raise ValueError(
                             f"lasers[{laser_index}].pulses[{pulse_index}].times_ms max values cannot exceed end_time_ms"
                         )
         return self
 
+    @field_validator("lasers")
+    @classmethod
+    def check_lasers(cls, v):
+        if v:
+            if len(v) > 1:
+                raise ValueError("Multiple lasers not supported.")
+            for laser in v:
+                if not laser.type == LaserType.TERMINATOR:
+                    raise ValueError(
+                        "Must be type TERMINATOR. Other laser types not supported."
+                    )
+        return v
+
 
 class Input(BaseModel):
     job_id: int | None = None
     run: int | None = None
     values: InputValues
     output: Output | None = None
     notes: JobNote | None = None
     model_config = ConfigDict(validate_assignment=True)
 
 
+class RfEvaporationWithoutValidation(BaseModel):
+    times_ms: list[int]
+    frequencies_mhz: list[float]
+    powers_mw: list[float]
+    interpolation: RfInterpolationType
+
+
+class OpticalBarriersWithoutValidation(BaseModel):
+    times_ms: list[float]
+    positions_um: list[float]
+    heights_khz: list[float]
+    widths_um: list[float]
+    interpolation: InterpolationType
+    shape: ShapeType
+
+
+class LandscapeWithoutValidation(BaseModel):
+    time_ms: float
+    potentials_khz: list[float]
+    positions_um: list[float]
+    spatial_interpolation: InterpolationType
+
+
+class OpticalLandscapeWithoutValidation(BaseModel):
+    interpolation: InterpolationType
+    landscapes: list[LandscapeWithoutValidation]
+
+
+class PulseWithoutValidation(BaseModel):
+    times_ms: list[float]
+    intensities_mw_per_cm2: list[float]
+    detuning_mhz: float
+    interpolation: InterpolationType
+
+
+class LaserWithoutValidation(BaseModel):
+    type: LaserType
+    position_um: float
+    pulses: list[PulseWithoutValidation]
+
+
+class InputValuesWithoutValidation(BaseModel):
+    end_time_ms: int
+    image_type: ImageType
+    time_of_flight_ms: int
+    rf_evaporation: RfEvaporationWithoutValidation
+    optical_barriers: list[OpticalBarriersWithoutValidation] | None = None
+    optical_landscape: OpticalLandscapeWithoutValidation | None = None
+    lasers: list[LaserWithoutValidation] | None = None
+
+
 class InputWithoutOutput(Input):
-    output: Output = Field(exclude=True)
+    values: InputValuesWithoutValidation
+    output: object | None = Field(exclude=True)
 
 
 class JobBase(BaseModel):
     name: JobName
     origin: JobOrigin | None = None
     status: JobStatus = JobStatus.PENDING
     display: bool = True
@@ -1056,15 +1157,15 @@
 class JobCreate(JobBase):
     pass
 
 
 class ResponseInput(BaseModel):
     job_id: int | None = None
     run: int | None = None
-    values: InputValues
+    values: InputValuesWithoutValidation
     output: JobOutput | None = None
     notes: JobNote | None = None
     model_config = ConfigDict(from_attributes=True)
 
 
 class JobResponse(JobBase):
     external_id: UUID
@@ -1075,15 +1176,15 @@
 
 
 class JobInputsResponse(JobResponse):
     qpu_name: QPUName = QPUName.UNDEFINED
     inputs: list[InputWithoutOutput]
 
 
-class PaginatedJobsResponse(JobBase):
+class PaginatedJobsResponse(JobInputsResponse):
     external_id: UUID
     time_submit: datetime
     time_start: datetime | None = None
     time_complete: datetime | None = None
     model_config = ConfigDict(from_attributes=True, use_enum_values=True)
```

### Comparing `bert_schemas-2.6.0/bert_schemas/message.py` & `bert_schemas-2.8.0/bert_schemas/message.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/projected.py` & `bert_schemas-2.8.0/bert_schemas/projected.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 POSITION_STEP = 1.0  # grid step between projected spots, microns
 POSITION_MIN = -60.0  # minimum position of projected light, microns
 POSITION_MAX = 60  # maximum position of projected light, microns
 PROJECTED_SPOTS = np.arange(POSITION_MIN, POSITION_MAX + 1.0, POSITION_STEP)
 UPDATE_PERIOD = 0.1  # milliseconds between updates of projected light
 ENERGY_MIN = 0.0  # minimum projected energy shift at any position, kHz
 ENERGY_MAX = 100  # maximum projected energy shift at any position, kHz
-
+TERMINATOR_POSITION = 30 # position of the center of the gaussian terminator beam in um
+TERMINATOR_WIDTH = 20.7 # 1/e^2 width of the terminator beam in um
 
 def get_corrected_times(times: list[float]) -> list[float]:
     """Method to calculate the effective times realized by the projection system,
     which only updates optical features periodically
 
     Args:
         times (list[float]): Time, in ms, to be corrected
```

### Comparing `bert_schemas-2.6.0/bert_schemas/qpu.py` & `bert_schemas-2.8.0/bert_schemas/qpu.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/qpu_access.py` & `bert_schemas-2.8.0/bert_schemas/qpu_access.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/questionnaire.py` & `bert_schemas-2.8.0/bert_schemas/questionnaire.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/report.py` & `bert_schemas-2.8.0/bert_schemas/report.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/testing/__init__.py` & `bert_schemas-2.8.0/bert_schemas/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/testing/factories/__init__.py` & `bert_schemas-2.8.0/bert_schemas/testing/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/testing/factories/helpers.py` & `bert_schemas-2.8.0/bert_schemas/testing/factories/helpers.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/testing/factories/job.py` & `bert_schemas-2.8.0/bert_schemas/testing/factories/job.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/testing/fixtures/__init__.py` & `bert_schemas-2.8.0/bert_schemas/testing/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/testing/fixtures/job.py` & `bert_schemas-2.8.0/bert_schemas/testing/fixtures/job.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/tests/test_job_schemas.py` & `bert_schemas-2.8.0/bert_schemas/tests/test_job_schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,14 +164,30 @@
         "positions_um": [2, 3],
         "heights_khz": [2, 3],
         "widths_um": [2, 3],
         "interpolation": "LINEAR",
     }
 
 
+@pytest.fixture
+def laser_data():
+    yield {
+        "type": "TERMINATOR",
+        "position_um": 30,
+        "pulses": [
+            {
+                "times_ms": [1, 3],
+                "intensities_mw_per_cm2": [1, 1],
+                "detuning_mhz": 0,
+                "interpolation": "OFF",
+            }
+        ],
+    }
+
+
 def test_barrier_cross_validate(barrier_data):
     assert job_schema.Barrier.model_validate(barrier_data)
 
     barrier_data["heights_khz"] = [2, 3, 4]
     with pytest.raises(ValidationError):
         job_schema.Barrier.model_validate(barrier_data)
 
@@ -247,52 +263,107 @@
 # need Noah input
 # def test_barrier_get_position_spectra(barrier_data):
 #     barrier = job_schema.Barrier(**barrier_data)
 #     spectra = barrier.get_position_spectra([2, 3], [6, 3])
 #     assert spectra == np.ndarray([[0.0, 0.0], [0.27067057, 1.76499381]])
 
 
-def test_pulse_cross_validate():
-    pulse_data = {
-        "times_ms": [1, 3, 4],
-        "intensities_mw_per_cm2": [2, 3, 4],
-        "detuning_mhz": 2,
-        "interpolation": "LINEAR",
+@pytest.fixture
+def pulse_data():
+    yield {
+        "times_ms": [1, 2],
+        "intensities_mw_per_cm2": [1, 1],
+        "detuning_mhz": 0,
+        "interpolation": "OFF",
     }
+
+
+def test_pulse_cross_validate(pulse_data):
+
     assert job_schema.Pulse.model_validate(pulse_data)
 
     pulse_data["times_ms"] = [1, 3, 4, 5]
     with pytest.raises(ValidationError):
         job_schema.Pulse.model_validate(pulse_data)
 
 
-def test_laser_pulses_overlap():
+def test_pulse_resonant_detuning_check(pulse_data):
+
+    pulse_data["detuning_mhz"] = 2
+    with pytest.raises(ValidationError):
+        job_schema.Pulse.model_validate(pulse_data)
+
+
+def test_pulse_default_intensity(pulse_data):
+    pulse_data["intensities_mw_per_cm2"] = [2, 0]
+    with pytest.raises(ValidationError):
+        job_schema.Pulse.model_validate(pulse_data)
+
+
+def test_pulse_timing(pulse_data):
+
+    pulse_data["times_ms"] = [1]
+    with pytest.raises(ValidationError):
+        job_schema.Pulse.model_validate(pulse_data)
+
+    pulse_data["times_ms"] = [1.1, 2]
+    with pytest.raises(ValidationError):
+        job_schema.Pulse.model_validate(pulse_data)
+
+    pulse_data["times_ms"] = [8, 2]
+    with pytest.raises(ValidationError):
+        job_schema.Pulse.model_validate(pulse_data)
+
+
+def test_pulse_no_interpolation(pulse_data):
+    pulse_data["interpolation"] = "LINEAR"
+    with pytest.raises(ValidationError):
+        job_schema.Pulse.model_validate(pulse_data)
+
+
+def test_laser_pulse_timing():
+
+    pulse_data_1 = {
+        "times_ms": [1, 3],
+        "intensities_mw_per_cm2": [1, 1],
+        "detuning_mhz": 0,
+        "interpolation": "OFF",
+    }
+
+    pulse_data_2 = {
+        "times_ms": [2, 3],
+        "intensities_mw_per_cm2": [1, 1],
+        "detuning_mhz": 0,
+        "interpolation": "OFF",
+    }
+
     laser_data = {
         "type": "TERMINATOR",
-        "position_um": 1.0,
-        "pulses": [
-            {
-                "times_ms": [1, 3, 4],
-                "intensities_mw_per_cm2": [2, 3, 4],
-                "detuning_mhz": 2,
-                "interpolation": "LINEAR",
-            },
-            {
-                "times_ms": [1, 3, 4],
-                "intensities_mw_per_cm2": [2, 3, 4],
-                "detuning_mhz": 2,
-                "interpolation": "LINEAR",
-            },
-        ],
+        "position_um": 30,
+        "pulses": [job_schema.Pulse(**pulse_data_1), job_schema.Pulse(**pulse_data_2)],
     }
 
     with pytest.raises(ValidationError):
         job_schema.Laser.model_validate(laser_data)
 
 
+def laser_default_position(laser_data):
+
+    laser_data["position_um"] = 1
+    with pytest.raises(ValidationError):
+        job_schema.Laser.model_validate(laser_data)
+
+
+def test_laser_is_on(laser_data):
+    laser = job_schema.Laser(**laser_data)
+
+    assert laser.is_on(2) == True
+    assert laser.is_on(5) == False
+
+
 # need Noah input
 # def test_laser_get_intensity_waveform():
 #     laser_data = {
 #         "type": "TERMINATOR",
 #         "position_um": 1.0,
 #         "pulses": [
 #             {
@@ -346,21 +417,21 @@
                     "spatial_interpolation": "LINEAR",
                 },
             ],
         },
         "lasers": [
             {
                 "type": "TERMINATOR",
-                "position_um": 1.0,
+                "position_um": 30,
                 "pulses": [
                     {
-                        "times_ms": [1, 3, 4],
-                        "intensities_mw_per_cm2": [2, 3, 4],
-                        "detuning_mhz": 2,
-                        "interpolation": "LINEAR",
+                        "times_ms": [1, 3],
+                        "intensities_mw_per_cm2": [1, 1],
+                        "detuning_mhz": 0,
+                        "interpolation": "OFF",
                     }
                 ],
             }
         ],
     }
 
     assert job_schema.InputValues.model_validate(input_values)
```

### Comparing `bert_schemas-2.6.0/bert_schemas/tests/test_projected.py` & `bert_schemas-2.8.0/bert_schemas/tests/test_projected.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/bert_schemas/user.py` & `bert_schemas-2.8.0/bert_schemas/user.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-2.6.0/pyproject.toml` & `bert_schemas-2.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bert-schemas"
-version = "2.6.0"
+version = "2.8.0"
 description = "Bert service schemas"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
 exclude = ["**/.pytest_cache/**/*", "**/__pycache__", ".gitignore"]
```

### Comparing `bert_schemas-2.6.0/PKG-INFO` & `bert_schemas-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-schemas
-Version: 2.6.0
+Version: 2.8.0
 Summary: Bert service schemas
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

