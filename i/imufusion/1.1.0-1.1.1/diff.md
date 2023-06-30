# Comparing `tmp/imufusion-1.1.0.tar.gz` & `tmp/imufusion-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imufusion-1.1.0.tar", last modified: Thu Mar  2 20:13:25 2023, max compression
+gzip compressed data, was "imufusion-1.1.1.tar", last modified: Fri Jun 30 09:40:33 2023, max compression
```

## Comparing `imufusion-1.1.0.tar` & `imufusion-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:13:25.446752 imufusion-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:13:25.446752 imufusion-1.1.0/Fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/Fusion.h
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionAhrs.c
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionAhrs.h
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionAxes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionCalibration.h
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionCompass.c
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionCompass.h
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionConvention.h
--rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionOffset.c
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-02 20:13:12.000000 imufusion-1.1.0/Fusion/FusionOffset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-02 20:13:12.000000 imufusion-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-02 20:13:12.000000 imufusion-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-02 20:13:25.446752 imufusion-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:13:25.442752 imufusion-1.1.0/Python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:13:25.446752 imufusion-1.1.0/Python/Python-C-API/
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Ahrs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Axes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Compass.h
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Flags.h
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/InternalStates.h
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/Settings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-03-02 20:13:12.000000 imufusion-1.1.0/Python/Python-C-API/imufusion.c
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-03-02 20:13:12.000000 imufusion-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:13:25.446752 imufusion-1.1.0/imufusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-02 20:13:25.000000 imufusion-1.1.0/imufusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-02 20:13:25.000000 imufusion-1.1.0/imufusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:13:25.000000 imufusion-1.1.0/imufusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-02 20:13:25.000000 imufusion-1.1.0/imufusion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:13:25.446752 imufusion-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-02 20:13:12.000000 imufusion-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.552789 imufusion-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.548789 imufusion-1.1.1/Fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/Fusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionAhrs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionAhrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionAxes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionCalibration.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionCompass.c
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionCompass.h
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionConvention.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionOffset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionOffset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-30 09:40:18.000000 imufusion-1.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 09:40:18.000000 imufusion-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 09:40:33.552789 imufusion-1.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.544789 imufusion-1.1.1/Python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.552789 imufusion-1.1.1/Python/Python-C-API/
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Ahrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Axes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Compass.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Flags.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/InternalStates.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Offset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/imufusion.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-06-30 09:40:18.000000 imufusion-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.552789 imufusion-1.1.1/imufusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:40:33.552789 imufusion-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-30 09:40:18.000000 imufusion-1.1.1/setup.py
```

### Comparing `imufusion-1.1.0/Fusion/Fusion.h` & `imufusion-1.1.1/Fusion/Fusion.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Fusion/FusionAhrs.c` & `imufusion-1.1.1/Fusion/FusionAhrs.c`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 //------------------------------------------------------------------------------
 // Function declarations
 
 static FusionVector HalfGravity(const FusionAhrs *const ahrs);
 
 static FusionVector HalfMagnetic(const FusionAhrs *const ahrs);
 
+static FusionVector Feedback(const FusionVector sensor, const FusionVector reference);
+
 //------------------------------------------------------------------------------
 // Functions
 
 /**
  * @brief Initialises the AHRS algorithm structure.
  * @param ahrs AHRS algorithm structure.
  */
@@ -136,15 +138,15 @@
             FusionAhrsReset(ahrs);
             ahrs->quaternion = quaternion;
             ahrs->accelerationRejectionTimer = 0;
             ahrs->accelerationRejectionTimeout = true;
         }
 
         // Calculate accelerometer feedback scaled by 0.5
-        ahrs->halfAccelerometerFeedback = FusionVectorCrossProduct(FusionVectorNormalise(accelerometer), halfGravity);
+        ahrs->halfAccelerometerFeedback = Feedback(FusionVectorNormalise(accelerometer), halfGravity);
 
         // Ignore accelerometer if acceleration distortion detected
         if ((ahrs->initialising == true) || (FusionVectorMagnitudeSquared(ahrs->halfAccelerometerFeedback) <= ahrs->settings.accelerationRejection)) {
             halfAccelerometerFeedback = ahrs->halfAccelerometerFeedback;
             ahrs->accelerometerIgnored = false;
             ahrs->accelerationRejectionTimer -= ahrs->accelerationRejectionTimer >= 10 ? 10 : 0;
         } else {
@@ -165,15 +167,15 @@
             ahrs->magneticRejectionTimeout = true;
         }
 
         // Calculate direction of magnetic field indicated by algorithm
         const FusionVector halfMagnetic = HalfMagnetic(ahrs);
 
         // Calculate magnetometer feedback scaled by 0.5
-        ahrs->halfMagnetometerFeedback = FusionVectorCrossProduct(FusionVectorNormalise(FusionVectorCrossProduct(halfGravity, magnetometer)), halfMagnetic);
+        ahrs->halfMagnetometerFeedback = Feedback(FusionVectorNormalise(FusionVectorCrossProduct(halfGravity, magnetometer)), halfMagnetic);
 
         // Ignore magnetometer if magnetic distortion detected
         if ((ahrs->initialising == true) || (FusionVectorMagnitudeSquared(ahrs->halfMagnetometerFeedback) <= ahrs->settings.magneticRejection)) {
             halfMagnetometerFeedback = ahrs->halfMagnetometerFeedback;
             ahrs->magnetometerIgnored = false;
             ahrs->magneticRejectionTimer -= ahrs->magneticRejectionTimer >= 10 ? 10 : 0;
         } else {
@@ -259,14 +261,27 @@
         }
     }
     return FUSION_VECTOR_ZERO; // avoid compiler warning
 #undef Q
 }
 
 /**
+ * @brief Returns the feedback.
+ * @param sensor Sensor.
+ * @param reference Reference.
+ * @return Feedback.
+ */
+static FusionVector Feedback(const FusionVector sensor, const FusionVector reference) {
+    if (FusionVectorDotProduct(sensor, reference) < 0.0f) { // if error is >90 degrees
+        return FusionVectorNormalise(FusionVectorCrossProduct(sensor, reference));
+    }
+    return FusionVectorCrossProduct(sensor, reference);
+}
+
+/**
  * @brief Updates the AHRS algorithm using the gyroscope and accelerometer
  * measurements only.
  * @param ahrs AHRS algorithm structure.
  * @param gyroscope Gyroscope measurement in degrees per second.
  * @param accelerometer Accelerometer measurement in g.
  * @param deltaTime Delta time in seconds.
  */
@@ -316,14 +331,23 @@
  * @return Quaternion describing the sensor relative to the Earth.
  */
 FusionQuaternion FusionAhrsGetQuaternion(const FusionAhrs *const ahrs) {
     return ahrs->quaternion;
 }
 
 /**
+ * @brief Sets the quaternion describing the sensor relative to the Earth.
+ * @param ahrs AHRS algorithm structure.
+ * @param quaternion Quaternion describing the sensor relative to the Earth.
+ */
+void FusionAhrsSetQuaternion(FusionAhrs *const ahrs, const FusionQuaternion quaternion) {
+    ahrs->quaternion = quaternion;
+}
+
+/**
  * @brief Returns the linear acceleration measurement equal to the accelerometer
  * measurement with the 1 g of gravity removed.
  * @param ahrs AHRS algorithm structure.
  * @return Linear acceleration measurement in g.
  */
 FusionVector FusionAhrsGetLinearAcceleration(const FusionAhrs *const ahrs) {
 #define Q ahrs->quaternion.element
```

