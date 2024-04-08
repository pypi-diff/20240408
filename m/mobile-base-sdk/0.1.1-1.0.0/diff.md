# Comparing `tmp/mobile-base-sdk-0.1.1.tar.gz` & `tmp/mobile-base-sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobile-base-sdk-0.1.1.tar", last modified: Tue Jul 19 14:34:49 2022, max compression
+gzip compressed data, was "mobile-base-sdk-1.0.0.tar", last modified: Mon Apr  8 15:01:19 2024, max compression
```

## Comparing `mobile-base-sdk-0.1.1.tar` & `mobile-base-sdk-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 14:34:49.553016 mobile-base-sdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-19 14:34:40.000000 mobile-base-sdk-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-07-19 14:34:49.553016 mobile-base-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-07-19 14:34:40.000000 mobile-base-sdk-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 14:34:49.553016 mobile-base-sdk-0.1.1/mobile_base_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-07-19 14:34:40.000000 mobile-base-sdk-0.1.1/mobile_base_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9908 2022-07-19 14:34:40.000000 mobile-base-sdk-0.1.1/mobile_base_sdk/mobile_base_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 14:34:49.553016 mobile-base-sdk-0.1.1/mobile_base_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-07-19 14:34:49.000000 mobile-base-sdk-0.1.1/mobile_base_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-19 14:34:49.000000 mobile-base-sdk-0.1.1/mobile_base_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 14:34:49.000000 mobile-base-sdk-0.1.1/mobile_base_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-07-19 14:34:49.000000 mobile-base-sdk-0.1.1/mobile_base_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-19 14:34:49.000000 mobile-base-sdk-0.1.1/mobile_base_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-19 14:34:49.553016 mobile-base-sdk-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-07-19 14:34:40.000000 mobile-base-sdk-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:01:19.497186 mobile-base-sdk-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 15:01:10.000000 mobile-base-sdk-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-08 15:01:19.497186 mobile-base-sdk-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-08 15:01:10.000000 mobile-base-sdk-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:01:19.497186 mobile-base-sdk-1.0.0/mobile_base_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-08 15:01:10.000000 mobile-base-sdk-1.0.0/mobile_base_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-08 15:01:10.000000 mobile-base-sdk-1.0.0/mobile_base_sdk/lidar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-08 15:01:10.000000 mobile-base-sdk-1.0.0/mobile_base_sdk/mobile_base_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:01:19.497186 mobile-base-sdk-1.0.0/mobile_base_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-08 15:01:19.000000 mobile-base-sdk-1.0.0/mobile_base_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 15:01:19.000000 mobile-base-sdk-1.0.0/mobile_base_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:01:19.000000 mobile-base-sdk-1.0.0/mobile_base_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 15:01:19.000000 mobile-base-sdk-1.0.0/mobile_base_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 15:01:19.000000 mobile-base-sdk-1.0.0/mobile_base_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 15:01:19.497186 mobile-base-sdk-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-08 15:01:10.000000 mobile-base-sdk-1.0.0/setup.py
```

### Comparing `mobile-base-sdk-0.1.1/LICENSE` & `mobile-base-sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mobile-base-sdk-0.1.1/PKG-INFO` & `mobile-base-sdk-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mobile-base-sdk
-Version: 0.1.1
+Version: 1.0.0
 Summary: Mobile Base SDK for the Reachy robot.
 Home-page: https://github.com/pollen-robotics/mobile-base-sdk
 Author: Pollen Robotics
 Author-email: contact@pollen-robotics.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # Mobile Base Python SDK for Reachy 2021
 
 As of July 2022, the [Reachy robot](https://www.pollen-robotics.com/reachy/) gained mobility!
@@ -81,9 +79,7 @@
 
 ## Support 
 
 This project adheres to the Contributor [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [contact@pollen-robotics.com](mailto:contact@pollen-robotics.com).
 
 Visit [pollen-robotics.com](https://pollen-robotics.com) to learn more or join our [Dicord community](https://discord.com/invite/Kg3mZHTKgs) if you have any questions or want to share your ideas.
 Follow [@PollenRobotics](https://twitter.com/pollenrobotics) on Twitter for important announcements.
-
-
```

### Comparing `mobile-base-sdk-0.1.1/README.md` & `mobile-base-sdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mobile-base-sdk-0.1.1/mobile_base_sdk/mobile_base_sdk.py` & `mobile-base-sdk-1.0.0/mobile_base_sdk/mobile_base_sdk.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,32 @@
 
 This package provides remote access (via socket) to the mobile base of a Reachy robot.
 You can have access to basic information from the mobile base such as the battery voltage
 or the odometry. You can also easily make the mobile base move by setting a goal position
 in cartesian coordinates (x, y, theta) or directly send velocities (x_vel, y_vel, theta_vel).
 """
 
-from numpy import round, rad2deg, deg2rad
-import time
 import asyncio
+import time
 from concurrent.futures import ThreadPoolExecutor
-from queue import Queue
 from logging import getLogger
+from queue import Queue
+from typing import Optional
+
 
 import grpc
 from google.protobuf.empty_pb2 import Empty
-from google.protobuf.wrappers_pb2 import FloatValue, BoolValue
+from google.protobuf.wrappers_pb2 import BoolValue, FloatValue
+from numpy import deg2rad, rad2deg, round
+from reachy2_sdk_api import mobile_base_mobility_pb2 as mob_pb2
+from reachy2_sdk_api import mobile_base_mobility_pb2_grpc as mob_pb2_grpc
+from reachy2_sdk_api import mobile_base_utility_pb2 as util_pb2
+from reachy2_sdk_api import mobile_base_utility_pb2_grpc as util_pb2_grpc
 
-from reachy_sdk_api import mobile_platform_reachy_pb2 as mp_pb2, mobile_platform_reachy_pb2_grpc as mp_pb2_grpc
+from .lidar import Lidar
 
 
 class MobileBaseSDK:
     """The MobileBaseSDK class handles the connection with Reachy's mobile base.
 
     It holds:
 
@@ -29,174 +35,154 @@
     - the battery voltage to monitor the battery usage,
     - the control and drive mode of the base,
     - two methods to send target positions or target velocities.
 
     If you encounter a problem when using the base, you have access to an emergency shutdown method.
     """
 
-    def __init__(self, host: str, mobile_base_port: int = 50061) -> None:
+    def __init__(self, host: str, mobile_base_port: int = 50051) -> None:
         """Set up the connection with the mobile base."""
         self._logger = getLogger()
         self._host = host
-        self._mobile_nase_port = mobile_base_port
-        self._grpc_channel = grpc.insecure_channel(
-            f'{self._host}:{self._mobile_nase_port}')
-
-        self._stub = mp_pb2_grpc.MobilityServiceStub(self._grpc_channel)
-        self._presence_stub = mp_pb2_grpc.MobileBasePresenceServiceStub(
-            self._grpc_channel)
-
-        def get_drive_mode():
-            mode_id = self._stub.GetZuuuMode(Empty()).mode
-            return mp_pb2.ZuuuModePossiblities.keys()[mode_id]
-
-        def get_control_mode():
-            mode_id = self._stub.GetControlMode(Empty()).mode
-            return mp_pb2.ControlModePossiblities.keys()[mode_id]
+        self._mobile_base_port = mobile_base_port
+        self._grpc_channel = grpc.insecure_channel(f"{self._host}:{self._mobile_base_port}")
+
+        self._utility_stub = util_pb2_grpc.MobileBaseUtilityServiceStub(self._grpc_channel)
+        self._mobility_stub = mob_pb2_grpc.MobileBaseMobilityServiceStub(self._grpc_channel)
 
-        self._drive_mode = get_drive_mode().lower()
-        self._control_mode = get_control_mode().lower()
+        self._drive_mode = self._get_drive_mode().lower()
+        self._control_mode = self._get_control_mode().lower()
 
         self._max_xy_vel = 1.0
         self._max_rot_vel = 180.0
         self._max_xy_goto = 1.0
 
+        self.lidar = Lidar(self._grpc_channel)
+
     def __repr__(self) -> str:
         """Clean representation of a mobile base."""
-        return f'''<MobileBase host="{self._host}" - version={self.model_version} - battery_voltage=
-        {self.battery_voltage} - drive mode={self._drive_mode} - control mode={self.control_mode}>'''
+        repr_template = (
+            '<MobileBase host="{host}" on={on} \n'
+            " lidar_safety_enabled={lidar_safety_enabled} \n"
+            " battery_voltage={battery_voltage}>"
+        )
+        return repr_template.format(
+            host=self._host,
+            on=self.is_on(),
+            lidar_safety_enabled=self.lidar.safety_enabled,
+            battery_voltage=self.battery_voltage,
+        )
 
-    @property
-    def model_version(self):
-        """Return the mobile base version specified in Reachy's config file."""
-        return self._presence_stub.GetMobileBasePresence(Empty()).model_version.value
+    def _get_drive_mode(self):
+        mode_id = self._utility_stub.GetZuuuMode(Empty()).mode
+        return util_pb2.ZuuuModePossiblities.keys()[mode_id]
+
+    def _get_control_mode(self):
+        mode_id = self._utility_stub.GetControlMode(Empty()).mode
+        return util_pb2.ControlModePossiblities.keys()[mode_id]
 
     @property
-    def battery_voltage(self):
+    def battery_voltage(self) -> float:
         """Return the battery voltage. Battery should be recharged if it reaches 24.5V or below."""
-        return round(self._stub.GetBatteryLevel(Empty()).level.value, 1)
+        return round(self._utility_stub.GetBatteryLevel(Empty()).level.value, 1)
 
     @property
     def odometry(self):
         """Return the odometry of the base. x, y are in meters and theta in degree."""
-        response = self._stub.GetOdometry(Empty())
+        response = self._utility_stub.GetOdometry(Empty())
         odom = {
-            'x': round(response.x.value, 3),
-            'y': round(response.y.value, 3),
-            'theta': round(rad2deg(response.theta.value), 3),
+            "x": round(response.x.value, 3),
+            "y": round(response.y.value, 3),
+            "theta": round(rad2deg(response.theta.value), 3),
         }
         return odom
 
-    @property
-    def drive_mode(self):
-        """Return the base's drive mode.
-
-        Drive mode is one of ['cmd_vel', 'brake', 'free_wheel', 'emergency_stop'].
-        """
-        return self._drive_mode
-
-    @drive_mode.setter
-    def drive_mode(self, mode: str):
+    def _set_drive_mode(self, mode: str):
         """Set the base's drive mode."""
-        all_drive_modes = [mode.lower() for mode in mp_pb2.ZuuuModePossiblities.keys()][1:]
-        possible_drive_modes = [mode for mode in all_drive_modes if mode not in ('speed', 'goto')]
+        all_drive_modes = [mode.lower() for mode in util_pb2.ZuuuModePossiblities.keys()][1:]
+        possible_drive_modes = [mode for mode in all_drive_modes if mode not in ("speed", "goto")]
         if mode in possible_drive_modes:
-            req = mp_pb2.ZuuuModeCommand(
-                mode=getattr(mp_pb2.ZuuuModePossiblities, mode.upper())
-            )
-            self._stub.SetZuuuMode(req)
+            req = util_pb2.ZuuuModeCommand(mode=getattr(util_pb2.ZuuuModePossiblities, mode.upper()))
+            self._utility_stub.SetZuuuMode(req)
             self._drive_mode = mode
         else:
-            self._logger.warning(f'Drive mode requested should be in {possible_drive_modes}!')
+            self._logger.warning(f"Drive mode requested should be in {possible_drive_modes}!")
 
-    @property
-    def control_mode(self):
-        """Return the base's control mode.
-
-        Control mode is one of ['open_loop', 'pid'].
-        """
-        return self._control_mode
-
-    @control_mode.setter
-    def control_mode(self, mode: str):
+    def _set_control_mode(self, mode: str):
         """Set the base's control mode."""
-        possible_control_modes = [
-            mode.lower() for mode in mp_pb2.ControlModePossiblities.keys()][1:]
+        possible_control_modes = [mode.lower() for mode in util_pb2.ControlModePossiblities.keys()][1:]
         if mode in possible_control_modes:
-            req = mp_pb2.ControlModeCommand(
-                mode=getattr(mp_pb2.ControlModePossiblities, mode.upper())
-            )
-            self._stub.SetControlMode(req)
+            req = util_pb2.ControlModeCommand(mode=getattr(util_pb2.ControlModePossiblities, mode.upper()))
+            self._utility_stub.SetControlMode(req)
             self._control_mode = mode
         else:
-            self._logger.warning(f'Control mode requested should be in {possible_control_modes}!')
+            self._logger.warning(f"Control mode requested should be in {possible_control_modes}!")
 
     def reset_odometry(self):
         """Reset the odometry."""
-        self._stub.ResetOdometry(Empty())
+        self._utility_stub.ResetOdometry(Empty())
         time.sleep(0.03)
 
     def set_speed(self, x_vel: float, y_vel: float, rot_vel: float):
         """Send target speed. x_vel, y_vel are in m/s and rot_vel in deg/s for 200ms.
 
         The 200ms duration is predifined at the ROS level of the mobile base's code.
         This mode is prefered if the user wants to send speed instructions frequently.
         """
-        if self.drive_mode != 'cmd_vel':
-            self._drive_mode = 'cmd_vel'
+        if self._drive_mode != "cmd_vel":
+            self._set_drive_mode("cmd_vel")
 
-        for vel, value in {'x_vel': x_vel, 'y_vel': y_vel}.items():
+        for vel, value in {"x_vel": x_vel, "y_vel": y_vel}.items():
             if abs(value) > self._max_xy_vel:
-                raise ValueError(f'The asbolute value of {vel} should not be more than {self._max_xy_vel}!')
+                raise ValueError(f"The asbolute value of {vel} should not be more than {self._max_xy_vel}!")
 
         if abs(rot_vel) > self._max_rot_vel:
-            raise ValueError(f'The asbolute value of rot_vel should not be more than {self._max_rot_vel}!')
+            raise ValueError(f"The asbolute value of rot_vel should not be more than {self._max_rot_vel}!")
 
-        req = mp_pb2.TargetDirectionCommand(
-            direction=mp_pb2.DirectionVector(
+        req = mob_pb2.TargetDirectionCommand(
+            direction=mob_pb2.DirectionVector(
                 x=FloatValue(value=x_vel),
                 y=FloatValue(value=y_vel),
                 theta=FloatValue(value=deg2rad(rot_vel)),
             )
         )
-        self._stub.SendDirection(req)
+        self._mobility_stub.SendDirection(req)
 
     def goto(
-            self,
-            x: float,
-            y: float,
-            theta: float,
-            timeout: float = None,
-            tolerance: dict = {
-                'delta_x': 0.1,
-                'delta_y': 0.1,
-                'delta_theta': 15,
-                'distance': 0.1
-            }):
+        self,
+        x: float,
+        y: float,
+        theta: float,
+        timeout: Optional[float] = None,
+        tolerance: dict = {"delta_x": 0.1, "delta_y": 0.1, "delta_theta": 15, "distance": 0.1},
+    ):
         """Send target position. x, y are in meters and theta is in degree.
 
         (x, y) will define the position of the mobile base in cartesian space
         and theta its orientation. The zero position is set when the mobile base is
         started or if the  reset_odometry method is called.
         A timeout in seconds is defined so that the mobile base does get stuck in a go
         to call.
         The tolerance represents the margin along x, y and theta for which we consider
         that the mobile base has arrived its goal.
         """
+        if self.is_off():
+            raise RuntimeError(("Mobile base is off. Goto not sent."))
+
         exc_queue: Queue[Exception] = Queue()
 
         if not timeout:
             # We consider that the max velocity for the mobile base is 0.5 m/s
             # timeout is 2*_max_xy_goto / max velocity
-            timeout = 2*self._max_xy_goto / 0.5
+            timeout = 2 * self._max_xy_goto / 0.5
 
         def _wrapped_goto():
             try:
                 asyncio.run(
-                    self.goto_async(
+                    self._goto_async(
                         x=x,
                         y=y,
                         theta=theta,
                         timeout=timeout,
                         tolerance=tolerance,
                     ),
                 )
@@ -204,61 +190,75 @@
                 exc_queue.put(e)
 
         with ThreadPoolExecutor() as exec:
             exec.submit(_wrapped_goto)
         if not exc_queue.empty():
             raise exc_queue.get()
 
-    async def goto_async(
-            self,
-            x: float,
-            y: float,
-            theta: float,
-            timeout: float,
-            tolerance: dict = {
-                'delta_x': 0.1,
-                'delta_y': 0.1,
-                'delta_theta': 15,
-                'distance': 0.1
-            }):
+    async def _goto_async(
+        self,
+        x: float,
+        y: float,
+        theta: float,
+        timeout: float,
+        tolerance: dict = {"delta_x": 0.1, "delta_y": 0.1, "delta_theta": 15, "distance": 0.1},
+    ):
         """Async version of the goto method."""
-        for pos, value in {'x': x, 'y': y}.items():
+        for pos, value in {"x": x, "y": y}.items():
             if abs(value) > self._max_xy_goto:
-                raise ValueError(f'The asbolute value of {pos} should not be more than {self._max_xy_goto}!')
+                raise ValueError(f"The asbolute value of {pos} should not be more than {self._max_xy_goto}!")
 
-        req = mp_pb2.GoToVector(
+        req = mob_pb2.GoToVector(
             x_goal=FloatValue(value=x),
             y_goal=FloatValue(value=y),
             theta_goal=FloatValue(value=deg2rad(theta)),
         )
-        self._drive_mode = 'go_to'
-        self._stub.SendGoTo(req)
+        self._drive_mode = "go_to"
+        self._mobility_stub.SendGoTo(req)
 
         tic = time.time()
+        arrived: bool
         while time.time() - tic < timeout:
             arrived = True
             distance_to_goal = self._distance_to_goto_goal()
             for delta_key in tolerance.keys():
                 if tolerance[delta_key] < abs(distance_to_goal[delta_key]):
                     arrived = False
                     break
             await asyncio.sleep(0.1)
             if arrived:
                 break
 
+        if not arrived and self.lidar.obstacle_detection_status == "OBJECT_DETECTED_STOP":
+            self._logger.warning("Target not reached. Mobile base stopped because of obstacle.")
+
     def _distance_to_goto_goal(self):
-        response = self._stub.DistanceToGoal(Empty())
+        response = self._mobility_stub.DistanceToGoal(Empty())
         distance = {
-            'delta_x': round(response.delta_x.value, 3),
-            'delta_y': round(response.delta_y.value, 3),
-            'delta_theta': round(rad2deg(response.delta_theta.value), 3),
-            'distance': round(response.distance.value, 3),
+            "delta_x": round(response.delta_x.value, 3),
+            "delta_y": round(response.delta_y.value, 3),
+            "delta_theta": round(rad2deg(response.delta_theta.value), 3),
+            "distance": round(response.distance.value, 3),
         }
         return distance
 
-    def emergency_shutdown(self):
+    def turn_on(self) -> None:
         """Stop the mobile base immediately by changing its drive mode to 'brake'."""
-        self.drive_mode = 'brake'
+        self._set_drive_mode("brake")
+
+    def turn_off(self) -> None:
+        """Set the mobile base in free wheel mode."""
+        self._set_drive_mode("free_wheel")
+
+    def is_on(self) -> bool:
+        """Return True if the mobile base is not compliant."""
+        self._drive_mode = self._get_drive_mode().lower()
+        return not self._drive_mode == "free_wheel"
+
+    def is_off(self) -> bool:
+        """Return True if the mobile base is compliant."""
+        self._drive_mode = self._get_drive_mode().lower()
+        return self._drive_mode == "free_wheel"
 
     def _set_safety(self, safety_on):
-        req = mp_pb2.SetZuuuSafetyRequest(safety_on=BoolValue(value=safety_on))
-        self._stub.SetZuuuSafety(req)
+        req = mob_pb2.SetZuuuSafetyRequest(safety_on=BoolValue(value=safety_on))
+        self._utility_stub.SetZuuuSafety(req)
```

### Comparing `mobile-base-sdk-0.1.1/mobile_base_sdk.egg-info/PKG-INFO` & `mobile-base-sdk-1.0.0/mobile_base_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mobile-base-sdk
-Version: 0.1.1
+Version: 1.0.0
 Summary: Mobile Base SDK for the Reachy robot.
 Home-page: https://github.com/pollen-robotics/mobile-base-sdk
 Author: Pollen Robotics
 Author-email: contact@pollen-robotics.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # Mobile Base Python SDK for Reachy 2021
 
 As of July 2022, the [Reachy robot](https://www.pollen-robotics.com/reachy/) gained mobility!
@@ -81,9 +79,7 @@
 
 ## Support 
 
 This project adheres to the Contributor [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [contact@pollen-robotics.com](mailto:contact@pollen-robotics.com).
 
 Visit [pollen-robotics.com](https://pollen-robotics.com) to learn more or join our [Dicord community](https://discord.com/invite/Kg3mZHTKgs) if you have any questions or want to share your ideas.
 Follow [@PollenRobotics](https://twitter.com/pollenrobotics) on Twitter for important announcements.
-
-
```

### Comparing `mobile-base-sdk-0.1.1/setup.py` & `mobile-base-sdk-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 #!/usr/bin/env python
 """Setup config file."""
 
 from os import path
 
 from setuptools import find_packages, setup
 
-
 here = path.abspath(path.dirname(__file__))
 
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
-    name='mobile-base-sdk',
-    version='0.1.1',
-    packages=find_packages(exclude=['tests']),
-
+    name="mobile-base-sdk",
+    version="1.0.0",
+    packages=find_packages(exclude=["tests"]),
     install_requires=[
-        'numpy',
-        'reachy-sdk-api>=0.6.0',
-        'grpcio>=1.37',
-        'protobuf>3,<4',
-        'pygame',
+        "numpy>=1.24.0,<=1.26.4",
+        "grpcio>=1.59.0, <=1.62.2",
+        "protobuf>=4.25.0, <=4.25.3",
+        "pygame",
+        "pillow",
+        "reachy2-sdk-api==1.0.3",
     ],
-
     extras_require={
-        'doc': ['sphinx'],
+        "doc": ["sphinx"],
     },
-
-    author='Pollen Robotics',
-    author_email='contact@pollen-robotics.com',
-    url='https://github.com/pollen-robotics/mobile-base-sdk',
-
-    description='Mobile Base SDK for the Reachy robot.',
+    author="Pollen Robotics",
+    author_email="contact@pollen-robotics.com",
+    url="https://github.com/pollen-robotics/mobile-base-sdk",
+    description="Mobile Base SDK for the Reachy robot.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
 )
```

