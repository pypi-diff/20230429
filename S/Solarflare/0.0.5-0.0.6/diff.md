# Comparing `tmp/Solarflare-0.0.5.tar.gz` & `tmp/Solarflare-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Solarflare-0.0.5.tar", last modified: Sun Apr 23 22:37:09 2023, max compression
+gzip compressed data, was "Solarflare-0.0.6.tar", last modified: Sat Apr 29 17:04:30 2023, max compression
```

## Comparing `Solarflare-0.0.5.tar` & `Solarflare-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:37:09.207240 Solarflare-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 22:37:09.207240 Solarflare-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 22:36:53.000000 Solarflare-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:37:09.203240 Solarflare-0.0.5/Solarflare/
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 22:36:53.000000 Solarflare-0.0.5/Solarflare/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-23 22:36:53.000000 Solarflare-0.0.5/Solarflare/nightcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-23 22:36:53.000000 Solarflare-0.0.5/Solarflare/solarflare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:37:09.203240 Solarflare-0.0.5/Solarflare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 22:37:09.207240 Solarflare-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 22:36:53.000000 Solarflare-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:04:30.253445 Solarflare-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-29 17:04:30.253445 Solarflare-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-29 17:04:17.000000 Solarflare-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:04:30.253445 Solarflare-0.0.6/Solarflare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-29 17:04:17.000000 Solarflare-0.0.6/Solarflare/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-29 17:04:17.000000 Solarflare-0.0.6/Solarflare/nightcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-29 17:04:17.000000 Solarflare-0.0.6/Solarflare/solarflare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:04:30.253445 Solarflare-0.0.6/Solarflare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-29 17:04:30.000000 Solarflare-0.0.6/Solarflare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 17:04:30.000000 Solarflare-0.0.6/Solarflare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:04:30.000000 Solarflare-0.0.6/Solarflare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 17:04:30.000000 Solarflare-0.0.6/Solarflare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 17:04:30.253445 Solarflare-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-29 17:04:17.000000 Solarflare-0.0.6/setup.py
```

### Comparing `Solarflare-0.0.5/Solarflare/conversions.py` & `Solarflare-0.0.6/Solarflare/conversions.py`

 * *Files identical despite different names*

### Comparing `Solarflare-0.0.5/Solarflare/nightcalc.py` & `Solarflare-0.0.6/Solarflare/nightcalc.py`

 * *Files identical despite different names*

### Comparing `Solarflare-0.0.5/Solarflare/solarflare.py` & `Solarflare-0.0.6/Solarflare/solarflare.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,139 @@
-import math
+# 1. TIME
+# For these calculations, it is convenient to use Julian dates.
 import datetime
+from decimal import Decimal, getcontext
+import math
 
-# degree input trigonometry functions
-
-def sin(x): return math.sin(math.radians(x))
-def cos(x): return math.cos(math.radians(x))
-def tan(x): return math.tan(math.radians(x))
-def acos(x): return math.degrees(math.acos(x))
-def asin(x): return math.degrees(math.asin(x))
-def atan2(y, x): return math.degrees(math.atan2(y, x))
-
-# Version function
-def VERSION():
-    return "0.0.5"
+# set the precision for Decimal module
+getcontext().prec = 50 # good precision, fast results
 
-# 1. TIME
-# for these calculations, it is convenient to use Julian dates.
 def julian_date(date=datetime.datetime.now()):
     time = date.timestamp() * 1000
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() else 0
-    return (time / 86400000) - (tzoffset / 1440) + 2440587.5
+    return Decimal((time / 86400000) - (tzoffset / 1440) + 2440587.5)
 
-J1970 = 2440588
-dayMs = 24 * 60 * 60 * 1000
+J1970 = Decimal('2440588')
+dayMs = Decimal('86400000')
 # this is the inverse of the Julian Date function
+
 def fromJulian(j):
-    return datetime.datetime.fromtimestamp((j + 0.5 - J1970) * dayMs / 1000.0)
+    return datetime.datetime.fromtimestamp(float((Decimal(j) + Decimal('0.5') - J1970) * (dayMs / Decimal('1000.0'))))
+
+
+#2. Math Tools
+# degree input trigonometry functions
+def sin(x): return Decimal(math.sin(math.radians(x)))
+def cos(x): return Decimal(math.cos(math.radians(x)))
+def tan(x): return Decimal(math.tan(math.radians(x)))
+def acos(x): return Decimal(math.degrees(math.acos(x)))
+def asin(x): return Decimal(math.degrees(math.asin(x)))
+def atan2(y, x): return Decimal(math.degrees(math.atan2(y, x)))
+
 