### Comparing `imufusion-1.1.0/Fusion/FusionAhrs.h` & `imufusion-1.1.1/Fusion/FusionAhrs.h`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 
 void FusionAhrsUpdateNoMagnetometer(FusionAhrs *const ahrs, const FusionVector gyroscope, const FusionVector accelerometer, const float deltaTime);
 
 void FusionAhrsUpdateExternalHeading(FusionAhrs *const ahrs, const FusionVector gyroscope, const FusionVector accelerometer, const float heading, const float deltaTime);
 
 FusionQuaternion FusionAhrsGetQuaternion(const FusionAhrs *const ahrs);
 
+void FusionAhrsSetQuaternion(FusionAhrs *const ahrs, const FusionQuaternion quaternion);
+
 FusionVector FusionAhrsGetLinearAcceleration(const FusionAhrs *const ahrs);
 
 FusionVector FusionAhrsGetEarthAcceleration(const FusionAhrs *const ahrs);
 
 FusionAhrsInternalStates FusionAhrsGetInternalStates(const FusionAhrs *const ahrs);
 
 FusionAhrsFlags FusionAhrsGetFlags(const FusionAhrs *const ahrs);
```

### Comparing `imufusion-1.1.0/Fusion/FusionAxes.h` & `imufusion-1.1.1/Fusion/FusionAxes.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Fusion/FusionCalibration.h` & `imufusion-1.1.1/Fusion/FusionCalibration.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Fusion/FusionCompass.c` & `imufusion-1.1.1/Fusion/FusionCompass.c`

 * *Files 4% similar despite different names*

```diff
@@ -38,12 +38,12 @@
         case FusionConventionNed: {
             const FusionVector up = FusionVectorMultiplyScalar(accelerometer, -1.0f);
             const FusionVector west = FusionVectorNormalise(FusionVectorCrossProduct(up, magnetometer));
             const FusionVector north = FusionVectorNormalise(FusionVectorCrossProduct(west, up));
             return FusionRadiansToDegrees(atan2f(west.axis.x, north.axis.x));
         }
     }
-	return 0; // avoid compiler warning
+    return 0; // avoid compiler warning
 }
 
 //------------------------------------------------------------------------------
 // End of file
```

### Comparing `imufusion-1.1.0/Fusion/FusionCompass.h` & `imufusion-1.1.1/Fusion/FusionCompass.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Fusion/FusionConvention.h` & `imufusion-1.1.1/Fusion/FusionConvention.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Fusion/FusionMath.h` & `imufusion-1.1.1/Fusion/FusionMath.h`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,24 @@
     }};
     return result;
 #undef A
 #undef B
 }
 
 /**
+ * @brief Returns the dot product.
+ * @param vectorA Vector A.
+ * @param vectorB Vector B.
+ * @return Dot product.
+ */
+static inline float FusionVectorDotProduct(const FusionVector vectorA, const FusionVector vectorB) {
+    return FusionVectorSum(FusionVectorHadamardProduct(vectorA, vectorB));
+}
+
+/**
  * @brief Returns the vector magnitude squared.
  * @param vector Vector.
  * @return Vector magnitude squared.
  */
 static inline float FusionVectorMagnitudeSquared(const FusionVector vector) {
     return FusionVectorSum(FusionVectorHadamardProduct(vector, vector));
 }
```

### Comparing `imufusion-1.1.0/Fusion/FusionOffset.c` & `imufusion-1.1.1/Fusion/FusionOffset.c`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Fusion/FusionOffset.h` & `imufusion-1.1.1/Fusion/FusionOffset.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/LICENSE.md` & `imufusion-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/PKG-INFO` & `imufusion-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imufusion
-Version: 1.1.0
+Version: 1.1.1
 Summary: Fusion Python package
 Home-page: https://github.com/xioTechnologies/Fusion
 Author: x-io Technologies Limited
 Author-email: info@x-io.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `imufusion-1.1.0/Python/Python-C-API/Ahrs.h` & `imufusion-1.1.1/Python/Python-C-API/Ahrs.h`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,25 @@
 }
 
 static PyObject *ahrs_get_quaternion(Ahrs *self) {
     const FusionQuaternion quaternion = FusionAhrsGetQuaternion(&self->ahrs);
     return quaternion_from(&quaternion);
 }
 