-# 2. Mean Anomaly of the Sun
+#3. The Mean Anomaly using Decimal for Accuracy
 def mean_anomaly(date=datetime.datetime.now()):
-    julian = julian_date(date)
-    # using formula defined at https://aa.quae.nl/en/reken/zonpositie.html
-    M = (357.5291 + 0.98560028 * (julian - 2451545)) % 360
-    return M
-
-# 3. Equation of Center
-def equation(date = datetime.datetime.now()):
-    # using formula defined at https://aa.quae.nl/en/reken/zonpositie.html
-    M = mean_anomaly(date)
-    C = 1.9148 * sin(M) + 0.0200 * sin(2 * M) + 0.0003 * sin(3 * M)
+    J = Decimal(julian_date(date))
+    J200 = Decimal('2451545')
+    M0 = Decimal('357.5291')
+    M1 = Decimal('0.98560028')
+    return (M0 + M1 * (J - J200)) % Decimal('360')
+
+#4. Equation of Center
+def equation(date=datetime.datetime.now()):
+    C1, C2, C3 = Decimal('1.9148'), Decimal('0.0200'), Decimal('0.0003')
+    M = Decimal(mean_anomaly(date))
+    C = C1 * sin(M) + C2 * sin(M * 2) + C3 * sin(M * 3)
     return C
 
-# 4. True Anomaly
-def true_anomaly(date = datetime.datetime.now()):
-    M = mean_anomaly(date)
-    C = equation(date)
-    return M + C
-
-# 5. The Perihelion and the Obliquity of the Ecliptic
-II = 102.9373
-e = 23.4393
+#5. True Anomaly
+def true_anomaly(date=datetime.datetime.now()):
+    return equation(date) + mean_anomaly(date)
+
+#6. Perihelion and Obliquity
+II = Decimal('102.9373')
+e = Decimal('23.4393')
 
-# 6. The Ecliptical Coordinates
+#7. Ecliptical Coordinates
 def ecliptical_longitude(date=datetime.datetime.now()):
     L = mean_anomaly(date) + II
-    mean = L + 180
-    longitude = mean + equation(date)
-    return longitude % 360
+    Lsun = Decimal(Decimal(L) + Decimal('180'))
+    long = Lsun + Decimal(equation(date))
+    return long % Decimal('360.0')
 
-# 7. The Equatorial Coordinates
-def declination(date=datetime.datetime.now()):
+#8. Equatorial Coordinates
+def right_ascension(date=datetime.datetime.now()):
     long = ecliptical_longitude(date)
-    delta = asin(sin(long) * sin(e))
-    return delta
+    ra = atan2(sin(long) * cos(e), cos(long))
+    return ra
 
-def right_ascension(date=datetime.datetime.now()):
+def declination(date=datetime.datetime.now()):
     long = ecliptical_longitude(date)
-    alpha = atan2(sin(long) * cos(e), cos(long))
-    return alpha
+    dec = asin(sin(long) * sin(e))
+    return dec
 
-# 8. The Observer
-def sidereal_time(longitude, time=datetime.datetime.now()):
+#9. The Observer
+def sidereal_time(longitude, date=datetime.datetime.now()):
     lw = -longitude
-    theta = (280.1470 + (360.9856235 * (julian_date(time) - 2451545)) - lw) % 360
+    theta1, theta2 = Decimal('280.1470'), Decimal('360.9856235')
+    theta = (theta1 + theta2 * (julian_date(date) - Decimal('2451545')) - Decimal(lw)) % Decimal('360')
     return theta
 
-
-# 9. The Solar Transit
+#10. Solar Transit
 def solar_transit(longitude, date=datetime.datetime.now()):
-    lw = -longitude
-    J = julian_date(date)
-    J2000 = 2451545.0
-    J0, J1, J2, J3 = 0.0009, 0.0053, -0.0068, 1.0000000
-    nx = ((J - J2000 - J0)/J3) - lw/360
-    n = round(nx)
-    jx = J + J3 * (n - nx)
-    Jtransit = jx + J1 * sin(mean_anomaly(date)) + J2 * sin(2 * ecliptical_longitude(date))
-    return Jtransit
+    L = mean_anomaly(date) + II
+    Lsun = Decimal(Decimal(L) + Decimal('180'))
+    J, J2000, J0, lw = julian_date(date), Decimal('2451545'), Decimal('0.0009'), -longitude
+    nx = ((J - J2000 - J0) / Decimal('1.0000000')) - Decimal(lw)/Decimal('360')
+    jx = J + Decimal('1.0000000') * (round(nx) - nx)
+    jtransit = jx + Decimal('0.0053') * sin(mean_anomaly(date)) - Decimal('0.0068') * sin(Decimal('2') * Lsun)
+    return jtransit
 