+static int ahrs_set_quaternion(Ahrs *self, PyObject *value, void *closure) {
+    if (PyObject_IsInstance(value, (PyObject *) &quaternion_object) == false) {
+        static char string[64];
+        snprintf(string, sizeof(string), "Value type is not %s", quaternion_object.tp_name);
+        PyErr_SetString(PyExc_TypeError, string);
+        return -1;
+    }
+    FusionAhrsSetQuaternion(&self->ahrs, ((Quaternion *) value)->quaternion);
+    return 0;
+}
+
 static PyObject *ahrs_get_linear_acceleration(Ahrs *self) {
     FusionVector *const linear_acceleration = malloc(sizeof(FusionVector));
     *linear_acceleration = FusionAhrsGetLinearAcceleration(&self->ahrs);
 
     const npy_intp dims[] = {3};
     PyObject *array = PyArray_SimpleNewFromData(1, dims, NPY_FLOAT, linear_acceleration->array);
     PyArray_ENABLEFLAGS((PyArrayObject *) array, NPY_ARRAY_OWNDATA);
@@ -187,21 +198,21 @@
     }
 
     FusionAhrsSetHeading(&self->ahrs, heading);;
     return 0;
 }
 
 static PyGetSetDef ahrs_get_set[] = {
-        {"settings", NULL, (setter) ahrs_set_settings,                       "", NULL},
-        {"quaternion",          (getter) ahrs_get_quaternion,          NULL, "", NULL},
-        {"linear_acceleration", (getter) ahrs_get_linear_acceleration, NULL, "", NULL},
-        {"earth_acceleration",  (getter) ahrs_get_earth_acceleration,  NULL, "", NULL},
-        {"internal_states",     (getter) ahrs_get_internal_states,     NULL, "", NULL},
-        {"flags",               (getter) ahrs_get_flags,               NULL, "", NULL},
-        {"heading",  NULL, (setter) ahrs_set_heading,                        "", NULL},
+        {"settings", NULL,                                    (setter) ahrs_set_settings,   "", NULL},
+        {"quaternion",          (getter) ahrs_get_quaternion, (setter) ahrs_set_quaternion, "", NULL},
+        {"linear_acceleration", (getter) ahrs_get_linear_acceleration, NULL,                "", NULL},
+        {"earth_acceleration",  (getter) ahrs_get_earth_acceleration,  NULL,                "", NULL},
+        {"internal_states",     (getter) ahrs_get_internal_states,     NULL,                "", NULL},
+        {"flags",               (getter) ahrs_get_flags,               NULL,                "", NULL},
+        {"heading",  NULL,                                    (setter) ahrs_set_heading,    "", NULL},
         {NULL}  /* sentinel */
 };
 
 static PyMethodDef ahrs_methods[] = {
         {"reset",                   (PyCFunction) ahrs_reset,                   METH_NOARGS,  ""},
         {"update",                  (PyCFunction) ahrs_update,                  METH_VARARGS, ""},
         {"update_no_magnetometer",  (PyCFunction) ahrs_update_no_magnetometer,  METH_VARARGS, ""},
```

### Comparing `imufusion-1.1.0/Python/Python-C-API/Axes.h` & `imufusion-1.1.1/Python/Python-C-API/Axes.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/Compass.h` & `imufusion-1.1.1/Python/Python-C-API/Compass.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/Flags.h` & `imufusion-1.1.1/Python/Python-C-API/Flags.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/Helpers.h` & `imufusion-1.1.1/Python/Python-C-API/Helpers.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/InternalStates.h` & `imufusion-1.1.1/Python/Python-C-API/InternalStates.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/Offset.h` & `imufusion-1.1.1/Python/Python-C-API/Offset.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/Quaternion.h` & `imufusion-1.1.1/Python/Python-C-API/Quaternion.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/Settings.h` & `imufusion-1.1.1/Python/Python-C-API/Settings.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/Python/Python-C-API/imufusion.c` & `imufusion-1.1.1/Python/Python-C-API/imufusion.c`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/README.md` & `imufusion-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/imufusion.egg-info/PKG-INFO` & `imufusion-1.1.1/imufusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imufusion
-Version: 1.1.0
+Version: 1.1.1
 Summary: Fusion Python package
 Home-page: https://github.com/xioTechnologies/Fusion
 Author: x-io Technologies Limited
 Author-email: info@x-io.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `imufusion-1.1.0/imufusion.egg-info/SOURCES.txt` & `imufusion-1.1.1/imufusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.0/setup.py` & `imufusion-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 github_url = "https://github.com/xioTechnologies/Fusion"
 
 ext_modules = Extension("imufusion", ["Python/Python-C-API/imufusion.c",
                                       "Fusion/FusionAhrs.c",
                                       "Fusion/FusionCompass.c",
                                       "Fusion/FusionOffset.c"],
                         include_dirs=[numpy.get_include()],
+                        define_macros=[("FUSION_USE_NORMAL_SQRT", None)],
                         libraries=(["m"] if "linux" in sys.platform else []))  # link math library for Linux
 
 setup(name="imufusion",
-      version="1.1.0",
+      version="1.1.1",
       description="Fusion Python package",
       long_description="See [github](" + github_url + ") for documentation and examples.",
       long_description_content_type='text/markdown',
       url=github_url,
       author="x-io Technologies Limited",
       author_email="info@x-io.co.uk",
       license="MIT",
```