-# 10. Sunset and Sunrise Julian
+#11. Sunrise and Sunset
 def suntimes(latitude, longitude, date=datetime.datetime.now()):
     try:
-        ht = acos((sin(-0.83) - sin(latitude) * sin(declination(date))) / cos(latitude) * cos(declination(date)))
-        Jtransit = solar_transit(longitude, date)
-        Jrise = Jtransit - ht/360
-        Jset = Jtransit + ht / 360
-        return (Jrise, Jset)
+        ht = acos((sin(Decimal('-0.83')) - sin(Decimal(latitude)) * sin(declination(date)))/ cos(Decimal(latitude)) * cos(declination(date)))
+        Jrise = solar_transit(longitude, date) - (ht/Decimal('360')) * Decimal('1.0000000')
+        Jset = solar_transit(longitude, date) + (ht / Decimal('360')) * Decimal('1.0000000')
+        return (Jrise - Decimal('0.00247222222'), Decimal('0.00247222222') + Jset)
     except:
         return (None, None)
 
+
 def sunrise(latitude, longitude, date=datetime.datetime.now()):
     try:
-        sunrise = suntimes(latitude, longitude, date)[0]
-        return fromJulian(sunrise)
+        return fromJulian(suntimes(latitude, longitude, date)[0])
     except:
-        return f"Sun does not rise at specified location: ({latitude}, {longitude})"
+        return None
 
 def sunset(latitude, longitude, date=datetime.datetime.now()):
     try:
-        sunset = suntimes(latitude, longitude, date)[1]
-        return fromJulian(sunset)
+        return fromJulian(suntimes(latitude, longitude, date)[1])
     except:
-        return f"Sun does not set at specified location: ({latitude}, {longitude})"
+        return None
+
 
-# 11. Hour Angle & Horizontal Coordinates
+#12. Horizontal Coordinates
 def hour_angle(longitude, date=datetime.datetime.now()):
     return sidereal_time(longitude, date) - right_ascension(date)
 
-# Horizontal Coordinates
 def azimuth(latitude, longitude, date=datetime.datetime.now()):
     H = hour_angle(longitude, date)
     dec = declination(date)
     A = atan2(sin(H), cos(H) * sin(latitude) - tan(dec) * cos(latitude))
-    return A + 180
+    return A + Decimal('180')
 
 def altitude(latitude, longitude, date=datetime.datetime.now()):
     H = hour_angle(longitude, date)
     delta = declination(date)
     sinh = sin(delta) * sin(latitude) + cos(delta) * cos(latitude) * cos(H)
     return asin(sinh)
 
-# Seasons based on sun Longitude
+
+#13. Seasons
 def spring():
     date = datetime.datetime(datetime.datetime.now().year, 1, 1)
     for i in range(365):
         if round(ecliptical_longitude(date)) == 0:
             return date - datetime.timedelta(days=1)
         else:
             date += datetime.timedelta(days = 1)
@@ -159,26 +158,7 @@
     date = datetime.datetime(datetime.datetime.now().year, 1, 1)
     for i in range(365):
         if round(ecliptical_longitude(date)) == 270:
             return date
         else:
             date += datetime.timedelta(days=1)
 
-
-#12. Combine all previous methods into a convenient class
-class Daystar:
-    def __init__(self, latitude, longitude, height=0):
-        self.lat = latitude
-        self.long = longitude
-        self.ht = height
-
-    def set(self, date=datetime.datetime.now()): return sunset(self.lat, self.long, date)
-    def rise(self, date=datetime.datetime.now()): return sunrise(self.lat, self.long, date)
-    def transit(self, date=datetime.datetime.now(), julian=False): return fromJulian(solar_transit(self.long, date)) if julian == False else solar_transit(self.long, date)
-    def right_ascension(self, date = datetime.datetime.now()): return right_ascension(date)
-    def declination(self, date=datetime.datetime.now()): return declination(date)
-    def ecliptical_longitude(self, date=datetime.datetime.now()): return ecliptical_longitude(date)
-    def nadir(self, date=datetime.datetime.now()): return fromJulian(solar_transit(self.long, date) - 0.5)
-    def hour_angle(self, date=datetime.datetime.now()): return hour_angle(self.long, date)
-    def observer_angle(self): return -2.076 * math.sqrt(self.ht) / 60
-
-
```

### Comparing `Solarflare-0.0.5/setup.py` & `Solarflare-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='Solarflare',
-    version='0.0.5',
+    version='0.0.6',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with solar calculations',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/Solarflare',
     project_urls = {
```

