# Comparing `tmp/mappy-2.8.tar.gz` & `tmp/mappy-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mappy-2.8.tar", last modified: Thu Feb  1 17:36:10 2018, max compression
+gzip compressed data, was "dist/mappy-2.9.tar", last modified: Sat Feb 24 14:47:30 2018, max compression
```

## Comparing `mappy-2.8.tar` & `mappy-2.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)        0 2018-02-01 17:36:10.000000 mappy-2.8/
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    26701 2018-01-31 00:54:48.000000 mappy-2.8/align.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4282 2018-01-28 22:35:45.000000 mappy-2.8/bseq.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     1540 2017-12-13 14:03:32.000000 mappy-2.8/bseq.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     5433 2017-12-13 14:03:32.000000 mappy-2.8/chain.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     1826 2017-12-13 14:03:32.000000 mappy-2.8/esterr.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    14951 2017-12-13 14:03:32.000000 mappy-2.8/format.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4896 2017-12-13 14:03:32.000000 mappy-2.8/getopt.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     1670 2017-12-13 14:03:32.000000 mappy-2.8/getopt.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    15066 2018-01-31 15:27:44.000000 mappy-2.8/hit.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    15549 2018-01-19 15:32:50.000000 mappy-2.8/index.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     7245 2017-12-13 14:03:32.000000 mappy-2.8/kalloc.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)      509 2017-12-13 14:03:32.000000 mappy-2.8/kalloc.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4400 2017-12-13 14:03:32.000000 mappy-2.8/kdq.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    21381 2017-12-13 14:03:32.000000 mappy-2.8/khash.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     8555 2017-12-13 14:03:32.000000 mappy-2.8/kseq.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     5154 2018-01-26 17:24:46.000000 mappy-2.8/ksort.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     8262 2018-01-08 16:33:33.000000 mappy-2.8/ksw2.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4366 2017-12-13 14:03:32.000000 mappy-2.8/ksw2_dispatch.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    17390 2017-12-31 01:36:41.000000 mappy-2.8/ksw2_extd2_sse.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    16348 2018-01-08 00:19:37.000000 mappy-2.8/ksw2_exts2_sse.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    13161 2017-12-13 14:03:32.000000 mappy-2.8/ksw2_extz2_sse.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4564 2017-12-13 14:03:32.000000 mappy-2.8/ksw2_ll_sse.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4074 2018-01-19 15:37:19.000000 mappy-2.8/kthread.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)      291 2017-12-13 14:03:32.000000 mappy-2.8/kthread.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     3029 2017-12-13 14:03:32.000000 mappy-2.8/kvec.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    16893 2018-01-31 18:59:15.000000 mappy-2.8/main.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     3777 2018-02-01 17:21:48.000000 mappy-2.8/Makefile
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)      227 2017-12-13 14:03:32.000000 mappy-2.8/MANIFEST.in
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    20626 2018-01-31 17:53:45.000000 mappy-2.8/map.c
-drwxr-xr-x   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)        0 2018-02-01 17:36:10.000000 mappy-2.8/mappy.egg-info/
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)        1 2018-02-01 17:36:10.000000 mappy-2.8/mappy.egg-info/dependency_links.txt
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     6501 2018-02-01 17:36:10.000000 mappy-2.8/mappy.egg-info/PKG-INFO
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)      579 2018-02-01 17:36:10.000000 mappy-2.8/mappy.egg-info/SOURCES.txt
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)        6 2018-02-01 17:36:10.000000 mappy-2.8/mappy.egg-info/top_level.txt
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    10422 2018-01-31 17:52:33.000000 mappy-2.8/minimap.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     3612 2018-01-19 15:36:15.000000 mappy-2.8/misc.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4060 2018-01-30 23:50:07.000000 mappy-2.8/mmpriv.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4923 2018-01-31 17:52:38.000000 mappy-2.8/options.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     5664 2017-12-13 14:03:32.000000 mappy-2.8/pe.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     6501 2018-02-01 17:36:10.000000 mappy-2.8/PKG-INFO
-drwxr-xr-x   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)        0 2018-02-01 17:36:10.000000 mappy-2.8/python/
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     2613 2018-01-31 16:20:07.000000 mappy-2.8/python/cmappy.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     2588 2018-01-31 16:31:30.000000 mappy-2.8/python/cmappy.pxd
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)   419991 2018-02-01 17:35:34.000000 mappy-2.8/python/mappy.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     5280 2018-01-31 16:11:29.000000 mappy-2.8/python/mappy.pyx
--rwxr-xr-x   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     1258 2017-12-13 14:03:32.000000 mappy-2.8/python/minimap2.py
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     4597 2018-01-31 16:29:19.000000 mappy-2.8/python/README.rst
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)    18436 2018-02-01 17:26:18.000000 mappy-2.8/README.md
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     6595 2017-12-13 14:03:32.000000 mappy-2.8/sdust.c
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)      574 2017-12-13 14:03:32.000000 mappy-2.8/sdust.h
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)       38 2018-02-01 17:36:10.000000 mappy-2.8/setup.cfg
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     1851 2018-01-31 15:10:49.000000 mappy-2.8/setup.py
--rw-r--r--   0 hengli   (1686716830) CHARLES\Domain Users (1594166068)     5829 2018-01-19 15:39:22.000000 mappy-2.8/sketch.c
+drwxr-xr-x   0 hengli   (1686716830) 1594166068        0 2018-02-24 14:47:30.000000 mappy-2.9/
+-rw-r--r--   0 hengli   (1686716830) 1594166068    28420 2018-02-24 14:32:11.000000 mappy-2.9/align.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     4414 2018-02-24 14:32:11.000000 mappy-2.9/bseq.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     1540 2018-02-01 20:12:44.000000 mappy-2.9/bseq.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     5433 2018-02-01 20:12:44.000000 mappy-2.9/chain.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     1826 2018-02-01 20:12:44.000000 mappy-2.9/esterr.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068    14951 2018-02-01 20:12:44.000000 mappy-2.9/format.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     4896 2018-02-01 20:12:44.000000 mappy-2.9/getopt.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     1670 2018-02-01 20:12:44.000000 mappy-2.9/getopt.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068    16025 2018-02-24 14:32:11.000000 mappy-2.9/hit.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068    16069 2018-02-24 14:32:11.000000 mappy-2.9/index.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     7245 2018-02-01 20:12:44.000000 mappy-2.9/kalloc.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068      509 2018-02-01 20:12:44.000000 mappy-2.9/kalloc.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     4400 2018-02-01 20:12:44.000000 mappy-2.9/kdq.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068    21381 2018-02-01 20:12:44.000000 mappy-2.9/khash.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     8555 2018-02-01 20:12:44.000000 mappy-2.9/kseq.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     5154 2018-02-01 20:12:44.000000 mappy-2.9/ksort.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     8262 2018-02-01 20:12:44.000000 mappy-2.9/ksw2.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     4366 2018-02-01 20:12:44.000000 mappy-2.9/ksw2_dispatch.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068    17390 2018-02-01 20:12:44.000000 mappy-2.9/ksw2_extd2_sse.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068    16348 2018-02-01 20:12:44.000000 mappy-2.9/ksw2_exts2_sse.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068    13161 2018-02-01 20:12:44.000000 mappy-2.9/ksw2_extz2_sse.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     4564 2018-02-01 20:12:44.000000 mappy-2.9/ksw2_ll_sse.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     4074 2018-02-01 20:12:44.000000 mappy-2.9/kthread.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068      291 2018-02-01 20:12:44.000000 mappy-2.9/kthread.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     3029 2018-02-01 20:12:44.000000 mappy-2.9/kvec.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068    17169 2018-02-24 14:32:11.000000 mappy-2.9/main.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     3777 2018-02-24 14:32:51.000000 mappy-2.9/Makefile
+-rw-r--r--   0 hengli   (1686716830) 1594166068      227 2018-02-01 20:12:44.000000 mappy-2.9/MANIFEST.in
+-rw-r--r--   0 hengli   (1686716830) 1594166068    20640 2018-02-24 14:32:11.000000 mappy-2.9/map.c
+drwxr-xr-x   0 hengli   (1686716830) 1594166068        0 2018-02-24 14:47:30.000000 mappy-2.9/mappy.egg-info/
+-rw-r--r--   0 hengli   (1686716830) 1594166068        1 2018-02-24 14:47:30.000000 mappy-2.9/mappy.egg-info/dependency_links.txt
+-rw-r--r--   0 hengli   (1686716830) 1594166068     7422 2018-02-24 14:47:30.000000 mappy-2.9/mappy.egg-info/PKG-INFO
+-rw-r--r--   0 hengli   (1686716830) 1594166068      579 2018-02-24 14:47:30.000000 mappy-2.9/mappy.egg-info/SOURCES.txt
+-rw-r--r--   0 hengli   (1686716830) 1594166068        6 2018-02-24 14:47:30.000000 mappy-2.9/mappy.egg-info/top_level.txt
+-rw-r--r--   0 hengli   (1686716830) 1594166068    10779 2018-02-24 14:32:11.000000 mappy-2.9/minimap.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     3797 2018-02-24 14:32:11.000000 mappy-2.9/misc.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     4007 2018-02-24 14:32:11.000000 mappy-2.9/mmpriv.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     5456 2018-02-24 14:32:11.000000 mappy-2.9/options.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     5664 2018-02-01 20:12:44.000000 mappy-2.9/pe.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     7422 2018-02-24 14:47:30.000000 mappy-2.9/PKG-INFO
+drwxr-xr-x   0 hengli   (1686716830) 1594166068        0 2018-02-24 14:47:30.000000 mappy-2.9/python/
+-rw-r--r--   0 hengli   (1686716830) 1594166068     3291 2018-02-24 14:32:11.000000 mappy-2.9/python/cmappy.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068     2797 2018-02-24 14:32:11.000000 mappy-2.9/python/cmappy.pxd
+-rw-r--r--   0 hengli   (1686716830) 1594166068   450312 2018-02-24 14:47:00.000000 mappy-2.9/python/mappy.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068     6250 2018-02-24 14:32:11.000000 mappy-2.9/python/mappy.pyx
+-rwxr-xr-x   0 hengli   (1686716830) 1594166068     1258 2018-02-01 20:12:44.000000 mappy-2.9/python/minimap2.py
+-rw-r--r--   0 hengli   (1686716830) 1594166068     5353 2018-02-24 14:32:11.000000 mappy-2.9/python/README.rst
+-rw-r--r--   0 hengli   (1686716830) 1594166068    17918 2018-02-24 14:32:11.000000 mappy-2.9/README.md
+-rw-r--r--   0 hengli   (1686716830) 1594166068     6595 2018-02-01 20:12:44.000000 mappy-2.9/sdust.c
+-rw-r--r--   0 hengli   (1686716830) 1594166068      574 2018-02-01 20:12:44.000000 mappy-2.9/sdust.h
+-rw-r--r--   0 hengli   (1686716830) 1594166068       38 2018-02-24 14:47:30.000000 mappy-2.9/setup.cfg
+-rw-r--r--   0 hengli   (1686716830) 1594166068     1864 2018-02-24 14:32:11.000000 mappy-2.9/setup.py
+-rw-r--r--   0 hengli   (1686716830) 1594166068     5829 2018-02-01 20:12:44.000000 mappy-2.9/sketch.c
```

### Comparing `mappy-2.8/align.c` & `mappy-2.9/align.c`

 * *Files 6% similar despite different names*

```diff
@@ -24,47 +24,71 @@
 {
 	uint32_t i;
 	uint8_t t;
 	for (i = 0; i < len>>1; ++i)
 		t = seq[i], seq[i] = seq[len - 1 - i], seq[len - 1 - i] = t;
 }
 
-static inline int test_zdrop_aux(int32_t score, int i, int j, int32_t *max, int *max_i, int *max_j, int e, int zdrop)
+static inline void update_max_zdrop(int32_t score, int i, int j, int32_t *max, int *max_i, int *max_j, int e, int *max_zdrop, int pos[2][2])
 {
 	if (score < *max) {
 		int li = i - *max_i;
 		int lj = j - *max_j;
 		int diff = li > lj? li - lj : lj - li;
-		if (*max - score > zdrop + diff * e)
-			return 1;
+		int z = *max - score - diff * e;
+		if (z > *max_zdrop) {
+			*max_zdrop = z;
+			pos[0][0] = *max_i, pos[0][1] = i + 1;
+			pos[1][0] = *max_j, pos[1][1] = j + 1;
+		}
 	} else *max = score, *max_i = i, *max_j = j;
-	return 0;
 }
 
-static int mm_check_zdrop(const uint8_t *qseq, const uint8_t *tseq, uint32_t n_cigar, uint32_t *cigar, const int8_t *mat, int8_t q, int8_t e, int zdrop)
+static int mm_test_zdrop(void *km, const mm_mapopt_t *opt, const uint8_t *qseq, const uint8_t *tseq, uint32_t n_cigar, uint32_t *cigar, const int8_t *mat)
 {
 	uint32_t k;
-	int32_t score = 0, max = 0, max_i = -1, max_j = -1, i = 0, j = 0;
-	for (k = 0; k < n_cigar; ++k) {
+	int32_t score = 0, max = INT32_MIN, max_i = -1, max_j = -1, i = 0, j = 0, max_zdrop = 0;
+	int pos[2][2] = {{-1, -1}, {-1, -1}}, q_len, t_len;
+
+	// find the score and the region where score drops most along diagonal
+	for (k = 0, score = 0; k < n_cigar; ++k) {
 		uint32_t l, op = cigar[k]&0xf, len = cigar[k]>>4;
 		if (op == 0) {
 			for (l = 0; l < len; ++l) {
 				score += mat[tseq[i + l] * 5 + qseq[j + l]];
-				if (test_zdrop_aux(score, i+l, j+l, &max, &max_i, &max_j, e, zdrop)) return 1;
+				update_max_zdrop(score, i+l, j+l, &max, &max_i, &max_j, opt->e, &max_zdrop, pos);
 			}
 			i += len, j += len;
-		} else if (op == 1) {
-			score -= q + e * len, j += len;
-			if (test_zdrop_aux(score, i, j, &max, &max_i, &max_j, e, zdrop)) return 1;
-		} else if (op == 2 || op == 3) {
-			score -= q + e * len, i += len;
-			if (test_zdrop_aux(score, i, j, &max, &max_i, &max_j, e, zdrop)) return 1;
+		} else if (op == 1 || op == 2 || op == 3) {
+			score -= opt->q + opt->e * len;
+			if (op == 1) j += len; // insertion
+			else i += len;         // deletion
+			update_max_zdrop(score, i, j, &max, &max_i, &max_j, opt->e, &max_zdrop, pos);
 		}
 	}
-	return 0;
+
+	// test if there is an inversion in the most dropped region
+	q_len = pos[1][1] - pos[1][0], t_len = pos[0][1] - pos[0][0];
+	if (!(opt->flag&(MM_F_SPLICE|MM_F_SR|MM_F_FOR_ONLY|MM_F_REV_ONLY)) && max_zdrop > opt->zdrop_inv && q_len < opt->max_gap && t_len < opt->max_gap) {
+		uint8_t *qseq2;
+		void *qp;
+		int q_off, t_off;
+		qseq2 = (uint8_t*)kmalloc(km, q_len);
+		for (i = 0; i < q_len; ++i) {
+			int c = qseq[pos[1][1] - i - 1];
+			qseq2[i] = c >= 4? 4 : 3 - c;
+		}
+		qp = ksw_ll_qinit(km, 2, q_len, qseq2, 5, mat);
+		score = ksw_ll_i16(qp, t_len, tseq + pos[0][0], opt->q, opt->e, &q_off, &t_off);
+		kfree(km, qseq2);
+		kfree(km, qp);
+		if (score >= opt->min_chain_score * opt->a && score >= opt->min_dp_max)
+			return 2; // there is a potential inversion
+	}
+	return max_zdrop > opt->zdrop? 1 : 0;
 }
 
 static void mm_fix_cigar(mm_reg1_t *r, const uint8_t *qseq, const uint8_t *tseq, int *qshift, int *tshift)
 {
 	mm_extra_t *p = r->p;
 	int32_t k, toff = 0, qoff = 0, to_shrink = 0;
 	*qshift = *tshift = 0;
@@ -189,17 +213,16 @@
 		p->n_cigar += n_cigar - 1;
 	} else {
 		memcpy(p->cigar + p->n_cigar, cigar, n_cigar * 4);
 		p->n_cigar += n_cigar;
 	}
 }
 
-static void mm_align_pair(void *km, const mm_mapopt_t *opt, int qlen, const uint8_t *qseq, int tlen, const uint8_t *tseq, const int8_t *mat, int w, int end_bonus, int flag, ksw_extz_t *ez)
+static void mm_align_pair(void *km, const mm_mapopt_t *opt, int qlen, const uint8_t *qseq, int tlen, const uint8_t *tseq, const int8_t *mat, int w, int end_bonus, int zdrop, int flag, ksw_extz_t *ez)
 {
-	int zdrop = opt->zdrop;
 	if (mm_dbg_flag & MM_DBG_PRINT_ALN_SEQ) {
 		int i;
 		fprintf(stderr, "===> q=(%d,%d), e=(%d,%d), bw=%d, flag=%d, zdrop=%d <===\n", opt->q, opt->q2, opt->e, opt->e2, w, flag, opt->zdrop);
 		for (i = 0; i < tlen; ++i) fputc("ACGTN"[tseq[i]], stderr);
 		fputc('\n', stderr);
 		for (i = 0; i < qlen; ++i) fputc("ACGTN"[qseq[i]], stderr);
 		fputc('\n', stderr);
@@ -287,41 +310,47 @@
 		}
 		if (max_diff > diff_thres && max_diff > max)
 			max = max_diff, max_st = k, max_en = max_diff_l;
 	}
 	kfree(km, K);
 }
 
-static void mm_fix_bad_ends(const mm_reg1_t *r, const mm128_t *a, int bw, int32_t *as, int32_t *cnt)
+static void mm_fix_bad_ends(const mm_reg1_t *r, const mm128_t *a, int bw, int min_match, int32_t *as, int32_t *cnt)
 {
-	int32_t i, l;
+	int32_t i, l, m;
 	*as = r->as, *cnt = r->cnt;
 	if (r->cnt < 3) return;
-	l = a[r->as].y >> 32 & 0xff;
+	m = l = a[r->as].y >> 32 & 0xff;
 	for (i = r->as + 1; i < r->as + r->cnt - 1; ++i) {
 		int32_t lq, lr, min, max;
+		int32_t q_span = a[i].y >> 32 & 0xff;
+		if (a[i].y & MM_SEED_LONG_JOIN) break;
 		lr = (int32_t)a[i].x - (int32_t)a[i-1].x;
 		lq = (int32_t)a[i].y - (int32_t)a[i-1].y;
 		min = lr < lq? lr : lq;
 		max = lr > lq? lr : lq;
 		if (max - min > l >> 1) *as = i;
 		l += min;
-		if (l >= bw << 1) break;
+		m += min < q_span? min : q_span;
+		if (l >= bw << 1 || (m >= min_match && m >= bw) || m >= r->mlen >> 1) break;
 	}
 	*cnt = r->as + r->cnt - *as;
-	l = a[r->as + r->cnt - 1].y >> 32 & 0xff;
+	m = l = a[r->as + r->cnt - 1].y >> 32 & 0xff;
 	for (i = r->as + r->cnt - 2; i > *as; --i) {
 		int32_t lq, lr, min, max;
+		int32_t q_span = a[i+1].y >> 32 & 0xff;
+		if (a[i+1].y & MM_SEED_LONG_JOIN) break;
 		lr = (int32_t)a[i+1].x - (int32_t)a[i].x;
 		lq = (int32_t)a[i+1].y - (int32_t)a[i].y;
 		min = lr < lq? lr : lq;
 		max = lr > lq? lr : lq;
 		if (max - min > l >> 1) *cnt = i + 1 - *as;
 		l += min;
-		if (l >= bw) break;
+		m += min < q_span? min : q_span;
+		if (l >= bw << 1 || (m >= min_match && m >= bw) || m >= r->mlen >> 1) break;
 	}
 }
 
 static void mm_max_stretch(const mm_mapopt_t *opt, const mm_reg1_t *r, const mm128_t *a, int32_t *as, int32_t *cnt)
 {
 	int32_t i, score, max_score, len, max_i, max_len;
 
@@ -414,15 +443,15 @@
 		qs = (int32_t)a[as1].y + 1 - (int32_t)(a[as1].y>>32&0xff);
 		re = (int32_t)a[as1+cnt1-1].x + 1;
 		qe = (int32_t)a[as1+cnt1-1].y + 1;
 	} else {
 		if (is_splice) {
 			mm_fix_bad_ends_splice(km, opt, mi, r, mat, qlen, qseq0, a, &as1, &cnt1);
 		} else {
-			mm_fix_bad_ends(r, a, opt->bw, &as1, &cnt1);
+			mm_fix_bad_ends(r, a, opt->bw, opt->min_chain_score * 2, &as1, &cnt1);
 		}
 		mm_filter_bad_seeds(km, as1, cnt1, a, 10, 40, opt->max_gap>>1, 10);
 		mm_adjust_minier(mi, qseq0, &a[as1], &rs, &qs);
 		mm_adjust_minier(mi, qseq0, &a[as1 + cnt1 - 1], &re, &qe);
 	}
 	assert(cnt1 > 0);
 
@@ -512,15 +541,15 @@
 	tseq = (uint8_t*)kmalloc(km, re0 - rs0);
 
 	if (qs > 0 && rs > 0) { // left extension
 		qseq = &qseq0[rev][qs0];
 		mm_idx_getseq(mi, rid, rs0, rs, tseq);
 		mm_seq_rev(qs - qs0, qseq);
 		mm_seq_rev(rs - rs0, tseq);
-		mm_align_pair(km, opt, qs - qs0, qseq, rs - rs0, tseq, mat, bw, opt->end_bonus, extra_flag|KSW_EZ_EXTZ_ONLY|KSW_EZ_RIGHT|KSW_EZ_REV_CIGAR, ez);
+		mm_align_pair(km, opt, qs - qs0, qseq, rs - rs0, tseq, mat, bw, opt->end_bonus, r->split_inv? opt->zdrop_inv : opt->zdrop, extra_flag|KSW_EZ_EXTZ_ONLY|KSW_EZ_RIGHT|KSW_EZ_REV_CIGAR, ez);
 		if (ez->n_cigar > 0) {
 			mm_append_cigar(r, ez->n_cigar, ez->cigar);
 			r->p->dp_score += ez->max;
 		}
 		rs1 = rs - (ez->reach_end? ez->mqe_t + 1 : ez->max_t + 1);
 		qs1 = qs - (ez->reach_end? qs - qs0 : ez->max_q + 1);
 		mm_seq_rev(qs - qs0, qseq);
@@ -532,55 +561,60 @@
 		if ((a[as1+i].y & (MM_SEED_IGNORE|MM_SEED_TANDEM)) && i != cnt1 - 1) continue;
 		if (is_sr && !(mi->flag & MM_I_HPC)) {
 			re = (int32_t)a[as1 + i].x + 1;
 			qe = (int32_t)a[as1 + i].y + 1;
 		} else mm_adjust_minier(mi, qseq0, &a[as1 + i], &re, &qe);
 		re1 = re, qe1 = qe;
 		if (i == cnt1 - 1 || (a[as1+i].y&MM_SEED_LONG_JOIN) || (qe - qs >= opt->min_ksw_len && re - rs >= opt->min_ksw_len)) {
-			int j, bw1 = bw;
+			int j, bw1 = bw, zdrop_code;
 			if (a[as1+i].y & MM_SEED_LONG_JOIN)
 				bw1 = qe - qs > re - rs? qe - qs : re - rs;
+			// perform alignment
 			qseq = &qseq0[rev][qs];
 			mm_idx_getseq(mi, rid, rs, re, tseq);
 			if (is_sr) { // perform ungapped alignment
 				assert(qe - qs == re - rs);
 				ksw_reset_extz(ez);
 				for (j = 0, ez->score = 0; j < qe - qs; ++j) {
 					if (qseq[j] >= 4 || tseq[j] >= 4) ez->score += opt->e2;
 					else ez->score += qseq[j] == tseq[j]? opt->a : -opt->b;
 				}
 				ez->cigar = ksw_push_cigar(km, &ez->n_cigar, &ez->m_cigar, ez->cigar, 0, qe - qs);
 			} else { // perform normal gapped alignment
-				mm_align_pair(km, opt, qe - qs, qseq, re - rs, tseq, mat, bw1, -1, extra_flag|KSW_EZ_APPROX_MAX, ez); // first pass: with approximate Z-drop
+				mm_align_pair(km, opt, qe - qs, qseq, re - rs, tseq, mat, bw1, -1, opt->zdrop, extra_flag|KSW_EZ_APPROX_MAX, ez); // first pass: with approximate Z-drop
 			}
-			if (mm_check_zdrop(qseq, tseq, ez->n_cigar, ez->cigar, mat, opt->q, opt->e, opt->zdrop))
-				mm_align_pair(km, opt, qe - qs, qseq, re - rs, tseq, mat, bw1, -1, extra_flag, ez); // second pass: lift approximate
+			// test Z-drop and inversion Z-drop
+			if ((zdrop_code = mm_test_zdrop(km, opt, qseq, tseq, ez->n_cigar, ez->cigar, mat)) != 0)
+				mm_align_pair(km, opt, qe - qs, qseq, re - rs, tseq, mat, bw1, -1, zdrop_code == 2? opt->zdrop_inv : opt->zdrop, extra_flag, ez); // second pass: lift approximate
+			// update CIGAR
 			if (ez->n_cigar > 0)
 				mm_append_cigar(r, ez->n_cigar, ez->cigar);
 			if (ez->zdropped) { // truncated by Z-drop; TODO: sometimes Z-drop kicks in because the next seed placement is wrong. This can be fixed in principle.
 				for (j = i - 1; j >= 0; --j)
 					if ((int32_t)a[as1 + j].x <= rs + ez->max_t)
 						break;
 				dropped = 1;
 				if (j < 0) j = 0;
 				r->p->dp_score += ez->max;
 				re1 = rs + (ez->max_t + 1);
 				qe1 = qs + (ez->max_q + 1);
-				if (cnt1 - (j + 1) >= opt->min_cnt)
+				if (cnt1 - (j + 1) >= opt->min_cnt) {
 					mm_split_reg(r, r2, as1 + j + 1 - r->as, qlen, a);
+					if (zdrop_code == 2) r2->split_inv = 1;
+				}
 				break;
 			} else r->p->dp_score += ez->score;
 			rs = re, qs = qe;
 		}
 	}
 
 	if (!dropped && qe < qe0 && re < re0) { // right extension
 		qseq = &qseq0[rev][qe];
 		mm_idx_getseq(mi, rid, re, re0, tseq);
-		mm_align_pair(km, opt, qe0 - qe, qseq, re0 - re, tseq, mat, bw, opt->end_bonus, extra_flag|KSW_EZ_EXTZ_ONLY, ez);
+		mm_align_pair(km, opt, qe0 - qe, qseq, re0 - re, tseq, mat, bw, opt->end_bonus, opt->zdrop, extra_flag|KSW_EZ_EXTZ_ONLY, ez);
 		if (ez->n_cigar > 0) {
 			mm_append_cigar(r, ez->n_cigar, ez->cigar);
 			r->p->dp_score += ez->max;
 		}
 		re1 = re + (ez->reach_end? ez->mqe_t + 1 : ez->max_t + 1);
 		qe1 = qe + (ez->reach_end? qe0 - qe : ez->max_q + 1);
 	}
@@ -609,45 +643,52 @@
 	void *qp;
 
 	memset(r_inv, 0, sizeof(mm_reg1_t));
 	if (!(r1->split&1) || !(r2->split&2)) return 0;
 	if (r1->id != r1->parent && r1->parent != MM_PARENT_TMP_PRI) return 0;
 	if (r2->id != r2->parent && r2->parent != MM_PARENT_TMP_PRI) return 0;
 	if (r1->rid != r2->rid || r1->rev != r2->rev) return 0;
-	ql = r2->qs - r1->qe;
+	ql = r1->rev? r1->qs - r2->qe : r2->qs - r1->qe;
 	tl = r2->rs - r1->re;
 	if (ql < opt->min_chain_score || ql > opt->max_gap) return 0;
 	if (tl < opt->min_chain_score || tl > opt->max_gap) return 0;
 
 	ksw_gen_simple_mat(5, mat, opt->a, opt->b);
 	tseq = (uint8_t*)kmalloc(km, tl);
 	mm_idx_getseq(mi, r1->rid, r1->re, r2->rs, tseq);
-	qseq = &qseq0[!r1->rev][qlen - r2->qs];
+	qseq = r1->rev? &qseq0[0][r2->qe] : &qseq0[1][qlen - r2->qs];
 
 	mm_seq_rev(ql, qseq);
 	mm_seq_rev(tl, tseq);
 	qp = ksw_ll_qinit(km, 2, ql, qseq, 5, mat);
 	score = ksw_ll_i16(qp, tl, tseq, opt->q, opt->e, &q_off, &t_off);
 	kfree(km, qp);
 	mm_seq_rev(ql, qseq);
 	mm_seq_rev(tl, tseq);
 	if (score < opt->min_dp_max) goto end_align1_inv;
 	q_off = ql - (q_off + 1), t_off = tl - (t_off + 1);
-	mm_align_pair(km, opt, ql - q_off, qseq + q_off, tl - t_off, tseq + t_off, mat, (int)(opt->bw * 1.5), -1, KSW_EZ_EXTZ_ONLY, ez);
+	mm_align_pair(km, opt, ql - q_off, qseq + q_off, tl - t_off, tseq + t_off, mat, (int)(opt->bw * 1.5), -1, opt->zdrop, KSW_EZ_EXTZ_ONLY, ez);
 	if (ez->n_cigar == 0) goto end_align1_inv; // should never be here
 	mm_append_cigar(r_inv, ez->n_cigar, ez->cigar);
 	r_inv->p->dp_score = ez->max;
 	r_inv->id = -1;
 	r_inv->parent = MM_PARENT_UNSET;
 	r_inv->inv = 1;
 	r_inv->rev = !r1->rev;
 	r_inv->rid = r1->rid;
 	r_inv->div = -1.0f;
-	r_inv->qs = r1->qe + q_off, r_inv->qe = r_inv->qs + ez->max_q + 1;
-	r_inv->rs = r1->re + t_off, r_inv->re = r_inv->rs + ez->max_t + 1;
+	if (r_inv->rev == 0) {
+		r_inv->qs = r2->qe + q_off;
+		r_inv->qe = r_inv->qs + ez->max_q + 1;
+	} else {
+		r_inv->qe = r2->qs - q_off;
+		r_inv->qs = r_inv->qe - (ez->max_q + 1);
+	}
+	r_inv->rs = r1->re + t_off;
+	r_inv->re = r_inv->rs + ez->max_t + 1;
 	mm_update_extra(r_inv, &qseq[q_off], &tseq[t_off], mat, opt->q, opt->e);
 	ret = 1;
 end_align1_inv:
 	kfree(km, tseq);
 	return ret;
 }
 
@@ -700,21 +741,21 @@
 			regs[i].p->trans_strand = trans_strand;
 		} else { // one round of alignment
 			mm_align1(km, opt, mi, qlen, qseq0, &regs[i], &r2, n_a, a, &ez, opt->flag);
 			if (opt->flag&MM_F_SPLICE)
 				regs[i].p->trans_strand = opt->flag&MM_F_SPLICE_FOR? 1 : 2;
 		}
 		if (r2.cnt > 0) regs = mm_insert_reg(&r2, i, &n_regs, regs);
-		if (!(opt->flag&(MM_F_SPLICE|MM_F_SR)) && !(opt->flag&(MM_F_FOR_ONLY|MM_F_REV_ONLY)) && i > 0) { // don't try inversion alignment for -xsplice or -xsr, or --for-only/rev-only
+		if (i > 0 && regs[i].split_inv) {
 			if (mm_align1_inv(km, opt, mi, qlen, qseq0, &regs[i-1], &regs[i], &r2, &ez)) {
 				regs = mm_insert_reg(&r2, i, &n_regs, regs);
 				++i; // skip the inserted INV alignment
 			}
 		}
 	}
 	*n_regs_ = n_regs;
 	kfree(km, qseq0[0]);
 	kfree(km, ez.cigar);
-	mm_filter_regs(km, opt, n_regs_, regs);
+	mm_filter_regs(km, opt, qlen, n_regs_, regs);
 	mm_hit_sort_by_dp(km, n_regs_, regs);
 	return regs;
 }
```

### Comparing `mappy-2.8/bseq.c` & `mappy-2.9/bseq.c`

 * *Files 5% similar despite different names*

```diff
@@ -50,23 +50,31 @@
 void mm_bseq_close(mm_bseq_file_t *fp)
 {
 	kseq_destroy(fp->ks);
 	gzclose(fp->fp);
 	free(fp);
 }
 
+static inline char *kstrdup(const kstring_t *s)
+{
+	char *t;
+	t = (char*)malloc(s->l + 1);
+	memcpy(t, s->s, s->l + 1);
+	return t;
+}
+
 static inline void kseq2bseq(kseq_t *ks, mm_bseq1_t *s, int with_qual)
 {
 	int i;
-	s->name = strdup(ks->name.s);
-	s->seq = strdup(ks->seq.s);
+	s->name = kstrdup(&ks->name);
+	s->seq = kstrdup(&ks->seq);
 	for (i = 0; i < ks->seq.l; ++i) // convert U to T
 		if (s->seq[i] == 'u' || s->seq[i] == 'U')
 			--s->seq[i];
-	s->qual = with_qual && ks->qual.l? strdup(ks->qual.s) : 0;
+	s->qual = with_qual && ks->qual.l? kstrdup(&ks->qual) : 0;
 	s->l_seq = ks->seq.l;
 }
 
 mm_bseq1_t *mm_bseq_read2(mm_bseq_file_t *fp, int chunk_size, int with_qual, int frag_mode, int *n_)
 {
 	int64_t size = 0;
 	kvec_t(mm_bseq1_t) a = {0,0,0};
```

### Comparing `mappy-2.8/bseq.h` & `mappy-2.9/bseq.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/chain.c` & `mappy-2.9/chain.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/esterr.c` & `mappy-2.9/esterr.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/format.c` & `mappy-2.9/format.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/getopt.c` & `mappy-2.9/getopt.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/getopt.h` & `mappy-2.9/getopt.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/hit.c` & `mappy-2.9/hit.c`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 void mm_split_reg(mm_reg1_t *r, mm_reg1_t *r2, int n, int qlen, mm128_t *a)
 {
 	if (n <= 0 || n >= r->cnt) return;
 	*r2 = *r;
 	r2->id = -1;
 	r2->sam_pri = 0;
 	r2->p = 0;
+	r2->split_inv = 0;
 	r2->cnt = r->cnt - n;
 	r2->score = (int32_t)(r->score * ((float)r2->cnt / r->cnt) + .499);
 	r2->as = r->as + n;
 	if (r->parent == r->id) r2->parent = MM_PARENT_TMP_PRI;
 	mm_reg_set_coor(r2, qlen, a);
 	r->cnt -= r2->cnt;
 	r->score -= r2->score;
@@ -241,24 +242,25 @@
 			} else if (r[i].p) free(r[i].p);
 		}
 		if (k != n) mm_sync_regs(km, k, r); // removing hits requires sync()
 		*n_ = k;
 	}
 }
 
-void mm_filter_regs(void *km, const mm_mapopt_t *opt, int *n_regs, mm_reg1_t *regs)
+void mm_filter_regs(void *km, const mm_mapopt_t *opt, int qlen, int *n_regs, mm_reg1_t *regs)
 { // NB: after this call, mm_reg1_t::parent can be -1 if its parent filtered out
 	int i, k;
 	for (i = k = 0; i < *n_regs; ++i) {
 		mm_reg1_t *r = &regs[i];
 		int flt = 0;
 		if (!r->inv && !r->seg_split && r->cnt < opt->min_cnt) flt = 1;
-		if (r->p) {
+		if (r->p) { // these filters are only applied when base-alignment is available
 			if (r->mlen < opt->min_chain_score) flt = 1;
 			else if (r->p->dp_max < opt->min_dp_max) flt = 1;
+			else if (r->qs > qlen * opt->max_clip_ratio && qlen - r->qe > qlen * opt->max_clip_ratio) flt = 1;
 			if (flt) free(r->p);
 		}
 		if (!flt) {
 			if (k < i) regs[k++] = regs[i];
 			else ++k;
 		}
 	}
@@ -333,15 +335,15 @@
 		for (i = 0; i < n_regs; ++i) { // adjust the mm_reg1_t::parent
 			mm_reg1_t *r = &regs[i];
 			if (r->parent >= 0 && r->id != r->parent) { // fix for secondary hits only
 				if (regs[r->parent].parent >= 0 && regs[r->parent].parent != r->parent)
 					r->parent = regs[r->parent].parent;
 			}
 		}
-		mm_filter_regs(km, opt, n_regs_, regs);
+		mm_filter_regs(km, opt, qlen, n_regs_, regs);
 		mm_sync_regs(km, *n_regs_, regs);
 	}
 }
 
 mm_seg_t *mm_seg_gen(void *km, uint32_t hash, int n_segs, const int *qlens, int n_regs0, const mm_reg1_t *regs0, int *n_regs, mm_reg1_t **regs, const mm128_t *a)
 {
 	int s, i, j, acc_qlen[MM_MAX_SEG+1], qlen_sum = 0;
@@ -402,15 +404,41 @@
 {
 	int i;
 	for (i = 0; i < n_segs; ++i) kfree(km, segs[i].u);
 	for (i = 0; i < n_segs; ++i) kfree(km, segs[i].a);
 	kfree(km, segs);
 }
 
-void mm_set_mapq(int n_regs, mm_reg1_t *regs, int min_chain_sc, int match_sc, int rep_len, int is_sr)
+static void mm_set_inv_mapq(void *km, int n_regs, mm_reg1_t *regs)
+{
+	int i, n_aux;
+	uint64_t *aux;
+	if (n_regs < 3) return;
+	for (i = 0; i < n_regs; ++i)
+		if (regs[i].inv) break;
+	if (i == n_regs) return; // no inversion hits
+
+	aux = (uint64_t*)kmalloc(km, n_regs * 8);
+	for (i = n_aux = 0; i < n_regs; ++i)
+		if (regs[i].parent == i || regs[i].parent < 0)
+			aux[n_aux++] = (uint64_t)regs[i].as << 32 | i;
+	radix_sort_64(aux, aux + n_aux);
+
+	for (i = 1; i < n_aux - 1; ++i) {
+		mm_reg1_t *inv = &regs[(int32_t)aux[i]];
+		if (inv->inv) {
+			mm_reg1_t *l = &regs[(int32_t)aux[i-1]];
+			mm_reg1_t *r = &regs[(int32_t)aux[i+1]];
+			inv->mapq = l->mapq < r->mapq? l->mapq : r->mapq;
+		}
+	}
+	kfree(km, aux);
+}
+
+void mm_set_mapq(void *km, int n_regs, mm_reg1_t *regs, int min_chain_sc, int match_sc, int rep_len, int is_sr)
 {
 	static const float q_coef = 40.0f;
 	int64_t sum_sc = 0;
 	float uniq_ratio;
 	int i;
 	for (i = 0; i < n_regs; ++i)
 		if (regs[i].parent == regs[i].id)
@@ -445,8 +473,9 @@
 			}
 			mapq -= (int)(4.343f * logf(r->n_sub + 1) + .499f);
 			mapq = mapq > 0? mapq : 0;
 			r->mapq = mapq < 60? mapq : 60;
 			if (r->p && r->p->dp_max > r->p->dp_max2 && r->mapq == 0) r->mapq = 1;
 		} else r->mapq = 0;
 	}
+	mm_set_inv_mapq(km, n_regs, regs);
 }
```

### Comparing `mappy-2.8/index.c` & `mappy-2.9/index.c`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,25 @@
 #include "khash.h"
 
 #define idx_hash(a) ((a)>>1)
 #define idx_eq(a, b) ((a)>>1 == (b)>>1)
 KHASH_INIT(idx, uint64_t, uint64_t, 1, idx_hash, idx_eq)
 typedef khash_t(idx) idxhash_t;
 
+KHASH_MAP_INIT_STR(str, uint32_t)
+
 #define kroundup64(x) (--(x), (x)|=(x)>>1, (x)|=(x)>>2, (x)|=(x)>>4, (x)|=(x)>>8, (x)|=(x)>>16, (x)|=(x)>>32, ++(x))
 
 typedef struct mm_idx_bucket_s {
 	mm128_v a;   // (minimizer, position) array
 	int32_t n;   // size of the _p_ array
 	uint64_t *p; // position array for minimizers appearing >1 times
 	void *h;     // hash table indexing _p_ and minimizers appearing once
 } mm_idx_bucket_t;
 
-void mm_idxopt_init(mm_idxopt_t *opt)
-{
-	memset(opt, 0, sizeof(mm_idxopt_t));
-	opt->k = 15, opt->w = 10, opt->flag = 0;
-	opt->bucket_bits = 14;
-	opt->mini_batch_size = 50000000;
-	opt->batch_size = 4000000000ULL;
-}
-
 mm_idx_t *mm_idx_init(int w, int k, int b, int flag)
 {
 	mm_idx_t *mi;
 	if (k*2 < b) b = k * 2;
 	if (w < 1) w = 1;
 	mi = (mm_idx_t*)calloc(1, sizeof(mm_idx_t));
 	mi->w = w, mi->k = k, mi->b = b, mi->flag = flag;
@@ -50,14 +43,15 @@
 	return mi;
 }
 
 void mm_idx_destroy(mm_idx_t *mi)
 {
 	int i;
 	if (mi == 0) return;
+	if (mi->h) kh_destroy(str, (khash_t(str)*)mi->h);
 	for (i = 0; i < 1<<mi->b; ++i) {
 		free(mi->B[i].p);
 		free(mi->B[i].a.a);
 		kh_destroy(idx, (idxhash_t*)mi->B[i].h);
 	}
 	if (!mi->km) {
 		for (i = 0; i < mi->n_seq; ++i)
@@ -105,14 +99,42 @@
 				if (kh_key(h, k)&1) ++n1;
 			}
 	}
 	fprintf(stderr, "[M::%s::%.3f*%.2f] distinct minimizers: %d (%.2f%% are singletons); average occurrences: %.3lf; average spacing: %.3lf\n",
 			__func__, realtime() - mm_realtime0, cputime() / (realtime() - mm_realtime0), n, 100.0*n1/n, (double)sum / n, (double)len / sum);
 }
 
+int mm_idx_index_name(mm_idx_t *mi)
+{
+	khash_t(str) *h;
+	uint32_t i;
+	int has_dup = 0, absent;
+	if (mi->h) return 0;
+	h = kh_init(str);
+	for (i = 0; i < mi->n_seq; ++i) {
+		khint_t k;
+		k = kh_put(str, h, mi->seq[i].name, &absent);
+		if (absent) kh_val(h, k) = i;
+		else has_dup = 1;
+	}
+	mi->h = h;
+	if (has_dup && mm_verbose >= 2)
+		fprintf(stderr, "[WARNING] some database sequences have identical sequence names\n");
+	return has_dup;
+}
+
+int mm_idx_name2id(const mm_idx_t *mi, const char *name)
+{
+	khash_t(str) *h = (khash_t(str)*)mi->h;
+	khint_t k;
+	if (h == 0) return -2;
+	k = kh_get(str, h, name);
+	return k == kh_end(h)? -1 : kh_val(h, k);
+}
+
 int mm_idx_getseq(const mm_idx_t *mi, uint32_t rid, uint32_t st, uint32_t en, uint8_t *seq)
 {
 	uint64_t i, st1, en1;
 	if (rid >= mi->n_seq || st >= mi->seq[rid].len) return -1;
 	if (en > mi->seq[rid].len) en = mi->seq[rid].len;
 	st1 = mi->seq[rid].offset + st;
 	en1 = mi->seq[rid].offset + en;
```

### Comparing `mappy-2.8/kalloc.c` & `mappy-2.9/kalloc.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/kdq.h` & `mappy-2.9/kdq.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/khash.h` & `mappy-2.9/khash.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/kseq.h` & `mappy-2.9/kseq.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/ksort.h` & `mappy-2.9/ksort.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/ksw2.h` & `mappy-2.9/ksw2.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/ksw2_dispatch.c` & `mappy-2.9/ksw2_dispatch.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/ksw2_extd2_sse.c` & `mappy-2.9/ksw2_extd2_sse.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/ksw2_exts2_sse.c` & `mappy-2.9/ksw2_exts2_sse.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/ksw2_extz2_sse.c` & `mappy-2.9/ksw2_extz2_sse.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/ksw2_ll_sse.c` & `mappy-2.9/ksw2_ll_sse.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/kthread.c` & `mappy-2.9/kthread.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/kvec.h` & `mappy-2.9/kvec.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/main.c` & `mappy-2.9/main.c`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #include <stdio.h>
 #include <string.h>
 #include "bseq.h"
 #include "minimap.h"
 #include "mmpriv.h"
 #include "getopt.h"
 
-#define MM_VERSION "2.7-r671-dirty"
+#define MM_VERSION "2.9-r720"
 
 #ifdef __linux__
 #include <sys/resource.h>
 #include <sys/time.h>
 void liftrlimit()
 {
 	struct rlimit r;
@@ -46,14 +46,15 @@
 	{ "idx-no-seq",     no_argument,       0, 0 },
 	{ "end-seed-pen",   required_argument, 0, 0 },   // 21
 	{ "for-only",       no_argument,       0, 0 },   // 22
 	{ "rev-only",       no_argument,       0, 0 },   // 23
 	{ "heap-sort",      required_argument, 0, 0 },   // 24
 	{ "all-chain",      no_argument,       0, 'P' },
 	{ "dual",           required_argument, 0, 0 },   // 26
+	{ "max-clip-ratio", required_argument, 0, 0 },   // 27
 	{ "help",           no_argument,       0, 'h' },
 	{ "max-intron-len", required_argument, 0, 'G' },
 	{ "version",        no_argument,       0, 'V' },
 	{ "min-count",      required_argument, 0, 'n' },
 	{ "min-chain-score",required_argument, 0, 'm' },
 	{ "mask-level",     required_argument, 0, 'M' },
 	{ "min-dp-score",   required_argument, 0, 's' },
@@ -134,15 +135,14 @@
 		else if (c == 'Y') opt.flag |= MM_F_SOFTCLIP;
 		else if (c == 'L') opt.flag |= MM_F_LONG_CIGAR;
 		else if (c == 'T') opt.sdust_thres = atoi(optarg);
 		else if (c == 'n') opt.min_cnt = atoi(optarg);
 		else if (c == 'm') opt.min_chain_score = atoi(optarg);
 		else if (c == 'A') opt.a = atoi(optarg);
 		else if (c == 'B') opt.b = atoi(optarg);
-		else if (c == 'z') opt.zdrop = atoi(optarg);
 		else if (c == 's') opt.min_dp_max = atoi(optarg);
 		else if (c == 'C') opt.noncan = atoi(optarg);
 		else if (c == 'I') ipt.batch_size = mm_parse_num(optarg);
 		else if (c == 'K') opt.mini_batch_size = (int)mm_parse_num(optarg);
 		else if (c == 'R') rg = optarg;
 		else if (c == 'h') fp_help = stdout;
 		else if (c == '2') opt.flag |= MM_F_2_IO_THREADS;
@@ -159,14 +159,15 @@
 		else if (c == 0 && long_idx ==13) opt.flag |= MM_F_SR; // --sr
 		else if (c == 0 && long_idx ==17) opt.end_bonus = atoi(optarg); // --end-bonus
 		else if (c == 0 && long_idx ==18) opt.flag |= MM_F_INDEPEND_SEG; // --no-pairing
 		else if (c == 0 && long_idx ==20) ipt.flag |= MM_I_NO_SEQ; // --idx-no-seq
 		else if (c == 0 && long_idx ==21) opt.anchor_ext_shift = atoi(optarg); // --end-seed-pen
 		else if (c == 0 && long_idx ==22) opt.flag |= MM_F_FOR_ONLY; // --for-only
 		else if (c == 0 && long_idx ==23) opt.flag |= MM_F_REV_ONLY; // --rev-only
+		else if (c == 0 && long_idx ==27) opt.max_clip_ratio = atof(optarg); // --max-clip-ratio
 		else if (c == 0 && long_idx == 14) { // --frag
 			yes_or_no(&opt, MM_F_FRAG_MODE, long_idx, optarg, 1);
 		} else if (c == 0 && long_idx == 15) { // --secondary
 			yes_or_no(&opt, MM_F_NO_PRINT_2ND, long_idx, optarg, 0);
 		} else if (c == 0 && long_idx == 16) { // --cs
 			opt.flag |= MM_F_OUT_CS | MM_F_CIGAR;
 			if (optarg == 0 || strcmp(optarg, "short") == 0) {
@@ -203,14 +204,17 @@
 			else if (*optarg == 'f') opt.flag |= MM_F_SPLICE_FOR, opt.flag &= ~MM_F_SPLICE_REV; // match GT-AG
 			else if (*optarg == 'r') opt.flag |= MM_F_SPLICE_REV, opt.flag &= ~MM_F_SPLICE_FOR; // match CT-AC (reverse complement of GT-AG)
 			else if (*optarg == 'n') opt.flag &= ~(MM_F_SPLICE_FOR|MM_F_SPLICE_REV); // don't try to match the GT-AG signal
 			else {
 				fprintf(stderr, "[ERROR]\033[1;31m unrecognized cDNA direction\033[0m\n");
 				return 1;
 			}
+		} else if (c == 'z') {
+			opt.zdrop = opt.zdrop_inv = strtol(optarg, &s, 10);
+			if (*s == ',') opt.zdrop_inv = strtol(s + 1, &s, 10);
 		} else if (c == 'O') {
 			opt.q = opt.q2 = strtol(optarg, &s, 10);
 			if (*s == ',') opt.q2 = strtol(s + 1, &s, 10);
 		} else if (c == 'E') {
 			opt.e = opt.e2 = strtol(optarg, &s, 10);
 			if (*s == ',') opt.e2 = strtol(s + 1, &s, 10);
 		}
@@ -246,15 +250,15 @@
 		fprintf(fp_help, "    -p FLOAT     min secondary-to-primary score ratio [%g]\n", opt.pri_ratio);
 		fprintf(fp_help, "    -N INT       retain at most INT secondary alignments [%d]\n", opt.best_n);
 		fprintf(fp_help, "  Alignment:\n");
 		fprintf(fp_help, "    -A INT       matching score [%d]\n", opt.a);
 		fprintf(fp_help, "    -B INT       mismatch penalty [%d]\n", opt.b);
 		fprintf(fp_help, "    -O INT[,INT] gap open penalty [%d,%d]\n", opt.q, opt.q2);
 		fprintf(fp_help, "    -E INT[,INT] gap extension penalty; a k-long gap costs min{O1+k*E1,O2+k*E2} [%d,%d]\n", opt.e, opt.e2);
-		fprintf(fp_help, "    -z INT       Z-drop score [%d]\n", opt.zdrop);
+		fprintf(fp_help, "    -z INT[,INT] Z-drop score and inversion Z-drop score [%d,%d]\n", opt.zdrop, opt.zdrop_inv);
 		fprintf(fp_help, "    -s INT       minimal peak DP alignment score [%d]\n", opt.min_dp_max);
 		fprintf(fp_help, "    -u CHAR      how to find GT-AG. f:transcript strand, b:both strands, n:don't match GT-AG [n]\n");
 		fprintf(fp_help, "  Input/Output:\n");
 		fprintf(fp_help, "    -a           output in the SAM format (PAF by default)\n");
 		fprintf(fp_help, "    -Q           don't output base quality in SAM\n");
 		fprintf(fp_help, "    -L           write CIGAR with >65535 ops at the CG tag\n");
 		fprintf(fp_help, "    -R STR       SAM read group line in a format like '@RG\\tID:foo\\tSM:bar' []\n");
```

### Comparing `mappy-2.8/Makefile` & `mappy-2.9/Makefile`

 * *Files identical despite different names*

### Comparing `mappy-2.8/map.c` & `mappy-2.9/map.c`

 * *Files 0% similar despite different names*

```diff
@@ -336,24 +336,24 @@
 						i == regs0[j].as? 0 : ((int32_t)a[i].y - (int32_t)a[i-1].y) - ((int32_t)a[i].x - (int32_t)a[i-1].x));
 
 	chain_post(opt, max_chain_gap_ref, mi, b->km, qlen_sum, n_segs, qlens, &n_regs0, regs0, a);
 	if (!is_sr) mm_est_err(mi, qlen_sum, n_regs0, regs0, a, n_mini_pos, mini_pos);
 
 	if (n_segs == 1) { // uni-segment
 		regs0 = align_regs(opt, mi, b->km, qlens[0], seqs[0], &n_regs0, regs0, a);
-		mm_set_mapq(n_regs0, regs0, opt->min_chain_score, opt->a, rep_len, is_sr);
+		mm_set_mapq(b->km, n_regs0, regs0, opt->min_chain_score, opt->a, rep_len, is_sr);
 		n_regs[0] = n_regs0, regs[0] = regs0;
 	} else { // multi-segment
 		mm_seg_t *seg;
 		seg = mm_seg_gen(b->km, hash, n_segs, qlens, n_regs0, regs0, n_regs, regs, a); // split fragment chain to separate segment chains
 		free(regs0);
 		for (i = 0; i < n_segs; ++i) {
 			mm_set_parent(b->km, opt->mask_level, n_regs[i], regs[i], opt->a * 2 + opt->b); // update mm_reg1_t::parent
 			regs[i] = align_regs(opt, mi, b->km, qlens[i], seqs[i], &n_regs[i], regs[i], seg[i].a);
-			mm_set_mapq(n_regs[i], regs[i], opt->min_chain_score, opt->a, rep_len, is_sr);
+			mm_set_mapq(b->km, n_regs[i], regs[i], opt->min_chain_score, opt->a, rep_len, is_sr);
 		}
 		mm_seg_free(b->km, n_segs, seg);
 		if (n_segs == 2 && opt->pe_ori >= 0 && (opt->flag&MM_F_CIGAR))
 			mm_pair(b->km, max_chain_gap_ref, opt->pe_bonus, opt->a * 2 + opt->b, opt->a, qlens, n_regs, regs); // pairing
 	}
 
 	kfree(b->km, mv.a);
```

### Comparing `mappy-2.8/mappy.egg-info/PKG-INFO` & `mappy-2.9/mappy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mappy
-Version: 2.8
+Version: 2.9
 Summary: Minimap2 python binding
 Home-page: https://github.com/lh3/minimap2
 Author: Heng Li
 Author-email: lh3@me.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: ==============================
@@ -39,14 +39,16 @@
         The following Python script demonstrates the key functionality of mappy:
         
         .. code:: python
         
         	import mappy as mp
         	a = mp.Aligner("test/MT-human.fa")  # load or build index
         	if not a: raise Exception("ERROR: failed to load/build index")
+        	s = a.seq("MT_human", 100, 200)     # retrieve a subsequence from the index
+        	print(mp.revcomp(s))                # reverse complement
         	for name, seq, qual in mp.fastx_read("test/MT-orang.fa"): # read a fasta/q sequence
         		for hit in a.map(seq): # traverse alignments
         			print("{}\t{}\t{}\t{}".format(hit.ctg, hit.r_st, hit.r_en, hit.cigar_str))
         
         APIs
         ----
         
@@ -92,15 +94,23 @@
         
         	mappy.Aligner.map(seq, seq2=None)
         
         This method aligns :code:`seq` against the index. It is a generator, *yielding*
         a series of :code:`mappy.Alignment` objects. If :code:`seq2` is present, mappy
         performs paired-end alignment, assuming the two ends are in the FR orientation.
         Alignments of the two ends can be distinguished by the :code:`read_num` field
-        (see below).
+        (see Class mappy.Alignment below).
+        
+        .. code:: python
+        
+        	mappy.Aligner.seq(name, start=0, end=0x7fffffff)
+        
+        This method retrieves a (sub)sequence from the index and returns it as a Python
+        string. :code:`None` is returned if :code:`name` is not present in the index or
+        the start/end coordinates are invalid.
         
         Class mappy.Alignment
         ~~~~~~~~~~~~~~~~~~~~~
         
         This class describes an alignment. An object of this class has the following
         properties:
         
@@ -144,28 +154,37 @@
         ::
         
         	q_st  q_en  strand  ctg  ctg_len  r_st  r_en  mlen  blen  mapq  cg:Z:cigar_str
         
         It is effectively the PAF format without the QueryName and QueryLength columns
         (the first two columns in PAF).
         
-        Function mappy.fastx_read
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
+        Miscellaneous Functions
+        ~~~~~~~~~~~~~~~~~~~~~~~
         
         .. code:: python
         
-        	mappy.fastx_read(fn)
+        	mappy.fastx_read(fn, read_comment=False)
         
         This generator function opens a FASTA/FASTQ file and *yields* a
         :code:`(name,seq,qual)` tuple for each sequence entry. The input file may be
-        optionally gzip'd.
+        optionally gzip'd. If :code:`read_comment` is True, this generator yields
+        a :code:`(name,seq,qual,comment)` tuple instead.
+        
+        .. code:: python
+        
+        	mappy.revcomp(seq)
+        
+        Return the reverse complement of DNA string :code:`seq`. This function
+        recognizes IUB code and preserves the letter cases. Uracil :code:`U` is
+        complemented to :code:`A`.
         
 Keywords: sequence-alignment
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappy-2.8/mappy.egg-info/SOURCES.txt` & `mappy-2.9/mappy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mappy-2.8/minimap.h` & `mappy-2.9/minimap.h`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 typedef struct {
 	int32_t b, w, k, flag;
 	uint32_t n_seq;            // number of reference sequences
 	mm_idx_seq_t *seq;         // sequence name, length and offset
 	uint32_t *S;               // 4-bit packed sequence
 	struct mm_idx_bucket_s *B; // index (hidden)
-	void *km;
+	void *km, *h;
 } mm_idx_t;
 
 // minimap2 alignment
 typedef struct {
 	uint32_t capacity;                  // the capacity of cigar[]
 	int32_t dp_score, dp_max, dp_max2;  // DP score; score of the max-scoring segment; score of the best alternate mappings
 	uint32_t n_ambi:30, trans_strand:2; // number of ambiguous bases; transcript strand: 0 for unknown, 1 for +, 2 for -
@@ -78,15 +78,15 @@
 	int32_t score;          // DP alignment score
 	int32_t qs, qe, rs, re; // query start and end; reference start and end
 	int32_t parent, subsc;  // parent==id if primary; best alternate mapping score
 	int32_t as;             // offset in the a[] array (for internal uses only)
 	int32_t mlen, blen;     // seeded exact match length; seeded alignment block length
 	int32_t n_sub;          // number of suboptimal mappings
 	int32_t score0;         // initial chaining score (before chain merging/spliting)
-	uint32_t mapq:8, split:2, rev:1, inv:1, sam_pri:1, proper_frag:1, pe_thru:1, seg_split:1, seg_id:8, dummy:8;
+	uint32_t mapq:8, split:2, rev:1, inv:1, sam_pri:1, proper_frag:1, pe_thru:1, seg_split:1, seg_id:8, split_inv:1, dummy:7;
 	uint32_t hash;
 	float div;
 	mm_extra_t *p;
 } mm_reg1_t;
 
 // indexing and mapping options
 typedef struct {
@@ -112,19 +112,20 @@
 	int best_n;      // top best_n chains are subjected to DP alignment
 
 	int max_join_long, max_join_short;
 	int min_join_flank_sc;
 
 	int a, b, q, e, q2, e2; // matching score, mismatch, gap-open and gap-ext penalties
 	int noncan;      // cost of non-canonical splicing sites
-	int zdrop;       // break alignment if alignment score drops too fast along the diagonal
+	int zdrop, zdrop_inv;   // break alignment if alignment score drops too fast along the diagonal
 	int end_bonus;
 	int min_dp_max;  // drop an alignment if the score of the max scoring segment is below this threshold
 	int min_ksw_len;
 	int anchor_ext_len, anchor_ext_shift;
+	float max_clip_ratio; // drop an alignment if BOTH ends are clipped above this ratio
 
 	int pe_ori, pe_bonus;
 
 	float mid_occ_frac;  // only used by mm_mapopt_update(); see below
 	int32_t mid_occ;     // ignore seeds with occurrences above this threshold
 	int32_t max_occ;
 	int mini_batch_size; // size of a batch of query bases to process in parallel
@@ -292,14 +293,19 @@
  *
  * @return 0 on success; -1 if _fn_ can't be read
  */
 int mm_map_file(const mm_idx_t *idx, const char *fn, const mm_mapopt_t *opt, int n_threads);
 
 int mm_map_file_frag(const mm_idx_t *idx, int n_segs, const char **fn, const mm_mapopt_t *opt, int n_threads);
 
+// query sequence name and sequence in the minimap2 index
+int mm_idx_index_name(mm_idx_t *mi);
+int mm_idx_name2id(const mm_idx_t *mi, const char *name);
+int mm_idx_getseq(const mm_idx_t *mi, uint32_t rid, uint32_t st, uint32_t en, uint8_t *seq);
+
 // deprecated APIs for backward compatibility
 void mm_mapopt_init(mm_mapopt_t *opt);
 mm_idx_t *mm_idx_build(const char *fn, int w, int k, int flag, int n_threads);
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `mappy-2.8/misc.c` & `mappy-2.9/misc.c`

 * *Files 9% similar despite different names*

```diff
@@ -82,24 +82,38 @@
 	FileTimeToSystemTime(&ftUser, &stUser);
 
 	double kernelModeTime = ((stKernel.wHour * 60.) + stKernel.wMinute * 60.) + stKernel.wSecond * 1. + stKernel.wMilliseconds / 1000.;
 	double userModeTime = ((stUser.wHour * 60.) + stUser.wMinute * 60.) + stUser.wSecond * 1. + stUser.wMilliseconds / 1000.;
 
 	return kernelModeTime + userModeTime;
 }
+
+long peakrss(void) { return 0; }
 #else
 #include <sys/resource.h>
 #include <sys/time.h>
 
 double cputime(void)
 {
 	struct rusage r;
 	getrusage(RUSAGE_SELF, &r);
 	return r.ru_utime.tv_sec + r.ru_stime.tv_sec + 1e-6 * (r.ru_utime.tv_usec + r.ru_stime.tv_usec);
 }
+
+long peakrss(void)
+{
+	struct rusage r;
+	getrusage(RUSAGE_SELF, &r);
+#ifdef __linux__
+	return r.ru_maxrss * 1024;
+#else
+	return r.ru_maxrss;
+#endif
+}
+
 #endif /* WIN32 || _WIN32 */
 
 double realtime(void)
 {
 	struct timeval tp;
 	struct timezone tzp;
 	gettimeofday(&tp, &tzp);
```

### Comparing `mappy-2.8/mmpriv.h` & `mappy-2.9/mmpriv.h`

 * *Files 3% similar despite different names*

```diff
@@ -44,45 +44,45 @@
 	int n_u, n_a;
 	uint64_t *u;
 	mm128_t *a;
 } mm_seg_t;
 
 double cputime(void);
 double realtime(void);
+long peakrss(void);
 
 void radix_sort_128x(mm128_t *beg, mm128_t *end);
 void radix_sort_64(uint64_t *beg, uint64_t *end);
 uint32_t ks_ksmall_uint32_t(size_t n, uint32_t arr[], size_t kk);
 
 void mm_sketch(void *km, const char *str, int len, int w, int k, uint32_t rid, int is_hpc, mm128_v *p);
 
 void mm_write_sam_hdr(const mm_idx_t *mi, const char *rg, const char *ver, int argc, char *argv[]);
 void mm_write_paf(kstring_t *s, const mm_idx_t *mi, const mm_bseq1_t *t, const mm_reg1_t *r, void *km, int opt_flag);
 void mm_write_sam(kstring_t *s, const mm_idx_t *mi, const mm_bseq1_t *t, const mm_reg1_t *r, int n_regs, const mm_reg1_t *regs);
 void mm_write_sam2(kstring_t *s, const mm_idx_t *mi, const mm_bseq1_t *t, int seg_idx, int reg_idx, int n_seg, const int *n_regs, const mm_reg1_t *const* regs, void *km, int opt_flag);
 
 void mm_idxopt_init(mm_idxopt_t *opt);
 const uint64_t *mm_idx_get(const mm_idx_t *mi, uint64_t minier, int *n);
-int mm_idx_getseq(const mm_idx_t *mi, uint32_t rid, uint32_t st, uint32_t en, uint8_t *seq);
 int32_t mm_idx_cal_max_occ(const mm_idx_t *mi, float f);
 mm128_t *mm_chain_dp(int max_dist_x, int max_dist_y, int bw, int max_skip, int min_cnt, int min_sc, int is_cdna, int n_segs, int64_t n, mm128_t *a, int *n_u_, uint64_t **_u, void *km);
 mm_reg1_t *mm_align_skeleton(void *km, const mm_mapopt_t *opt, const mm_idx_t *mi, int qlen, const char *qstr, int *n_regs_, mm_reg1_t *regs, mm128_t *a);
 
 mm_reg1_t *mm_gen_regs(void *km, uint32_t hash, int qlen, int n_u, uint64_t *u, mm128_t *a);
 void mm_split_reg(mm_reg1_t *r, mm_reg1_t *r2, int n, int qlen, mm128_t *a);
 void mm_sync_regs(void *km, int n_regs, mm_reg1_t *regs);
 int mm_squeeze_a(void *km, int n_regs, mm_reg1_t *regs, mm128_t *a);
 int mm_set_sam_pri(int n, mm_reg1_t *r);
 void mm_set_parent(void *km, float mask_level, int n, mm_reg1_t *r, int sub_diff);
 void mm_select_sub(void *km, float pri_ratio, int min_diff, int best_n, int *n_, mm_reg1_t *r);
 void mm_select_sub_multi(void *km, float pri_ratio, float pri1, float pri2, int max_gap_ref, int min_diff, int best_n, int n_segs, const int *qlens, int *n_, mm_reg1_t *r);
-void mm_filter_regs(void *km, const mm_mapopt_t *opt, int *n_regs, mm_reg1_t *regs);
+void mm_filter_regs(void *km, const mm_mapopt_t *opt, int qlen, int *n_regs, mm_reg1_t *regs);
 void mm_join_long(void *km, const mm_mapopt_t *opt, int qlen, int *n_regs, mm_reg1_t *regs, mm128_t *a);
 void mm_hit_sort_by_dp(void *km, int *n_regs, mm_reg1_t *r);
-void mm_set_mapq(int n_regs, mm_reg1_t *regs, int min_chain_sc, int match_sc, int rep_len, int is_sr);
+void mm_set_mapq(void *km, int n_regs, mm_reg1_t *regs, int min_chain_sc, int match_sc, int rep_len, int is_sr);
 
 void mm_est_err(const mm_idx_t *mi, int qlen, int n_regs, mm_reg1_t *regs, const mm128_t *a, int32_t n, const uint64_t *mini_pos);
 
 mm_seg_t *mm_seg_gen(void *km, uint32_t hash, int n_segs, const int *qlens, int n_regs0, const mm_reg1_t *regs0, int *n_regs, mm_reg1_t **regs, const mm128_t *a);
 void mm_seg_free(void *km, int n_segs, mm_seg_t *segs);
 void mm_pair(void *km, int max_gap_ref, int dp_bonus, int sub_diff, int match_sc, const int *qlens, int *n_regs, mm_reg1_t **regs);
```

### Comparing `mappy-2.8/options.c` & `mappy-2.9/options.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #include <stdio.h>
 #include "mmpriv.h"
 
+void mm_idxopt_init(mm_idxopt_t *opt)
+{
+	memset(opt, 0, sizeof(mm_idxopt_t));
+	opt->k = 15, opt->w = 10, opt->flag = 0;
+	opt->bucket_bits = 14;
+	opt->mini_batch_size = 50000000;
+	opt->batch_size = 4000000000ULL;
+}
+
 void mm_mapopt_init(mm_mapopt_t *opt)
 {
 	memset(opt, 0, sizeof(mm_mapopt_t));
 	opt->seed = 11;
 	opt->mid_occ_frac = 2e-4f;
 	opt->sdust_thres = 0; // no SDUST masking
 
@@ -20,19 +29,20 @@
 	opt->best_n = 5;
 
 	opt->max_join_long = 20000;
 	opt->max_join_short = 2000;
 	opt->min_join_flank_sc = 1000;
 
 	opt->a = 2, opt->b = 4, opt->q = 4, opt->e = 2, opt->q2 = 24, opt->e2 = 1;
-	opt->zdrop = 400;
+	opt->zdrop = 400, opt->zdrop_inv = 200;
 	opt->end_bonus = -1;
 	opt->min_dp_max = opt->min_chain_score * opt->a;
 	opt->min_ksw_len = 200;
 	opt->anchor_ext_len = 20, opt->anchor_ext_shift = 6;
+	opt->max_clip_ratio = 1.0f;
 	opt->mini_batch_size = 500000000;
 
 	opt->pe_ori = 0; // FF
 	opt->pe_bonus = 33;
 }
 
 void mm_mapopt_update(mm_mapopt_t *opt, const mm_idx_t *mi)
@@ -66,28 +76,28 @@
 		mo->min_chain_score = 100, mo->pri_ratio = 0.0f, mo->max_gap = 10000, mo->max_chain_skip = 25;
 	} else if (strcmp(preset, "map10k") == 0 || strcmp(preset, "map-pb") == 0) {
 		io->flag |= MM_I_HPC, io->k = 19;
 	} else if (strcmp(preset, "map-ont") == 0) {
 		io->flag = 0, io->k = 15;
 	} else if (strcmp(preset, "asm5") == 0) {
 		io->flag = 0, io->k = 19, io->w = 19;
-		mo->a = 1, mo->b = 19, mo->q = 39, mo->q2 = 81, mo->e = 3, mo->e2 = 1, mo->zdrop = 200;
+		mo->a = 1, mo->b = 19, mo->q = 39, mo->q2 = 81, mo->e = 3, mo->e2 = 1, mo->zdrop = mo->zdrop_inv = 200;
 		mo->min_dp_max = 200;
 		mo->best_n = 50;
 	} else if (strcmp(preset, "asm10") == 0) {
 		io->flag = 0, io->k = 19, io->w = 19;
-		mo->a = 1, mo->b = 9, mo->q = 16, mo->q2 = 41, mo->e = 2, mo->e2 = 1, mo->zdrop = 200;
+		mo->a = 1, mo->b = 9, mo->q = 16, mo->q2 = 41, mo->e = 2, mo->e2 = 1, mo->zdrop = mo->zdrop_inv = 200;
 		mo->min_dp_max = 200;
 		mo->best_n = 50;
 	} else if (strcmp(preset, "short") == 0 || strcmp(preset, "sr") == 0) {
 		io->flag = 0, io->k = 21, io->w = 11;
 		mo->flag |= MM_F_SR | MM_F_FRAG_MODE | MM_F_NO_PRINT_2ND | MM_F_2_IO_THREADS | MM_F_HEAP_SORT;
 		mo->pe_ori = 0<<1|1; // FR
 		mo->a = 2, mo->b = 8, mo->q = 12, mo->e = 2, mo->q2 = 24, mo->e2 = 1;
-		mo->zdrop = 100;
+		mo->zdrop = mo->zdrop_inv = 100;
 		mo->end_bonus = 10;
 		mo->max_frag_len = 800;
 		mo->max_gap = 100;
 		mo->bw = 100;
 		mo->pri_ratio = 0.5f;
 		mo->min_cnt = 2;
 		mo->min_chain_score = 25;
@@ -98,15 +108,15 @@
 		mo->mini_batch_size = 50000000;
 	} else if (strcmp(preset, "splice") == 0 || strcmp(preset, "cdna") == 0) {
 		io->flag = 0, io->k = 15, io->w = 5;
 		mo->flag |= MM_F_SPLICE | MM_F_SPLICE_FOR | MM_F_SPLICE_REV | MM_F_SPLICE_FLANK;
 		mo->max_gap = 2000, mo->max_gap_ref = mo->bw = 200000;
 		mo->a = 1, mo->b = 2, mo->q = 2, mo->e = 1, mo->q2 = 32, mo->e2 = 0;
 		mo->noncan = 9;
-		mo->zdrop = 200;
+		mo->zdrop = 200, mo->zdrop_inv = 100; // because mo->a is halved
 	} else return -1;
 	return 0;
 }
 
 int mm_check_opt(const mm_idxopt_t *io, const mm_mapopt_t *mo)
 {
 	if (mo->best_n < 0) {
@@ -132,9 +142,14 @@
 		return -2;
 	}
 	if ((mo->q + mo->e) + (mo->q2 + mo->e2) > 127) {
 		if (mm_verbose >= 1)
 			fprintf(stderr, "[ERROR]\033[1;31m scoring system violating ({-O}+{-E})+({-O2}+{-E2}) <= 127\033[0m\n");
 		return -1;
 	}
+	if (mo->zdrop < mo->zdrop_inv) {
+		if (mm_verbose >= 1)
+			fprintf(stderr, "[ERROR]\033[1;31m Z-drop should not be less than inversion-Z-drop\033[0m\n");
+		return -5;
+	}
 	return 0;
 }
```

### Comparing `mappy-2.8/pe.c` & `mappy-2.9/pe.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/PKG-INFO` & `mappy-2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mappy
-Version: 2.8
+Version: 2.9
 Summary: Minimap2 python binding
 Home-page: https://github.com/lh3/minimap2
 Author: Heng Li
 Author-email: lh3@me.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: ==============================
@@ -39,14 +39,16 @@
         The following Python script demonstrates the key functionality of mappy:
         
         .. code:: python
         
         	import mappy as mp
         	a = mp.Aligner("test/MT-human.fa")  # load or build index
         	if not a: raise Exception("ERROR: failed to load/build index")
+        	s = a.seq("MT_human", 100, 200)     # retrieve a subsequence from the index
+        	print(mp.revcomp(s))                # reverse complement
         	for name, seq, qual in mp.fastx_read("test/MT-orang.fa"): # read a fasta/q sequence
         		for hit in a.map(seq): # traverse alignments
         			print("{}\t{}\t{}\t{}".format(hit.ctg, hit.r_st, hit.r_en, hit.cigar_str))
         
         APIs
         ----
         
@@ -92,15 +94,23 @@
         
         	mappy.Aligner.map(seq, seq2=None)
         
         This method aligns :code:`seq` against the index. It is a generator, *yielding*
         a series of :code:`mappy.Alignment` objects. If :code:`seq2` is present, mappy
         performs paired-end alignment, assuming the two ends are in the FR orientation.
         Alignments of the two ends can be distinguished by the :code:`read_num` field
-        (see below).
+        (see Class mappy.Alignment below).
+        
+        .. code:: python
+        
+        	mappy.Aligner.seq(name, start=0, end=0x7fffffff)
+        
+        This method retrieves a (sub)sequence from the index and returns it as a Python
+        string. :code:`None` is returned if :code:`name` is not present in the index or
+        the start/end coordinates are invalid.
         
         Class mappy.Alignment
         ~~~~~~~~~~~~~~~~~~~~~
         
         This class describes an alignment. An object of this class has the following
         properties:
         
@@ -144,28 +154,37 @@
         ::
         
         	q_st  q_en  strand  ctg  ctg_len  r_st  r_en  mlen  blen  mapq  cg:Z:cigar_str
         
         It is effectively the PAF format without the QueryName and QueryLength columns
         (the first two columns in PAF).
         
-        Function mappy.fastx_read
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
+        Miscellaneous Functions
+        ~~~~~~~~~~~~~~~~~~~~~~~
         
         .. code:: python
         
-        	mappy.fastx_read(fn)
+        	mappy.fastx_read(fn, read_comment=False)
         
         This generator function opens a FASTA/FASTQ file and *yields* a
         :code:`(name,seq,qual)` tuple for each sequence entry. The input file may be
-        optionally gzip'd.
+        optionally gzip'd. If :code:`read_comment` is True, this generator yields
+        a :code:`(name,seq,qual,comment)` tuple instead.
+        
+        .. code:: python
+        
+        	mappy.revcomp(seq)
+        
+        Return the reverse complement of DNA string :code:`seq`. This function
+        recognizes IUB code and preserves the letter cases. Uracil :code:`U` is
+        complemented to :code:`A`.
         
 Keywords: sequence-alignment
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappy-2.8/python/cmappy.h` & `mappy-2.9/python/cmappy.h`

 * *Files 23% similar despite different names*

```diff
@@ -97,8 +97,37 @@
 		regs[0] = (mm_reg1_t*)realloc(regs[0], sizeof(mm_reg1_t) * (*n_regs));
 		memcpy(&regs[0][_n_regs[0]], regs[1], _n_regs[1] * sizeof(mm_reg1_t));
 		free(regs[1]);
 		return regs[0];
 	}
 }
 
+static inline char *mappy_revcomp(int len, const uint8_t *seq)
+{
+	int i;
+	char *rev;
+	rev = (char*)malloc(len + 1);
+	for (i = 0; i < len; ++i)
+		rev[len - i - 1] = seq_comp_table[seq[i]];
+	rev[len] = 0;
+	return rev;
+}
+
+static char *mappy_fetch_seq(const mm_idx_t *mi, const char *name, int st, int en, int *len)
+{
+	int i, rid;
+	char *s;
+	*len = 0;
+	rid = mm_idx_name2id(mi, name);
+	if (rid < 0) return 0;
+	if (st >= mi->seq[i].len || st >= en) return 0;
+	if (en < 0 || en > mi->seq[i].len)
+		en = mi->seq[i].len;
+	s = (char*)malloc(en - st + 1);
+	*len = mm_idx_getseq(mi, rid, st, en, s);
+	for (i = 0; i < *len; ++i)
+		s[i] = "ACGTN"[(uint8_t)s[i]];
+	s[*len] = 0;
+	return s;
+}
+
 #endif
```

### Comparing `mappy-2.8/python/cmappy.pxd` & `mappy-2.9/python/cmappy.pxd`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 		float mask_level
 		float pri_ratio
 		int best_n
 		int max_join_long, max_join_short
 		int min_join_flank_sc
 		int a, b, q, e, q2, e2
 		int noncan
-		int zdrop
+		int zdrop, zdrop_inv
 		int end_bonus
 		int min_dp_max
 		int min_ksw_len
 		int anchor_ext_len, anchor_ext_shift
+		float max_clip_ratio
 		int pe_ori, pe_bonus
 		float mid_occ_frac
 		int32_t mid_occ
 		int32_t max_occ
 		int mini_batch_size
 
 	int mm_set_opt(char *preset, mm_idxopt_t *io, mm_mapopt_t *mo)
@@ -53,25 +54,27 @@
 
 	ctypedef struct mm_idx_t:
 		int32_t b, w, k, flag
 		uint32_t n_seq
 		mm_idx_seq_t *seq
 		uint32_t *S
 		mm_idx_bucket_t *B
-		void *km
+		void *km, *h
 
 	ctypedef struct mm_idx_reader_t:
 		pass
 
 	mm_idx_reader_t *mm_idx_reader_open(const char *fn, const mm_idxopt_t *opt, const char *fn_out)
 	mm_idx_t *mm_idx_reader_read(mm_idx_reader_t *r, int n_threads)
 	void mm_idx_reader_close(mm_idx_reader_t *r)
 	void mm_idx_destroy(mm_idx_t *mi)
 	void mm_mapopt_update(mm_mapopt_t *opt, const mm_idx_t *mi)
 
+	int mm_idx_index_name(mm_idx_t *mi)
+
 	#
 	# Mapping (key struct defined in cmappy.h below)
 	#
 	ctypedef struct mm_reg1_t:
 		pass
 
 	ctypedef struct mm_tbuf_t:
@@ -94,14 +97,15 @@
 		int32_t seg_id
 		int32_t n_cigar32
 		uint32_t *cigar32
 
 	void mm_reg2hitpy(const mm_idx_t *mi, mm_reg1_t *r, mm_hitpy_t *h)
 	void mm_free_reg1(mm_reg1_t *r)
 	mm_reg1_t *mm_map_aux(const mm_idx_t *mi, const char *seq1, const char *seq2, int *n_regs, mm_tbuf_t *b, const mm_mapopt_t *opt)
+	char *mappy_fetch_seq(const mm_idx_t *mi, const char *name, int st, int en, int *l)
 
 	ctypedef struct kstring_t:
 		unsigned l, m
 		char *s
 
 	ctypedef struct kstream_t:
 		pass
@@ -111,9 +115,10 @@
 		int last_char
 		kstream_t *f
 
 	kseq_t *mm_fastx_open(const char *fn)
 	void mm_fastx_close(kseq_t *ks)
 	int kseq_read(kseq_t *seq)
 
+	char *mappy_revcomp(int l, const uint8_t *seq)
 	int mm_verbose_level(int v)
 	void mm_reset_timer()
```

### Comparing `mappy-2.8/python/mappy.c` & `mappy-2.9/python/mappy.c`

 * *Files 1% similar despite different names*

```diff
@@ -691,15 +691,15 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_5mappy_Alignment;
 struct __pyx_obj_5mappy_ThreadBuffer;
 struct __pyx_obj_5mappy_Aligner;
 struct __pyx_obj_5mappy___pyx_scope_struct__map;
 struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read;
 
-/* "mappy.pyx":7
+/* "mappy.pyx":8
  * cmappy.mm_reset_timer()
  * 
  * cdef class Alignment:             # <<<<<<<<<<<<<<
  * 	cdef int _ctg_len, _r_st, _r_en
  * 	cdef int _q_st, _q_en
  */
 struct __pyx_obj_5mappy_Alignment {
@@ -718,51 +718,53 @@
   uint8_t _is_primary;
   int _seg_id;
   PyObject *_ctg;
   PyObject *_cigar;
 };
 
 
-/* "mappy.pyx":88
+/* "mappy.pyx":89
  * 				str(self._mlen), str(self._blen), str(self._mapq), tp, ts, "cg:Z:" + self.cigar_str])
  * 
  * cdef class ThreadBuffer:             # <<<<<<<<<<<<<<
  * 	cdef cmappy.mm_tbuf_t *_b
  * 
  */
 struct __pyx_obj_5mappy_ThreadBuffer {
   PyObject_HEAD
   mm_tbuf_t *_b;
 };
 
 
-/* "mappy.pyx":97
+/* "mappy.pyx":98
  * 		cmappy.mm_tbuf_destroy(self._b)
  * 
  * cdef class Aligner:             # <<<<<<<<<<<<<<
  * 	cdef cmappy.mm_idx_t *_idx
  * 	cdef cmappy.mm_idxopt_t idx_opt
  */
 struct __pyx_obj_5mappy_Aligner {
   PyObject_HEAD
   mm_idx_t *_idx;
   mm_idxopt_t idx_opt;
   mm_mapopt_t map_opt;
 };
 
 
-/* "mappy.pyx":133
+/* "mappy.pyx":135
  * 		return (self._idx != NULL)
  * 
  * 	def map(self, seq, seq2=None, buf=None):             # <<<<<<<<<<<<<<
  * 		cdef cmappy.mm_reg1_t *regs
  * 		cdef cmappy.mm_hitpy_t h
  */
 struct __pyx_obj_5mappy___pyx_scope_struct__map {
   PyObject_HEAD
+  PyObject *__pyx_v__seq;
+  PyObject *__pyx_v__seq2;
   struct __pyx_obj_5mappy_ThreadBuffer *__pyx_v_b;
   PyObject *__pyx_v_buf;
   PyObject *__pyx_v_c;
   PyObject *__pyx_v_cigar;
   mm_hitpy_t __pyx_v_h;
   int __pyx_v_i;
   int32_t __pyx_v_k;
@@ -772,27 +774,29 @@
   PyObject *__pyx_v_seq;
   PyObject *__pyx_v_seq2;
   int __pyx_t_0;
   int __pyx_t_1;
 };
 
 
-/* "mappy.pyx":155
- * 		free(regs)
+/* "mappy.pyx":179
+ * 	def n_seq(self): return self._idx.n_seq
  * 
- * def fastx_read(fn):             # <<<<<<<<<<<<<<
+ * def fastx_read(fn, read_comment=False):             # <<<<<<<<<<<<<<
  * 	cdef cmappy.kseq_t *ks
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))
  */
 struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read {
   PyObject_HEAD
+  PyObject *__pyx_v_comment;
   PyObject *__pyx_v_fn;
   kseq_t *__pyx_v_ks;
   PyObject *__pyx_v_name;
   PyObject *__pyx_v_qual;
+  PyObject *__pyx_v_read_comment;
   PyObject *__pyx_v_seq;
 };
 
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
@@ -1051,32 +1055,14 @@
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* KeywordStringCheck.proto */
 static CYTHON_INLINE int __Pyx_CheckKeywordStrings(PyObject *kwdict, const char* function_name, int kw_allowed);
 
-/* PyObjectSetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o,n,NULL)
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_setattro))
-        return tp->tp_setattro(obj, attr_name, value);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_setattr))
-        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
-#endif
-    return PyObject_SetAttr(obj, attr_name, value);
-}
-#else
-#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
-#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
-#endif
-
 /* ReturnWithStopIteration.proto */
 #define __Pyx_ReturnWithStopIteration(value)\
     if (value == Py_None) PyErr_SetNone(PyExc_StopIteration); else __Pyx__ReturnWithStopIteration(value)
 static void __Pyx__ReturnWithStopIteration(PyObject* value);
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
@@ -1110,14 +1096,18 @@
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AndObjC(PyObject *op1, PyObject *op2, long intval, int inplace);
 #else
 #define __Pyx_PyInt_AndObjC(op1, op2, intval, inplace)\
     (inplace ? PyNumber_InPlaceAnd(op1, op2) : PyNumber_And(op1, op2))
 #endif
 
+/* ArgTypeTest.proto */
+static CYTHON_INLINE int __Pyx_ArgTypeTest(PyObject *obj, PyTypeObject *type, int none_allowed,
+    const char *name, int exact);
+
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
@@ -1136,14 +1126,17 @@
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
 /* CLineInTraceback.proto */
 static int __Pyx_CLineForTraceback(int c_line);
 
 /* CodeObjectCache.proto */
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
@@ -1278,14 +1271,17 @@
 
 /* Implementation of 'mappy' */
 static PyObject *__pyx_builtin_map;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_range;
 static const char __pyx_k_[] = "";
 static const char __pyx_k_k[] = "k";
+static const char __pyx_k_l[] = "l";
+static const char __pyx_k_r[] = "r";
+static const char __pyx_k_s[] = "s";
 static const char __pyx_k_v[] = "v";
 static const char __pyx_k_w[] = "w";
 static const char __pyx_k_NM[] = "NM";
 static const char __pyx_k__2[] = "+";
 static const char __pyx_k__3[] = "-";
 static const char __pyx_k__4[] = "?";
 static const char __pyx_k__5[] = "\t";
@@ -1295,61 +1291,69 @@
 static const char __pyx_k_cs[] = "cs";
 static const char __pyx_k_fn[] = "fn";
 static const char __pyx_k_ks[] = "ks";
 static const char __pyx_k_qe[] = "qe";
 static const char __pyx_k_qs[] = "qs";
 static const char __pyx_k_buf[] = "buf";
 static const char __pyx_k_ctg[] = "ctg";
+static const char __pyx_k_end[] = "end";
 static const char __pyx_k_map[] = "map";
 static const char __pyx_k_seq[] = "seq";
+static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_blen[] = "blen";
+static const char __pyx_k_bseq[] = "bseq";
 static const char __pyx_k_cg_Z[] = "cg:Z:";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mapq[] = "mapq";
 static const char __pyx_k_mlen[] = "mlen";
-static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_name[] = "name";
 static const char __pyx_k_qual[] = "qual";
 static const char __pyx_k_send[] = "send";
 static const char __pyx_k_seq2[] = "seq2";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ts_A[] = "ts:A:+";
 static const char __pyx_k_cigar[] = "cigar";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_mappy[] = "mappy";
 static const char __pyx_k_range[] = "range";
+static const char __pyx_k_start[] = "start";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_MIDNSH[] = "MIDNSH";
 static const char __pyx_k_best_n[] = "best_n";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_encode[] = "encode";
-static const char __pyx_k_name_2[] = "name";
+static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_preset[] = "preset";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_seg_id[] = "seg_id";
 static const char __pyx_k_strand[] = "strand";
 static const char __pyx_k_tp_A_P[] = "tp:A:P";
 static const char __pyx_k_tp_A_S[] = "tp:A:S";
 static const char __pyx_k_ts_A_2[] = "ts:A:-";
 static const char __pyx_k_ts_A_3[] = "ts:A:.";
+static const char __pyx_k_comment[] = "comment";
 static const char __pyx_k_min_cnt[] = "min_cnt";
+static const char __pyx_k_revcomp[] = "revcomp";
 static const char __pyx_k_verbose[] = "verbose";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_cigar_str[] = "cigar_str";
 static const char __pyx_k_fn_idx_in[] = "fn_idx_in";
 static const char __pyx_k_n_threads[] = "n_threads";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_fastx_read[] = "fastx_read";
 static const char __pyx_k_fn_idx_out[] = "fn_idx_out";
 static const char __pyx_k_is_primary[] = "is_primary";
 static const char __pyx_k_Aligner_map[] = "Aligner.map";
 static const char __pyx_k_min_dp_score[] = "min_dp_score";
+static const char __pyx_k_read_comment[] = "read_comment";
 static const char __pyx_k_trans_strand[] = "trans_strand";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_min_chain_score[] = "min_chain_score";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_python_mappy_pyx[] = "python/mappy.pyx";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Alignment___get___locals_lambda[] = "Alignment.__get__.<locals>.<lambda>";
@@ -1363,36 +1367,41 @@
 static PyObject *__pyx_kp_s__2;
 static PyObject *__pyx_kp_s__3;
 static PyObject *__pyx_kp_s__4;
 static PyObject *__pyx_kp_s__5;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_best_n;
 static PyObject *__pyx_n_s_blen;
+static PyObject *__pyx_n_s_bseq;
 static PyObject *__pyx_n_s_buf;
 static PyObject *__pyx_n_s_bw;
 static PyObject *__pyx_n_s_ce;
 static PyObject *__pyx_kp_s_cg_Z;
 static PyObject *__pyx_n_s_cigar;
 static PyObject *__pyx_n_s_cigar_str;
 static PyObject *__pyx_n_s_cl;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
+static PyObject *__pyx_n_s_comment;
 static PyObject *__pyx_n_s_cs;
 static PyObject *__pyx_n_s_ctg;
 static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_encode;
+static PyObject *__pyx_n_s_end;
 static PyObject *__pyx_n_s_fastx_read;
 static PyObject *__pyx_n_s_fn;
 static PyObject *__pyx_n_s_fn_idx_in;
 static PyObject *__pyx_n_s_fn_idx_out;
 static PyObject *__pyx_n_s_getstate;
+static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_is_primary;
 static PyObject *__pyx_n_s_join;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_ks;
+static PyObject *__pyx_n_s_l;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_map;
 static PyObject *__pyx_n_s_mappy;
 static PyObject *__pyx_n_s_mapq;
 static PyObject *__pyx_n_s_min_chain_score;
 static PyObject *__pyx_n_s_min_cnt;
 static PyObject *__pyx_n_s_min_dp_score;
@@ -1402,25 +1411,31 @@
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_preset;
 static PyObject *__pyx_kp_s_python_mappy_pyx;
 static PyObject *__pyx_n_s_qe;
 static PyObject *__pyx_n_s_qs;
 static PyObject *__pyx_n_s_qual;
+static PyObject *__pyx_n_s_r;
 static PyObject *__pyx_n_s_range;
+static PyObject *__pyx_n_s_read_comment;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
+static PyObject *__pyx_n_s_revcomp;
+static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_s_seg_id;
 static PyObject *__pyx_n_s_send;
 static PyObject *__pyx_n_s_seq;
 static PyObject *__pyx_n_s_seq2;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
+static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_strand;
+static PyObject *__pyx_n_s_sys;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_kp_s_tp_A_P;
 static PyObject *__pyx_kp_s_tp_A_S;
 static PyObject *__pyx_n_s_trans_strand;
 static PyObject *__pyx_kp_s_ts_A;
 static PyObject *__pyx_kp_s_ts_A_2;
@@ -1453,18 +1468,23 @@
 static void __pyx_pf_5mappy_12ThreadBuffer_2__dealloc__(struct __pyx_obj_5mappy_ThreadBuffer *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5mappy_12ThreadBuffer_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_ThreadBuffer *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5mappy_12ThreadBuffer_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_ThreadBuffer *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_5mappy_7Aligner___cinit__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self, PyObject *__pyx_v_fn_idx_in, PyObject *__pyx_v_preset, PyObject *__pyx_v_k, PyObject *__pyx_v_w, PyObject *__pyx_v_min_cnt, PyObject *__pyx_v_min_chain_score, PyObject *__pyx_v_min_dp_score, PyObject *__pyx_v_bw, PyObject *__pyx_v_best_n, PyObject *__pyx_v_n_threads, PyObject *__pyx_v_fn_idx_out); /* proto */
 static void __pyx_pf_5mappy_7Aligner_2__dealloc__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self); /* proto */
 static int __pyx_pf_5mappy_7Aligner_4__bool__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5mappy_7Aligner_6map(struct __pyx_obj_5mappy_Aligner *__pyx_v_self, PyObject *__pyx_v_seq, PyObject *__pyx_v_seq2, PyObject *__pyx_v_buf); /* proto */
-static PyObject *__pyx_pf_5mappy_7Aligner_9__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5mappy_7Aligner_11__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_5mappy_fastx_read(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fn); /* proto */
-static PyObject *__pyx_pf_5mappy_3verbose(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_v); /* proto */
+static PyObject *__pyx_pf_5mappy_7Aligner_9seq(struct __pyx_obj_5mappy_Aligner *__pyx_v_self, PyObject *__pyx_v_name, int __pyx_v_start, int __pyx_v_end); /* proto */
+static PyObject *__pyx_pf_5mappy_7Aligner_1k___get__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5mappy_7Aligner_1w___get__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5mappy_7Aligner_5n_seq___get__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5mappy_7Aligner_11__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5mappy_7Aligner_13__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_5mappy_fastx_read(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fn, PyObject *__pyx_v_read_comment); /* proto */
+static PyObject *__pyx_pf_5mappy_3revcomp(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq); /* proto */
+static PyObject *__pyx_pf_5mappy_5verbose(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_tp_new_5mappy_Alignment(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5mappy_ThreadBuffer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5mappy_Aligner(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5mappy___pyx_scope_struct__map(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5mappy___pyx_scope_struct_1_fastx_read(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_3;
 static PyObject *__pyx_int_4;
@@ -1474,18 +1494,20 @@
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_codeobj__13;
 static PyObject *__pyx_codeobj__15;
+static PyObject *__pyx_codeobj__17;
 
-/* "mappy.pyx":16
+/* "mappy.pyx":17
  * 	cdef _ctg, _cigar # these are python objects
  * 
  * 	def __cinit__(self, ctg, cl, cs, ce, strand, qs, qe, mapq, cigar, is_primary, mlen, blen, NM, trans_strand, seg_id):             # <<<<<<<<<<<<<<
  * 		self._ctg = ctg if isinstance(ctg, str) else ctg.decode()
  * 		self._ctg_len, self._r_st, self._r_en = cl, cs, ce
  */
 
@@ -1555,97 +1577,97 @@
         case  0:
         if (likely((values[0] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_ctg)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_cl)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 1); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 1); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 2); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 2); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_ce)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 3); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 3); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_strand)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 4); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 4); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_qs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 5); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 5); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_qe)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 6); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 6); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_mapq)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 7); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 7); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_cigar)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 8); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 8); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (likely((values[9] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_is_primary)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 9); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 9); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (likely((values[10] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_mlen)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 10); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 10); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 11:
         if (likely((values[11] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_blen)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 11); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 11); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 12:
         if (likely((values[12] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_NM)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 12); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 12); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 13:
         if (likely((values[13] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_trans_strand)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 13); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 13); __PYX_ERR(0, 17, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 14:
         if (likely((values[14] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_seg_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 14); __PYX_ERR(0, 16, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, 14); __PYX_ERR(0, 17, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 17, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 15) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -1676,15 +1698,15 @@
     __pyx_v_blen = values[11];
     __pyx_v_NM = values[12];
     __pyx_v_trans_strand = values[13];
     __pyx_v_seg_id = values[14];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 16, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 15, 15, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 17, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("mappy.Alignment.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5mappy_9Alignment___cinit__(((struct __pyx_obj_5mappy_Alignment *)__pyx_v_self), __pyx_v_ctg, __pyx_v_cl, __pyx_v_cs, __pyx_v_ce, __pyx_v_strand, __pyx_v_qs, __pyx_v_qe, __pyx_v_mapq, __pyx_v_cigar, __pyx_v_is_primary, __pyx_v_mlen, __pyx_v_blen, __pyx_v_NM, __pyx_v_trans_strand, __pyx_v_seg_id);
 
@@ -1704,151 +1726,151 @@
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int8_t __pyx_t_9;
   uint8_t __pyx_t_10;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "mappy.pyx":17
+  /* "mappy.pyx":18
  * 
  * 	def __cinit__(self, ctg, cl, cs, ce, strand, qs, qe, mapq, cigar, is_primary, mlen, blen, NM, trans_strand, seg_id):
  * 		self._ctg = ctg if isinstance(ctg, str) else ctg.decode()             # <<<<<<<<<<<<<<
  * 		self._ctg_len, self._r_st, self._r_en = cl, cs, ce
  * 		self._strand, self._q_st, self._q_en = strand, qs, qe
  */
   __pyx_t_2 = PyString_Check(__pyx_v_ctg); 
   if ((__pyx_t_2 != 0)) {
     __Pyx_INCREF(__pyx_v_ctg);
     __pyx_t_1 = __pyx_v_ctg;
   } else {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctg, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 17, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ctg, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 18, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     if (__pyx_t_5) {
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else {
-      __pyx_t_3 = __Pyx_PyObject_CallNoArg(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallNoArg(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
     }
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_ctg);
   __Pyx_DECREF(__pyx_v_self->_ctg);
   __pyx_v_self->_ctg = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "mappy.pyx":18
+  /* "mappy.pyx":19
  * 	def __cinit__(self, ctg, cl, cs, ce, strand, qs, qe, mapq, cigar, is_primary, mlen, blen, NM, trans_strand, seg_id):
  * 		self._ctg = ctg if isinstance(ctg, str) else ctg.decode()
  * 		self._ctg_len, self._r_st, self._r_en = cl, cs, ce             # <<<<<<<<<<<<<<
  * 		self._strand, self._q_st, self._q_en = strand, qs, qe
  * 		self._NM, self._mlen, self._blen = NM, mlen, blen
  */
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_cl); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_cs); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_ce); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_cl); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_cs); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_ce); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
   __pyx_v_self->_ctg_len = __pyx_t_6;
   __pyx_v_self->_r_st = __pyx_t_7;
   __pyx_v_self->_r_en = __pyx_t_8;
 
-  /* "mappy.pyx":19
+  /* "mappy.pyx":20
  * 		self._ctg = ctg if isinstance(ctg, str) else ctg.decode()
  * 		self._ctg_len, self._r_st, self._r_en = cl, cs, ce
  * 		self._strand, self._q_st, self._q_en = strand, qs, qe             # <<<<<<<<<<<<<<
  * 		self._NM, self._mlen, self._blen = NM, mlen, blen
  * 		self._mapq = mapq
  */
-  __pyx_t_9 = __Pyx_PyInt_As_int8_t(__pyx_v_strand); if (unlikely((__pyx_t_9 == ((int8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_qs); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_qe); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_int8_t(__pyx_v_strand); if (unlikely((__pyx_t_9 == ((int8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_qs); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_qe); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L1_error)
   __pyx_v_self->_strand = __pyx_t_9;
   __pyx_v_self->_q_st = __pyx_t_8;
   __pyx_v_self->_q_en = __pyx_t_7;
 
-  /* "mappy.pyx":20
+  /* "mappy.pyx":21
  * 		self._ctg_len, self._r_st, self._r_en = cl, cs, ce
  * 		self._strand, self._q_st, self._q_en = strand, qs, qe
  * 		self._NM, self._mlen, self._blen = NM, mlen, blen             # <<<<<<<<<<<<<<
  * 		self._mapq = mapq
  * 		self._cigar = cigar
  */
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_NM); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_mlen); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_blen); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_NM); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_mlen); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_blen); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L1_error)
   __pyx_v_self->_NM = __pyx_t_7;
   __pyx_v_self->_mlen = __pyx_t_8;
   __pyx_v_self->_blen = __pyx_t_6;
 
-  /* "mappy.pyx":21
+  /* "mappy.pyx":22
  * 		self._strand, self._q_st, self._q_en = strand, qs, qe
  * 		self._NM, self._mlen, self._blen = NM, mlen, blen
  * 		self._mapq = mapq             # <<<<<<<<<<<<<<
  * 		self._cigar = cigar
  * 		self._is_primary = is_primary
  */
-  __pyx_t_10 = __Pyx_PyInt_As_uint8_t(__pyx_v_mapq); if (unlikely((__pyx_t_10 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_uint8_t(__pyx_v_mapq); if (unlikely((__pyx_t_10 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 22, __pyx_L1_error)
   __pyx_v_self->_mapq = __pyx_t_10;
 
-  /* "mappy.pyx":22
+  /* "mappy.pyx":23
  * 		self._NM, self._mlen, self._blen = NM, mlen, blen
  * 		self._mapq = mapq
  * 		self._cigar = cigar             # <<<<<<<<<<<<<<
  * 		self._is_primary = is_primary
  * 		self._trans_strand = trans_strand
  */
   __Pyx_INCREF(__pyx_v_cigar);
   __Pyx_GIVEREF(__pyx_v_cigar);
   __Pyx_GOTREF(__pyx_v_self->_cigar);
   __Pyx_DECREF(__pyx_v_self->_cigar);
   __pyx_v_self->_cigar = __pyx_v_cigar;
 
-  /* "mappy.pyx":23
+  /* "mappy.pyx":24
  * 		self._mapq = mapq
  * 		self._cigar = cigar
  * 		self._is_primary = is_primary             # <<<<<<<<<<<<<<
  * 		self._trans_strand = trans_strand
  * 		self._seg_id = seg_id
  */
-  __pyx_t_10 = __Pyx_PyInt_As_uint8_t(__pyx_v_is_primary); if (unlikely((__pyx_t_10 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_uint8_t(__pyx_v_is_primary); if (unlikely((__pyx_t_10 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L1_error)
   __pyx_v_self->_is_primary = __pyx_t_10;
 
-  /* "mappy.pyx":24
+  /* "mappy.pyx":25
  * 		self._cigar = cigar
  * 		self._is_primary = is_primary
  * 		self._trans_strand = trans_strand             # <<<<<<<<<<<<<<
  * 		self._seg_id = seg_id
  * 
  */
-  __pyx_t_9 = __Pyx_PyInt_As_int8_t(__pyx_v_trans_strand); if (unlikely((__pyx_t_9 == ((int8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_int8_t(__pyx_v_trans_strand); if (unlikely((__pyx_t_9 == ((int8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L1_error)
   __pyx_v_self->_trans_strand = __pyx_t_9;
 
-  /* "mappy.pyx":25
+  /* "mappy.pyx":26
  * 		self._is_primary = is_primary
  * 		self._trans_strand = trans_strand
  * 		self._seg_id = seg_id             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_seg_id); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_seg_id); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L1_error)
   __pyx_v_self->_seg_id = __pyx_t_6;
 
-  /* "mappy.pyx":16
+  /* "mappy.pyx":17
  * 	cdef _ctg, _cigar # these are python objects
  * 
  * 	def __cinit__(self, ctg, cl, cs, ce, strand, qs, qe, mapq, cigar, is_primary, mlen, blen, NM, trans_strand, seg_id):             # <<<<<<<<<<<<<<
  * 		self._ctg = ctg if isinstance(ctg, str) else ctg.decode()
  * 		self._ctg_len, self._r_st, self._r_en = cl, cs, ce
  */
 
@@ -1863,15 +1885,15 @@
   __Pyx_AddTraceback("mappy.Alignment.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":28
+/* "mappy.pyx":29
  * 
  * 	@property
  * 	def ctg(self): return self._ctg             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -1900,15 +1922,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":31
+/* "mappy.pyx":32
  * 
  * 	@property
  * 	def ctg_len(self): return self._ctg_len             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -1927,15 +1949,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_7ctg_len___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_ctg_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_ctg_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1944,15 +1966,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":34
+/* "mappy.pyx":35
  * 
  * 	@property
  * 	def r_st(self): return self._r_st             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -1971,15 +1993,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_4r_st___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_r_st); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_r_st); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1988,15 +2010,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":37
+/* "mappy.pyx":38
  * 
  * 	@property
  * 	def r_en(self): return self._r_en             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2015,15 +2037,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_4r_en___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_r_en); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_r_en); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2032,15 +2054,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":40
+/* "mappy.pyx":41
  * 
  * 	@property
  * 	def strand(self): return self._strand             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2059,15 +2081,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_6strand___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int8_t(__pyx_v_self->_strand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int8_t(__pyx_v_self->_strand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2076,15 +2098,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":43
+/* "mappy.pyx":44
  * 
  * 	@property
  * 	def trans_strand(self): return self._trans_strand             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2103,15 +2125,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_12trans_strand___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int8_t(__pyx_v_self->_trans_strand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int8_t(__pyx_v_self->_trans_strand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2120,15 +2142,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":46
+/* "mappy.pyx":47
  * 
  * 	@property
  * 	def blen(self): return self._blen             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2147,15 +2169,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_4blen___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_blen); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_blen); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2164,15 +2186,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":49
+/* "mappy.pyx":50
  * 
  * 	@property
  * 	def mlen(self): return self._mlen             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2191,15 +2213,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_4mlen___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_mlen); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_mlen); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2208,15 +2230,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":52
+/* "mappy.pyx":53
  * 
  * 	@property
  * 	def NM(self): return self._NM             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2235,15 +2257,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_2NM___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_NM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_NM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2252,15 +2274,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":55
+/* "mappy.pyx":56
  * 
  * 	@property
  * 	def is_primary(self): return (self._is_primary != 0)             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2279,15 +2301,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_10is_primary___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_self->_is_primary != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_self->_is_primary != 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2296,15 +2318,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":58
+/* "mappy.pyx":59
  * 
  * 	@property
  * 	def q_st(self): return self._q_st             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2323,15 +2345,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_4q_st___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_q_st); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_q_st); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2340,15 +2362,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":61
+/* "mappy.pyx":62
  * 
  * 	@property
  * 	def q_en(self): return self._q_en             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2367,15 +2389,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_4q_en___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_q_en); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_q_en); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2384,15 +2406,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":64
+/* "mappy.pyx":65
  * 
  * 	@property
  * 	def mapq(self): return self._mapq             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2411,15 +2433,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_4mapq___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_mapq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_mapq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2428,15 +2450,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":67
+/* "mappy.pyx":68
  * 
  * 	@property
  * 	def cigar(self): return self._cigar             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2465,15 +2487,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":70
+/* "mappy.pyx":71
  * 
  * 	@property
  * 	def read_num(self): return self._seg_id + 1             # <<<<<<<<<<<<<<
  * 
  * 	@property
  */
 
@@ -2492,15 +2514,15 @@
 
 static PyObject *__pyx_pf_5mappy_9Alignment_8read_num___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_long((__pyx_v_self->_seg_id + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long((__pyx_v_self->_seg_id + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2509,15 +2531,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":73
+/* "mappy.pyx":74
  * 
  * 	@property
  * 	def cigar_str(self):             # <<<<<<<<<<<<<<
  * 		return "".join(map(lambda x: str(x[0]) + 'MIDNSH'[x[1]], self._cigar))
  * 
  */
 
@@ -2530,15 +2552,15 @@
   __pyx_r = __pyx_pf_5mappy_9Alignment_9cigar_str___get__(((struct __pyx_obj_5mappy_Alignment *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":74
+/* "mappy.pyx":75
  * 	@property
  * 	def cigar_str(self):
  * 		return "".join(map(lambda x: str(x[0]) + 'MIDNSH'[x[1]], self._cigar))             # <<<<<<<<<<<<<<
  * 
  * 	def __str__(self):
  */
 
@@ -2560,30 +2582,30 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("lambda", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_x, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_x, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_GetItem(__pyx_n_s_MIDNSH, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_3 = PyObject_GetItem(__pyx_n_s_MIDNSH, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
@@ -2596,58 +2618,58 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":73
+/* "mappy.pyx":74
  * 
  * 	@property
  * 	def cigar_str(self):             # <<<<<<<<<<<<<<
  * 		return "".join(map(lambda x: str(x[0]) + 'MIDNSH'[x[1]], self._cigar))
  * 
  */
 
 static PyObject *__pyx_pf_5mappy_9Alignment_9cigar_str___get__(struct __pyx_obj_5mappy_Alignment *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "mappy.pyx":74
+  /* "mappy.pyx":75
  * 	@property
  * 	def cigar_str(self):
  * 		return "".join(map(lambda x: str(x[0]) + 'MIDNSH'[x[1]], self._cigar))             # <<<<<<<<<<<<<<
  * 
  * 	def __str__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_5mappy_9Alignment_9cigar_str_7__get___lambda, 0, __pyx_n_s_Alignment___get___locals_lambda, NULL, __pyx_n_s_mappy, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_5mappy_9Alignment_9cigar_str_7__get___lambda, 0, __pyx_n_s_Alignment___get___locals_lambda, NULL, __pyx_n_s_mappy, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_v_self->_cigar);
   __Pyx_GIVEREF(__pyx_v_self->_cigar);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_self->_cigar);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s_, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Join(__pyx_kp_s_, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "mappy.pyx":73
+  /* "mappy.pyx":74
  * 
  * 	@property
  * 	def cigar_str(self):             # <<<<<<<<<<<<<<
  * 		return "".join(map(lambda x: str(x[0]) + 'MIDNSH'[x[1]], self._cigar))
  * 
  */
 
@@ -2659,15 +2681,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":76
+/* "mappy.pyx":77
  * 		return "".join(map(lambda x: str(x[0]) + 'MIDNSH'[x[1]], self._cigar))
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		if self._strand > 0: strand = '+'
  * 		elif self._strand < 0: strand = '-'
  */
 
@@ -2699,233 +2721,233 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "mappy.pyx":77
+  /* "mappy.pyx":78
  * 
  * 	def __str__(self):
  * 		if self._strand > 0: strand = '+'             # <<<<<<<<<<<<<<
  * 		elif self._strand < 0: strand = '-'
  * 		else: strand = '?'
  */
   __pyx_t_1 = ((__pyx_v_self->_strand > 0) != 0);
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_kp_s__2);
     __pyx_v_strand = __pyx_kp_s__2;
     goto __pyx_L3;
   }
 
-  /* "mappy.pyx":78
+  /* "mappy.pyx":79
  * 	def __str__(self):
  * 		if self._strand > 0: strand = '+'
  * 		elif self._strand < 0: strand = '-'             # <<<<<<<<<<<<<<
  * 		else: strand = '?'
  * 		if self._is_primary != 0: tp = 'tp:A:P'
  */
   __pyx_t_1 = ((__pyx_v_self->_strand < 0) != 0);
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_kp_s__3);
     __pyx_v_strand = __pyx_kp_s__3;
     goto __pyx_L3;
   }
 
-  /* "mappy.pyx":79
+  /* "mappy.pyx":80
  * 		if self._strand > 0: strand = '+'
  * 		elif self._strand < 0: strand = '-'
  * 		else: strand = '?'             # <<<<<<<<<<<<<<
  * 		if self._is_primary != 0: tp = 'tp:A:P'
  * 		else: tp = 'tp:A:S'
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_kp_s__4);
     __pyx_v_strand = __pyx_kp_s__4;
   }
   __pyx_L3:;
 
-  /* "mappy.pyx":80
+  /* "mappy.pyx":81
  * 		elif self._strand < 0: strand = '-'
  * 		else: strand = '?'
  * 		if self._is_primary != 0: tp = 'tp:A:P'             # <<<<<<<<<<<<<<
  * 		else: tp = 'tp:A:S'
  * 		if self._trans_strand > 0: ts = 'ts:A:+'
  */
   __pyx_t_1 = ((__pyx_v_self->_is_primary != 0) != 0);
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_kp_s_tp_A_P);
     __pyx_v_tp = __pyx_kp_s_tp_A_P;
     goto __pyx_L4;
   }
 
-  /* "mappy.pyx":81
+  /* "mappy.pyx":82
  * 		else: strand = '?'
  * 		if self._is_primary != 0: tp = 'tp:A:P'
  * 		else: tp = 'tp:A:S'             # <<<<<<<<<<<<<<
  * 		if self._trans_strand > 0: ts = 'ts:A:+'
  * 		elif self._trans_strand < 0: ts = 'ts:A:-'
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_kp_s_tp_A_S);
     __pyx_v_tp = __pyx_kp_s_tp_A_S;
   }
   __pyx_L4:;
 
-  /* "mappy.pyx":82
+  /* "mappy.pyx":83
  * 		if self._is_primary != 0: tp = 'tp:A:P'
  * 		else: tp = 'tp:A:S'
  * 		if self._trans_strand > 0: ts = 'ts:A:+'             # <<<<<<<<<<<<<<
  * 		elif self._trans_strand < 0: ts = 'ts:A:-'
  * 		else: ts = 'ts:A:.'
  */
   __pyx_t_1 = ((__pyx_v_self->_trans_strand > 0) != 0);
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_kp_s_ts_A);
     __pyx_v_ts = __pyx_kp_s_ts_A;
     goto __pyx_L5;
   }
 
-  /* "mappy.pyx":83
+  /* "mappy.pyx":84
  * 		else: tp = 'tp:A:S'
  * 		if self._trans_strand > 0: ts = 'ts:A:+'
  * 		elif self._trans_strand < 0: ts = 'ts:A:-'             # <<<<<<<<<<<<<<
  * 		else: ts = 'ts:A:.'
  * 		return "\t".join([str(self._q_st), str(self._q_en), strand, self._ctg, str(self._ctg_len), str(self._r_st), str(self._r_en),
  */
   __pyx_t_1 = ((__pyx_v_self->_trans_strand < 0) != 0);
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_kp_s_ts_A_2);
     __pyx_v_ts = __pyx_kp_s_ts_A_2;
     goto __pyx_L5;
   }
 
-  /* "mappy.pyx":84
+  /* "mappy.pyx":85
  * 		if self._trans_strand > 0: ts = 'ts:A:+'
  * 		elif self._trans_strand < 0: ts = 'ts:A:-'
  * 		else: ts = 'ts:A:.'             # <<<<<<<<<<<<<<
  * 		return "\t".join([str(self._q_st), str(self._q_en), strand, self._ctg, str(self._ctg_len), str(self._r_st), str(self._r_en),
  * 				str(self._mlen), str(self._blen), str(self._mapq), tp, ts, "cg:Z:" + self.cigar_str])
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_kp_s_ts_A_3);
     __pyx_v_ts = __pyx_kp_s_ts_A_3;
   }
   __pyx_L5:;
 
-  /* "mappy.pyx":85
+  /* "mappy.pyx":86
  * 		elif self._trans_strand < 0: ts = 'ts:A:-'
  * 		else: ts = 'ts:A:.'
  * 		return "\t".join([str(self._q_st), str(self._q_en), strand, self._ctg, str(self._ctg_len), str(self._r_st), str(self._r_en),             # <<<<<<<<<<<<<<
  * 				str(self._mlen), str(self._blen), str(self._mapq), tp, ts, "cg:Z:" + self.cigar_str])
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->_q_st); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->_q_st); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_q_en); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_q_en); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->_ctg_len); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->_ctg_len); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->_r_st); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->_r_st); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_self->_r_en); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_self->_r_en); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "mappy.pyx":86
+  /* "mappy.pyx":87
  * 		else: ts = 'ts:A:.'
  * 		return "\t".join([str(self._q_st), str(self._q_en), strand, self._ctg, str(self._ctg_len), str(self._r_st), str(self._r_en),
  * 				str(self._mlen), str(self._blen), str(self._mapq), tp, ts, "cg:Z:" + self.cigar_str])             # <<<<<<<<<<<<<<
  * 
  * cdef class ThreadBuffer:
  */
-  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_self->_mlen); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_self->_mlen); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->_blen); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->_blen); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_mapq); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_mapq); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_9);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9);
   __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cigar_str); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cigar_str); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = PyNumber_Add(__pyx_kp_s_cg_Z, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_11 = PyNumber_Add(__pyx_kp_s_cg_Z, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "mappy.pyx":85
+  /* "mappy.pyx":86
  * 		elif self._trans_strand < 0: ts = 'ts:A:-'
  * 		else: ts = 'ts:A:.'
  * 		return "\t".join([str(self._q_st), str(self._q_en), strand, self._ctg, str(self._ctg_len), str(self._r_st), str(self._r_en),             # <<<<<<<<<<<<<<
  * 				str(self._mlen), str(self._blen), str(self._mapq), tp, ts, "cg:Z:" + self.cigar_str])
  * 
  */
-  __pyx_t_10 = PyList_New(13); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_10 = PyList_New(13); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_2);
   PyList_SET_ITEM(__pyx_t_10, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_10, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_v_strand);
   __Pyx_GIVEREF(__pyx_v_strand);
@@ -2958,22 +2980,22 @@
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
   __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyString_Join(__pyx_kp_s__5, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyString_Join(__pyx_kp_s__5, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_r = __pyx_t_11;
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "mappy.pyx":76
+  /* "mappy.pyx":77
  * 		return "".join(map(lambda x: str(x[0]) + 'MIDNSH'[x[1]], self._cigar))
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		if self._strand > 0: strand = '+'
  * 		elif self._strand < 0: strand = '-'
  */
 
@@ -3103,15 +3125,15 @@
   __Pyx_AddTraceback("mappy.Alignment.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":91
+/* "mappy.pyx":92
  * 	cdef cmappy.mm_tbuf_t *_b
  * 
  * 	def __cinit__(self):             # <<<<<<<<<<<<<<
  * 		self._b = cmappy.mm_tbuf_init()
  * 
  */
 
@@ -3132,38 +3154,38 @@
 }
 
 static int __pyx_pf_5mappy_12ThreadBuffer___cinit__(struct __pyx_obj_5mappy_ThreadBuffer *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "mappy.pyx":92
+  /* "mappy.pyx":93
  * 
  * 	def __cinit__(self):
  * 		self._b = cmappy.mm_tbuf_init()             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
   __pyx_v_self->_b = mm_tbuf_init();
 
-  /* "mappy.pyx":91
+  /* "mappy.pyx":92
  * 	cdef cmappy.mm_tbuf_t *_b
  * 
  * 	def __cinit__(self):             # <<<<<<<<<<<<<<
  * 		self._b = cmappy.mm_tbuf_init()
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":94
+/* "mappy.pyx":95
  * 		self._b = cmappy.mm_tbuf_init()
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		cmappy.mm_tbuf_destroy(self._b)
  * 
  */
 
@@ -3178,24 +3200,24 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_5mappy_12ThreadBuffer_2__dealloc__(struct __pyx_obj_5mappy_ThreadBuffer *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "mappy.pyx":95
+  /* "mappy.pyx":96
  * 
  * 	def __dealloc__(self):
  * 		cmappy.mm_tbuf_destroy(self._b)             # <<<<<<<<<<<<<<
  * 
  * cdef class Aligner:
  */
   mm_tbuf_destroy(__pyx_v_self->_b);
 
-  /* "mappy.pyx":94
+  /* "mappy.pyx":95
  * 		self._b = cmappy.mm_tbuf_init()
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		cmappy.mm_tbuf_destroy(self._b)
  * 
  */
 
@@ -3306,15 +3328,15 @@
   __Pyx_AddTraceback("mappy.ThreadBuffer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":102
+/* "mappy.pyx":103
  * 	cdef cmappy.mm_mapopt_t map_opt
  * 
  * 	def __cinit__(self, fn_idx_in, preset=None, k=None, w=None, min_cnt=None, min_chain_score=None, min_dp_score=None, bw=None, best_n=None, n_threads=3, fn_idx_out=None):             # <<<<<<<<<<<<<<
  * 		cmappy.mm_set_opt(NULL, &self.idx_opt, &self.map_opt) # set the default options
  * 		if preset is not None:
  */
 
@@ -3440,15 +3462,15 @@
         case 10:
         if (kw_args > 0) {
           PyObject* value = PyDict_GetItem(__pyx_kwds, __pyx_n_s_fn_idx_out);
           if (value) { values[10] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 102, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 103, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
         CYTHON_FALLTHROUGH;
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
@@ -3483,15 +3505,15 @@
     __pyx_v_bw = values[7];
     __pyx_v_best_n = values[8];
     __pyx_v_n_threads = values[9];
     __pyx_v_fn_idx_out = values[10];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 11, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 102, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 11, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 103, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("mappy.Aligner.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5mappy_7Aligner___cinit__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self), __pyx_v_fn_idx_in, __pyx_v_preset, __pyx_v_k, __pyx_v_w, __pyx_v_min_cnt, __pyx_v_min_chain_score, __pyx_v_min_dp_score, __pyx_v_bw, __pyx_v_best_n, __pyx_v_n_threads, __pyx_v_fn_idx_out);
 
@@ -3513,399 +3535,409 @@
   char *__pyx_t_7;
   short __pyx_t_8;
   int __pyx_t_9;
   char const *__pyx_t_10;
   char const *__pyx_t_11;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "mappy.pyx":103
+  /* "mappy.pyx":104
  * 
  * 	def __cinit__(self, fn_idx_in, preset=None, k=None, w=None, min_cnt=None, min_chain_score=None, min_dp_score=None, bw=None, best_n=None, n_threads=3, fn_idx_out=None):
  * 		cmappy.mm_set_opt(NULL, &self.idx_opt, &self.map_opt) # set the default options             # <<<<<<<<<<<<<<
  * 		if preset is not None:
  * 			cmappy.mm_set_opt(str.encode(preset), &self.idx_opt, &self.map_opt) # apply preset
  */
   mm_set_opt(NULL, (&__pyx_v_self->idx_opt), (&__pyx_v_self->map_opt));
 
-  /* "mappy.pyx":104
+  /* "mappy.pyx":105
  * 	def __cinit__(self, fn_idx_in, preset=None, k=None, w=None, min_cnt=None, min_chain_score=None, min_dp_score=None, bw=None, best_n=None, n_threads=3, fn_idx_out=None):
  * 		cmappy.mm_set_opt(NULL, &self.idx_opt, &self.map_opt) # set the default options
  * 		if preset is not None:             # <<<<<<<<<<<<<<
  * 			cmappy.mm_set_opt(str.encode(preset), &self.idx_opt, &self.map_opt) # apply preset
  * 		self.map_opt.flag |= 4 # always perform alignment
  */
   __pyx_t_1 = (__pyx_v_preset != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "mappy.pyx":105
+    /* "mappy.pyx":106
  * 		cmappy.mm_set_opt(NULL, &self.idx_opt, &self.map_opt) # set the default options
  * 		if preset is not None:
  * 			cmappy.mm_set_opt(str.encode(preset), &self.idx_opt, &self.map_opt) # apply preset             # <<<<<<<<<<<<<<
  * 		self.map_opt.flag |= 4 # always perform alignment
  * 		self.idx_opt.batch_size = 0x7fffffffffffffffL # always build a uni-part index
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     if (!__pyx_t_5) {
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_preset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_preset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
     } else {
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[2] = {__pyx_t_5, __pyx_v_preset};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[2] = {__pyx_t_5, __pyx_v_preset};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       {
-        __pyx_t_6 = PyTuple_New(1+1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_6 = PyTuple_New(1+1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 106, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
         __Pyx_INCREF(__pyx_v_preset);
         __Pyx_GIVEREF(__pyx_v_preset);
         PyTuple_SET_ITEM(__pyx_t_6, 0+1, __pyx_v_preset);
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L1_error)
     mm_set_opt(__pyx_t_7, (&__pyx_v_self->idx_opt), (&__pyx_v_self->map_opt));
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "mappy.pyx":104
+    /* "mappy.pyx":105
  * 	def __cinit__(self, fn_idx_in, preset=None, k=None, w=None, min_cnt=None, min_chain_score=None, min_dp_score=None, bw=None, best_n=None, n_threads=3, fn_idx_out=None):
  * 		cmappy.mm_set_opt(NULL, &self.idx_opt, &self.map_opt) # set the default options
  * 		if preset is not None:             # <<<<<<<<<<<<<<
  * 			cmappy.mm_set_opt(str.encode(preset), &self.idx_opt, &self.map_opt) # apply preset
  * 		self.map_opt.flag |= 4 # always perform alignment
  */
   }
 
-  /* "mappy.pyx":106
+  /* "mappy.pyx":107
  * 		if preset is not None:
  * 			cmappy.mm_set_opt(str.encode(preset), &self.idx_opt, &self.map_opt) # apply preset
  * 		self.map_opt.flag |= 4 # always perform alignment             # <<<<<<<<<<<<<<
  * 		self.idx_opt.batch_size = 0x7fffffffffffffffL # always build a uni-part index
  * 		if k is not None: self.idx_opt.k = k
  */
   __pyx_v_self->map_opt.flag = (__pyx_v_self->map_opt.flag | 4);
 
-  /* "mappy.pyx":107
+  /* "mappy.pyx":108
  * 			cmappy.mm_set_opt(str.encode(preset), &self.idx_opt, &self.map_opt) # apply preset
  * 		self.map_opt.flag |= 4 # always perform alignment
  * 		self.idx_opt.batch_size = 0x7fffffffffffffffL # always build a uni-part index             # <<<<<<<<<<<<<<
  * 		if k is not None: self.idx_opt.k = k
  * 		if w is not None: self.idx_opt.w = w
  */
   __pyx_v_self->idx_opt.batch_size = 0x7fffffffffffffffL;
 
-  /* "mappy.pyx":108
+  /* "mappy.pyx":109
  * 		self.map_opt.flag |= 4 # always perform alignment
  * 		self.idx_opt.batch_size = 0x7fffffffffffffffL # always build a uni-part index
  * 		if k is not None: self.idx_opt.k = k             # <<<<<<<<<<<<<<
  * 		if w is not None: self.idx_opt.w = w
  * 		if min_cnt is not None: self.map_opt.min_cnt = min_cnt
  */
   __pyx_t_2 = (__pyx_v_k != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
-    __pyx_t_8 = __Pyx_PyInt_As_short(__pyx_v_k); if (unlikely((__pyx_t_8 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_short(__pyx_v_k); if (unlikely((__pyx_t_8 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
     __pyx_v_self->idx_opt.k = __pyx_t_8;
   }
 
-  /* "mappy.pyx":109
+  /* "mappy.pyx":110
  * 		self.idx_opt.batch_size = 0x7fffffffffffffffL # always build a uni-part index
  * 		if k is not None: self.idx_opt.k = k
  * 		if w is not None: self.idx_opt.w = w             # <<<<<<<<<<<<<<
  * 		if min_cnt is not None: self.map_opt.min_cnt = min_cnt
  * 		if min_chain_score is not None: self.map_opt.min_chain_score = min_chain_score
  */
   __pyx_t_1 = (__pyx_v_w != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
-    __pyx_t_8 = __Pyx_PyInt_As_short(__pyx_v_w); if (unlikely((__pyx_t_8 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_short(__pyx_v_w); if (unlikely((__pyx_t_8 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L1_error)
     __pyx_v_self->idx_opt.w = __pyx_t_8;
   }
 
-  /* "mappy.pyx":110
+  /* "mappy.pyx":111
  * 		if k is not None: self.idx_opt.k = k
  * 		if w is not None: self.idx_opt.w = w
  * 		if min_cnt is not None: self.map_opt.min_cnt = min_cnt             # <<<<<<<<<<<<<<
  * 		if min_chain_score is not None: self.map_opt.min_chain_score = min_chain_score
  * 		if min_dp_score is not None: self.map_opt.min_dp_max = min_dp_score
  */
   __pyx_t_2 = (__pyx_v_min_cnt != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
-    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_min_cnt); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_min_cnt); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
     __pyx_v_self->map_opt.min_cnt = __pyx_t_9;
   }
 
-  /* "mappy.pyx":111
+  /* "mappy.pyx":112
  * 		if w is not None: self.idx_opt.w = w
  * 		if min_cnt is not None: self.map_opt.min_cnt = min_cnt
  * 		if min_chain_score is not None: self.map_opt.min_chain_score = min_chain_score             # <<<<<<<<<<<<<<
  * 		if min_dp_score is not None: self.map_opt.min_dp_max = min_dp_score
  * 		if bw is not None: self.map_opt.bw = bw
  */
   __pyx_t_1 = (__pyx_v_min_chain_score != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
-    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_min_chain_score); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_min_chain_score); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L1_error)
     __pyx_v_self->map_opt.min_chain_score = __pyx_t_9;
   }
 
-  /* "mappy.pyx":112
+  /* "mappy.pyx":113
  * 		if min_cnt is not None: self.map_opt.min_cnt = min_cnt
  * 		if min_chain_score is not None: self.map_opt.min_chain_score = min_chain_score
  * 		if min_dp_score is not None: self.map_opt.min_dp_max = min_dp_score             # <<<<<<<<<<<<<<
  * 		if bw is not None: self.map_opt.bw = bw
- * 		if best_n is not None: self.best_n = best_n
+ * 		if best_n is not None: self.map_opt.best_n = best_n
  */
   __pyx_t_2 = (__pyx_v_min_dp_score != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
-    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_min_dp_score); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_min_dp_score); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L1_error)
     __pyx_v_self->map_opt.min_dp_max = __pyx_t_9;
   }
 
-  /* "mappy.pyx":113
+  /* "mappy.pyx":114
  * 		if min_chain_score is not None: self.map_opt.min_chain_score = min_chain_score
  * 		if min_dp_score is not None: self.map_opt.min_dp_max = min_dp_score
  * 		if bw is not None: self.map_opt.bw = bw             # <<<<<<<<<<<<<<
- * 		if best_n is not None: self.best_n = best_n
+ * 		if best_n is not None: self.map_opt.best_n = best_n
  * 
  */
   __pyx_t_1 = (__pyx_v_bw != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
-    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_bw); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_bw); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L1_error)
     __pyx_v_self->map_opt.bw = __pyx_t_9;
   }
 
-  /* "mappy.pyx":114
+  /* "mappy.pyx":115
  * 		if min_dp_score is not None: self.map_opt.min_dp_max = min_dp_score
  * 		if bw is not None: self.map_opt.bw = bw
- * 		if best_n is not None: self.best_n = best_n             # <<<<<<<<<<<<<<
+ * 		if best_n is not None: self.map_opt.best_n = best_n             # <<<<<<<<<<<<<<
  * 
  * 		cdef cmappy.mm_idx_reader_t *r;
  */
   __pyx_t_2 = (__pyx_v_best_n != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
-    if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_best_n, __pyx_v_best_n) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_best_n); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L1_error)
+    __pyx_v_self->map_opt.best_n = __pyx_t_9;
   }
 
-  /* "mappy.pyx":117
+  /* "mappy.pyx":118
  * 
  * 		cdef cmappy.mm_idx_reader_t *r;
  * 		if fn_idx_out is None:             # <<<<<<<<<<<<<<
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, NULL)
  * 		else:
  */
   __pyx_t_1 = (__pyx_v_fn_idx_out == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "mappy.pyx":118
+    /* "mappy.pyx":119
  * 		cdef cmappy.mm_idx_reader_t *r;
  * 		if fn_idx_out is None:
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, NULL)             # <<<<<<<<<<<<<<
  * 		else:
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, fn_idx_out)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     if (!__pyx_t_6) {
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_fn_idx_in); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_fn_idx_in); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
     } else {
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[2] = {__pyx_t_6, __pyx_v_fn_idx_in};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[2] = {__pyx_t_6, __pyx_v_fn_idx_in};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       {
-        __pyx_t_5 = PyTuple_New(1+1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_New(1+1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6); __pyx_t_6 = NULL;
         __Pyx_INCREF(__pyx_v_fn_idx_in);
         __Pyx_GIVEREF(__pyx_v_fn_idx_in);
         PyTuple_SET_ITEM(__pyx_t_5, 0+1, __pyx_v_fn_idx_in);
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_10 = __Pyx_PyObject_AsString(__pyx_t_3); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 118, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_AsString(__pyx_t_3); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L1_error)
     __pyx_v_r = mm_idx_reader_open(__pyx_t_10, (&__pyx_v_self->idx_opt), NULL);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "mappy.pyx":117
+    /* "mappy.pyx":118
  * 
  * 		cdef cmappy.mm_idx_reader_t *r;
  * 		if fn_idx_out is None:             # <<<<<<<<<<<<<<
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, NULL)
  * 		else:
  */
     goto __pyx_L11;
   }
 
-  /* "mappy.pyx":120
+  /* "mappy.pyx":121
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, NULL)
  * 		else:
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, fn_idx_out)             # <<<<<<<<<<<<<<
  * 		if r is not NULL:
  * 			self._idx = cmappy.mm_idx_reader_read(r, n_threads) # NB: ONLY read the first part
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     if (!__pyx_t_5) {
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_fn_idx_in); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_fn_idx_in); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
     } else {
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[2] = {__pyx_t_5, __pyx_v_fn_idx_in};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[2] = {__pyx_t_5, __pyx_v_fn_idx_in};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_3);
       } else
       #endif
       {
-        __pyx_t_6 = PyTuple_New(1+1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 120, __pyx_L1_error)
+        __pyx_t_6 = PyTuple_New(1+1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 121, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
         __Pyx_INCREF(__pyx_v_fn_idx_in);
         __Pyx_GIVEREF(__pyx_v_fn_idx_in);
         PyTuple_SET_ITEM(__pyx_t_6, 0+1, __pyx_v_fn_idx_in);
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_10 = __Pyx_PyObject_AsString(__pyx_t_3); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_v_fn_idx_out); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_AsString(__pyx_t_3); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_AsString(__pyx_v_fn_idx_out); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 121, __pyx_L1_error)
     __pyx_v_r = mm_idx_reader_open(__pyx_t_10, (&__pyx_v_self->idx_opt), __pyx_t_11);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L11:;
 
-  /* "mappy.pyx":121
+  /* "mappy.pyx":122
  * 		else:
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, fn_idx_out)
  * 		if r is not NULL:             # <<<<<<<<<<<<<<
  * 			self._idx = cmappy.mm_idx_reader_read(r, n_threads) # NB: ONLY read the first part
  * 			cmappy.mm_idx_reader_close(r)
  */
   __pyx_t_2 = ((__pyx_v_r != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "mappy.pyx":122
+    /* "mappy.pyx":123
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, fn_idx_out)
  * 		if r is not NULL:
  * 			self._idx = cmappy.mm_idx_reader_read(r, n_threads) # NB: ONLY read the first part             # <<<<<<<<<<<<<<
  * 			cmappy.mm_idx_reader_close(r)
  * 			cmappy.mm_mapopt_update(&self.map_opt, self._idx)
  */
-    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_n_threads); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_n_threads); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 123, __pyx_L1_error)
     __pyx_v_self->_idx = mm_idx_reader_read(__pyx_v_r, __pyx_t_9);
 
-    /* "mappy.pyx":123
+    /* "mappy.pyx":124
  * 		if r is not NULL:
  * 			self._idx = cmappy.mm_idx_reader_read(r, n_threads) # NB: ONLY read the first part
  * 			cmappy.mm_idx_reader_close(r)             # <<<<<<<<<<<<<<
  * 			cmappy.mm_mapopt_update(&self.map_opt, self._idx)
- * 
+ * 			cmappy.mm_idx_index_name(self._idx)
  */
     mm_idx_reader_close(__pyx_v_r);
 
-    /* "mappy.pyx":124
+    /* "mappy.pyx":125
  * 			self._idx = cmappy.mm_idx_reader_read(r, n_threads) # NB: ONLY read the first part
  * 			cmappy.mm_idx_reader_close(r)
  * 			cmappy.mm_mapopt_update(&self.map_opt, self._idx)             # <<<<<<<<<<<<<<
+ * 			cmappy.mm_idx_index_name(self._idx)
  * 
- * 	def __dealloc__(self):
  */
     mm_mapopt_update((&__pyx_v_self->map_opt), __pyx_v_self->_idx);
 
-    /* "mappy.pyx":121
+    /* "mappy.pyx":126
+ * 			cmappy.mm_idx_reader_close(r)
+ * 			cmappy.mm_mapopt_update(&self.map_opt, self._idx)
+ * 			cmappy.mm_idx_index_name(self._idx)             # <<<<<<<<<<<<<<
+ * 
+ * 	def __dealloc__(self):
+ */
+    mm_idx_index_name(__pyx_v_self->_idx);
+
+    /* "mappy.pyx":122
  * 		else:
  * 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, fn_idx_out)
  * 		if r is not NULL:             # <<<<<<<<<<<<<<
  * 			self._idx = cmappy.mm_idx_reader_read(r, n_threads) # NB: ONLY read the first part
  * 			cmappy.mm_idx_reader_close(r)
  */
   }
 
-  /* "mappy.pyx":102
+  /* "mappy.pyx":103
  * 	cdef cmappy.mm_mapopt_t map_opt
  * 
  * 	def __cinit__(self, fn_idx_in, preset=None, k=None, w=None, min_cnt=None, min_chain_score=None, min_dp_score=None, bw=None, best_n=None, n_threads=3, fn_idx_out=None):             # <<<<<<<<<<<<<<
  * 		cmappy.mm_set_opt(NULL, &self.idx_opt, &self.map_opt) # set the default options
  * 		if preset is not None:
  */
 
@@ -3920,16 +3952,16 @@
   __Pyx_AddTraceback("mappy.Aligner.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":126
- * 			cmappy.mm_mapopt_update(&self.map_opt, self._idx)
+/* "mappy.pyx":128
+ * 			cmappy.mm_idx_index_name(self._idx)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		if self._idx is not NULL:
  * 			cmappy.mm_idx_destroy(self._idx)
  */
 
 /* Python wrapper */
@@ -3944,55 +3976,55 @@
 }
 
 static void __pyx_pf_5mappy_7Aligner_2__dealloc__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "mappy.pyx":127
+  /* "mappy.pyx":129
  * 
  * 	def __dealloc__(self):
  * 		if self._idx is not NULL:             # <<<<<<<<<<<<<<
  * 			cmappy.mm_idx_destroy(self._idx)
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->_idx != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "mappy.pyx":128
+    /* "mappy.pyx":130
  * 	def __dealloc__(self):
  * 		if self._idx is not NULL:
  * 			cmappy.mm_idx_destroy(self._idx)             # <<<<<<<<<<<<<<
  * 
  * 	def __bool__(self):
  */
     mm_idx_destroy(__pyx_v_self->_idx);
 
-    /* "mappy.pyx":127
+    /* "mappy.pyx":129
  * 
  * 	def __dealloc__(self):
  * 		if self._idx is not NULL:             # <<<<<<<<<<<<<<
  * 			cmappy.mm_idx_destroy(self._idx)
  * 
  */
   }
 
-  /* "mappy.pyx":126
- * 			cmappy.mm_mapopt_update(&self.map_opt, self._idx)
+  /* "mappy.pyx":128
+ * 			cmappy.mm_idx_index_name(self._idx)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		if self._idx is not NULL:
  * 			cmappy.mm_idx_destroy(self._idx)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "mappy.pyx":130
+/* "mappy.pyx":132
  * 			cmappy.mm_idx_destroy(self._idx)
  * 
  * 	def __bool__(self):             # <<<<<<<<<<<<<<
  * 		return (self._idx != NULL)
  * 
  */
 
@@ -4010,40 +4042,40 @@
 }
 
 static int __pyx_pf_5mappy_7Aligner_4__bool__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__bool__", 0);
 
-  /* "mappy.pyx":131
+  /* "mappy.pyx":133
  * 
  * 	def __bool__(self):
  * 		return (self._idx != NULL)             # <<<<<<<<<<<<<<
  * 
  * 	def map(self, seq, seq2=None, buf=None):
  */
   __pyx_r = (__pyx_v_self->_idx != NULL);
   goto __pyx_L0;
 
-  /* "mappy.pyx":130
+  /* "mappy.pyx":132
  * 			cmappy.mm_idx_destroy(self._idx)
  * 
  * 	def __bool__(self):             # <<<<<<<<<<<<<<
  * 		return (self._idx != NULL)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_5mappy_7Aligner_8generator(__pyx_CoroutineObject *__pyx_generator, PyObject *__pyx_sent_value); /* proto */
 
-/* "mappy.pyx":133
+/* "mappy.pyx":135
  * 		return (self._idx != NULL)
  * 
  * 	def map(self, seq, seq2=None, buf=None):             # <<<<<<<<<<<<<<
  * 		cdef cmappy.mm_reg1_t *regs
  * 		cdef cmappy.mm_hitpy_t h
  */
 
@@ -4089,15 +4121,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = PyDict_GetItem(__pyx_kwds, __pyx_n_s_buf);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "map") < 0)) __PYX_ERR(0, 133, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "map") < 0)) __PYX_ERR(0, 135, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -4108,15 +4140,15 @@
     }
     __pyx_v_seq = values[0];
     __pyx_v_seq2 = values[1];
     __pyx_v_buf = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("map", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 133, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("map", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 135, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("mappy.Aligner.map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5mappy_7Aligner_6map(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self), __pyx_v_seq, __pyx_v_seq2, __pyx_v_buf);
 
@@ -4130,15 +4162,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("map", 0);
   __pyx_cur_scope = (struct __pyx_obj_5mappy___pyx_scope_struct__map *)__pyx_tp_new_5mappy___pyx_scope_struct__map(__pyx_ptype_5mappy___pyx_scope_struct__map, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_5mappy___pyx_scope_struct__map *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 133, __pyx_L1_error)
+    __PYX_ERR(0, 135, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_seq = __pyx_v_seq;
@@ -4147,15 +4179,15 @@
   __pyx_cur_scope->__pyx_v_seq2 = __pyx_v_seq2;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq2);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_seq2);
   __pyx_cur_scope->__pyx_v_buf = __pyx_v_buf;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_buf);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_buf);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_5mappy_7Aligner_8generator, (PyObject *) __pyx_cur_scope, __pyx_n_s_map, __pyx_n_s_Aligner_map, __pyx_n_s_mappy); if (unlikely(!gen)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_5mappy_7Aligner_8generator, (PyObject *) __pyx_cur_scope, __pyx_n_s_map, __pyx_n_s_Aligner_map, __pyx_n_s_mappy); if (unlikely(!gen)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4174,21 +4206,21 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   char const *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  char const *__pyx_t_9;
+  char const *__pyx_t_8;
+  int __pyx_t_9;
   int __pyx_t_10;
-  int __pyx_t_11;
+  int32_t __pyx_t_11;
   int32_t __pyx_t_12;
-  int32_t __pyx_t_13;
-  int __pyx_t_14;
+  int __pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   PyObject *__pyx_t_21 = NULL;
@@ -4201,361 +4233,317 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L11_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 135, __pyx_L1_error)
 
-  /* "mappy.pyx":139
+  /* "mappy.pyx":141
  * 		cdef int n_regs
  * 
  * 		if self._idx is NULL: return None             # <<<<<<<<<<<<<<
  * 		if buf is None: b = ThreadBuffer()
  * 		else: b = buf
  */
   __pyx_t_1 = ((__pyx_cur_scope->__pyx_v_self->_idx == NULL) != 0);
   if (__pyx_t_1) {
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = NULL; __Pyx_ReturnWithStopIteration(Py_None);
     goto __pyx_L0;
   }
 
-  /* "mappy.pyx":140
+  /* "mappy.pyx":142
  * 
  * 		if self._idx is NULL: return None
  * 		if buf is None: b = ThreadBuffer()             # <<<<<<<<<<<<<<
  * 		else: b = buf
- * 		if seq2 is None: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), NULL, &n_regs, b._b, &self.map_opt)
+ * 
  */
   __pyx_t_1 = (__pyx_cur_scope->__pyx_v_buf == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5mappy_ThreadBuffer), __pyx_empty_tuple, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5mappy_ThreadBuffer), __pyx_empty_tuple, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __pyx_cur_scope->__pyx_v_b = ((struct __pyx_obj_5mappy_ThreadBuffer *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L5;
   }
 
-  /* "mappy.pyx":141
+  /* "mappy.pyx":143
  * 		if self._idx is NULL: return None
  * 		if buf is None: b = ThreadBuffer()
  * 		else: b = buf             # <<<<<<<<<<<<<<
- * 		if seq2 is None: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), NULL, &n_regs, b._b, &self.map_opt)
- * 		else: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), str.encode(seq2), &n_regs, b._b, &self.map_opt)
+ * 
+ * 		_seq = seq if isinstance(seq, bytes) else seq.encode()
  */
   /*else*/ {
-    if (!(likely(((__pyx_cur_scope->__pyx_v_buf) == Py_None) || likely(__Pyx_TypeTest(__pyx_cur_scope->__pyx_v_buf, __pyx_ptype_5mappy_ThreadBuffer))))) __PYX_ERR(0, 141, __pyx_L1_error)
+    if (!(likely(((__pyx_cur_scope->__pyx_v_buf) == Py_None) || likely(__Pyx_TypeTest(__pyx_cur_scope->__pyx_v_buf, __pyx_ptype_5mappy_ThreadBuffer))))) __PYX_ERR(0, 143, __pyx_L1_error)
     __pyx_t_3 = __pyx_cur_scope->__pyx_v_buf;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __pyx_cur_scope->__pyx_v_b = ((struct __pyx_obj_5mappy_ThreadBuffer *)__pyx_t_3);
     __pyx_t_3 = 0;
   }
   __pyx_L5:;
 
-  /* "mappy.pyx":142
- * 		if buf is None: b = ThreadBuffer()
+  /* "mappy.pyx":145
  * 		else: b = buf
- * 		if seq2 is None: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), NULL, &n_regs, b._b, &self.map_opt)             # <<<<<<<<<<<<<<
- * 		else: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), str.encode(seq2), &n_regs, b._b, &self.map_opt)
  * 
+ * 		_seq = seq if isinstance(seq, bytes) else seq.encode()             # <<<<<<<<<<<<<<
+ * 		if seq2 is None:
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, NULL,  &n_regs, b._b, &self.map_opt)
  */
-  __pyx_t_2 = (__pyx_cur_scope->__pyx_v_seq2 == Py_None);
-  __pyx_t_1 = (__pyx_t_2 != 0);
-  if (__pyx_t_1) {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_5);
+  __pyx_t_2 = PyBytes_Check(__pyx_cur_scope->__pyx_v_seq); 
+  if ((__pyx_t_2 != 0)) {
+    __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq);
+    __pyx_t_3 = __pyx_cur_scope->__pyx_v_seq;
+  } else {
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_seq, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
-    if (!__pyx_t_5) {
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_cur_scope->__pyx_v_seq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+    if (__pyx_t_6) {
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else {
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[2] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_seq};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_GOTREF(__pyx_t_3);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[2] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_seq};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_GOTREF(__pyx_t_3);
-      } else
-      #endif
-      {
-        __pyx_t_6 = PyTuple_New(1+1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 142, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
-        __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq);
-        __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_seq);
-        PyTuple_SET_ITEM(__pyx_t_6, 0+1, __pyx_cur_scope->__pyx_v_seq);
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      }
+      __pyx_t_4 = __Pyx_PyObject_CallNoArg(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
     }
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_3); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_3 = __pyx_t_4;
+    __pyx_t_4 = 0;
+  }
+  __Pyx_GIVEREF(__pyx_t_3);
+  __pyx_cur_scope->__pyx_v__seq = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "mappy.pyx":146
+ * 
+ * 		_seq = seq if isinstance(seq, bytes) else seq.encode()
+ * 		if seq2 is None:             # <<<<<<<<<<<<<<
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, NULL,  &n_regs, b._b, &self.map_opt)
+ * 		else:
+ */
+  __pyx_t_2 = (__pyx_cur_scope->__pyx_v_seq2 == Py_None);
+  __pyx_t_1 = (__pyx_t_2 != 0);
+  if (__pyx_t_1) {
+
+    /* "mappy.pyx":147
+ * 		_seq = seq if isinstance(seq, bytes) else seq.encode()
+ * 		if seq2 is None:
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, NULL,  &n_regs, b._b, &self.map_opt)             # <<<<<<<<<<<<<<
+ * 		else:
+ * 			_seq2 = seq2 if isinstance(seq2, bytes) else seq2.encode()
+ */
+    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_cur_scope->__pyx_v__seq); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 147, __pyx_L1_error)
     __pyx_cur_scope->__pyx_v_regs = mm_map_aux(__pyx_cur_scope->__pyx_v_self->_idx, __pyx_t_7, NULL, (&__pyx_cur_scope->__pyx_v_n_regs), __pyx_cur_scope->__pyx_v_b->_b, (&__pyx_cur_scope->__pyx_v_self->map_opt));
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "mappy.pyx":146
+ * 
+ * 		_seq = seq if isinstance(seq, bytes) else seq.encode()
+ * 		if seq2 is None:             # <<<<<<<<<<<<<<
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, NULL,  &n_regs, b._b, &self.map_opt)
+ * 		else:
+ */
     goto __pyx_L6;
   }
 
-  /* "mappy.pyx":143
- * 		else: b = buf
- * 		if seq2 is None: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), NULL, &n_regs, b._b, &self.map_opt)
- * 		else: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), str.encode(seq2), &n_regs, b._b, &self.map_opt)             # <<<<<<<<<<<<<<
+  /* "mappy.pyx":149
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, NULL,  &n_regs, b._b, &self.map_opt)
+ * 		else:
+ * 			_seq2 = seq2 if isinstance(seq2, bytes) else seq2.encode()             # <<<<<<<<<<<<<<
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, _seq2, &n_regs, b._b, &self.map_opt)
  * 
- * 		for i in range(n_regs):
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-      }
-    }
-    if (!__pyx_t_6) {
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_cur_scope->__pyx_v_seq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = PyBytes_Check(__pyx_cur_scope->__pyx_v_seq2); 
+    if ((__pyx_t_1 != 0)) {
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq2);
+      __pyx_t_3 = __pyx_cur_scope->__pyx_v_seq2;
     } else {
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[2] = {__pyx_t_6, __pyx_cur_scope->__pyx_v_seq};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_GOTREF(__pyx_t_3);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[2] = {__pyx_t_6, __pyx_cur_scope->__pyx_v_seq};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_GOTREF(__pyx_t_3);
-      } else
-      #endif
-      {
-        __pyx_t_5 = PyTuple_New(1+1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6); __pyx_t_6 = NULL;
-        __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq);
-        __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_seq);
-        PyTuple_SET_ITEM(__pyx_t_5, 0+1, __pyx_cur_scope->__pyx_v_seq);
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_seq2, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+        }
       }
-    }
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_3); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_6);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+      if (__pyx_t_6) {
+        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      } else {
+        __pyx_t_4 = __Pyx_PyObject_CallNoArg(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
       }
-    }
-    if (!__pyx_t_6) {
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_cur_scope->__pyx_v_seq2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-    } else {
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_5)) {
-        PyObject *__pyx_temp[2] = {__pyx_t_6, __pyx_cur_scope->__pyx_v_seq2};
-        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_GOTREF(__pyx_t_4);
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
-        PyObject *__pyx_temp[2] = {__pyx_t_6, __pyx_cur_scope->__pyx_v_seq2};
-        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_GOTREF(__pyx_t_4);
-      } else
-      #endif
-      {
-        __pyx_t_8 = PyTuple_New(1+1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
-        __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq2);
-        __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_seq2);
-        PyTuple_SET_ITEM(__pyx_t_8, 0+1, __pyx_cur_scope->__pyx_v_seq2);
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      }
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_3 = __pyx_t_4;
+      __pyx_t_4 = 0;
     }
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_t_4); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L1_error)
-    __pyx_cur_scope->__pyx_v_regs = mm_map_aux(__pyx_cur_scope->__pyx_v_self->_idx, __pyx_t_7, __pyx_t_9, (&__pyx_cur_scope->__pyx_v_n_regs), __pyx_cur_scope->__pyx_v_b->_b, (&__pyx_cur_scope->__pyx_v_self->map_opt));
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GIVEREF(__pyx_t_3);
+    __pyx_cur_scope->__pyx_v__seq2 = __pyx_t_3;
+    __pyx_t_3 = 0;
+
+    /* "mappy.pyx":150
+ * 		else:
+ * 			_seq2 = seq2 if isinstance(seq2, bytes) else seq2.encode()
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, _seq2, &n_regs, b._b, &self.map_opt)             # <<<<<<<<<<<<<<
+ * 
+ * 		for i in range(n_regs):
+ */
+    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_cur_scope->__pyx_v__seq); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_cur_scope->__pyx_v__seq2); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_cur_scope->__pyx_v_regs = mm_map_aux(__pyx_cur_scope->__pyx_v_self->_idx, __pyx_t_7, __pyx_t_8, (&__pyx_cur_scope->__pyx_v_n_regs), __pyx_cur_scope->__pyx_v_b->_b, (&__pyx_cur_scope->__pyx_v_self->map_opt));
   }
   __pyx_L6:;
 
-  /* "mappy.pyx":145
- * 		else: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), str.encode(seq2), &n_regs, b._b, &self.map_opt)
+  /* "mappy.pyx":152
+ * 			regs = cmappy.mm_map_aux(self._idx, _seq, _seq2, &n_regs, b._b, &self.map_opt)
  * 
  * 		for i in range(n_regs):             # <<<<<<<<<<<<<<
  * 			cmappy.mm_reg2hitpy(self._idx, &regs[i], &h)
  * 			cigar = []
  */
-  __pyx_t_10 = __pyx_cur_scope->__pyx_v_n_regs;
-  for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
-    __pyx_cur_scope->__pyx_v_i = __pyx_t_11;
+  __pyx_t_9 = __pyx_cur_scope->__pyx_v_n_regs;
+  for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
+    __pyx_cur_scope->__pyx_v_i = __pyx_t_10;
 
-    /* "mappy.pyx":146
+    /* "mappy.pyx":153
  * 
  * 		for i in range(n_regs):
  * 			cmappy.mm_reg2hitpy(self._idx, &regs[i], &h)             # <<<<<<<<<<<<<<
  * 			cigar = []
  * 			for k in range(h.n_cigar32):
  */
     mm_reg2hitpy(__pyx_cur_scope->__pyx_v_self->_idx, (&(__pyx_cur_scope->__pyx_v_regs[__pyx_cur_scope->__pyx_v_i])), (&__pyx_cur_scope->__pyx_v_h));
 
-    /* "mappy.pyx":147
+    /* "mappy.pyx":154
  * 		for i in range(n_regs):
  * 			cmappy.mm_reg2hitpy(self._idx, &regs[i], &h)
  * 			cigar = []             # <<<<<<<<<<<<<<
  * 			for k in range(h.n_cigar32):
  * 				c = h.cigar32[k]
  */
-    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_cigar);
-    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_cigar, ((PyObject*)__pyx_t_4));
-    __Pyx_GIVEREF(__pyx_t_4);
-    __pyx_t_4 = 0;
+    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_cigar, ((PyObject*)__pyx_t_3));
+    __Pyx_GIVEREF(__pyx_t_3);
+    __pyx_t_3 = 0;
 
-    /* "mappy.pyx":148
+    /* "mappy.pyx":155
  * 			cmappy.mm_reg2hitpy(self._idx, &regs[i], &h)
  * 			cigar = []
  * 			for k in range(h.n_cigar32):             # <<<<<<<<<<<<<<
  * 				c = h.cigar32[k]
  * 				cigar.append([c>>4, c&0xf])
  */
-    __pyx_t_12 = __pyx_cur_scope->__pyx_v_h.n_cigar32;
-    for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
-      __pyx_cur_scope->__pyx_v_k = __pyx_t_13;
+    __pyx_t_11 = __pyx_cur_scope->__pyx_v_h.n_cigar32;
+    for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+      __pyx_cur_scope->__pyx_v_k = __pyx_t_12;
 
-      /* "mappy.pyx":149
+      /* "mappy.pyx":156
  * 			cigar = []
  * 			for k in range(h.n_cigar32):
  * 				c = h.cigar32[k]             # <<<<<<<<<<<<<<
  * 				cigar.append([c>>4, c&0xf])
  * 			yield Alignment(h.ctg, h.ctg_len, h.ctg_start, h.ctg_end, h.strand, h.qry_start, h.qry_end, h.mapq, cigar, h.is_primary, h.mlen, h.blen, h.NM, h.trans_strand, h.seg_id)
  */
-      __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_cur_scope->__pyx_v_h.cigar32[__pyx_cur_scope->__pyx_v_k])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_3 = __Pyx_PyInt_From_uint32_t((__pyx_cur_scope->__pyx_v_h.cigar32[__pyx_cur_scope->__pyx_v_k])); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_c);
-      __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_c, __pyx_t_4);
-      __Pyx_GIVEREF(__pyx_t_4);
-      __pyx_t_4 = 0;
+      __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_c, __pyx_t_3);
+      __Pyx_GIVEREF(__pyx_t_3);
+      __pyx_t_3 = 0;
 
-      /* "mappy.pyx":150
+      /* "mappy.pyx":157
  * 			for k in range(h.n_cigar32):
  * 				c = h.cigar32[k]
  * 				cigar.append([c>>4, c&0xf])             # <<<<<<<<<<<<<<
  * 			yield Alignment(h.ctg, h.ctg_len, h.ctg_start, h.ctg_end, h.strand, h.qry_start, h.qry_end, h.mapq, cigar, h.is_primary, h.mlen, h.blen, h.NM, h.trans_strand, h.seg_id)
  * 			cmappy.mm_free_reg1(&regs[i])
  */
-      __pyx_t_4 = __Pyx_PyInt_RshiftObjC(__pyx_cur_scope->__pyx_v_c, __pyx_int_4, 4, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = __Pyx_PyInt_AndObjC(__pyx_cur_scope->__pyx_v_c, __pyx_int_15, 0xf, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_RshiftObjC(__pyx_cur_scope->__pyx_v_c, __pyx_int_4, 4, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_AndObjC(__pyx_cur_scope->__pyx_v_c, __pyx_int_15, 0xf, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 157, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GIVEREF(__pyx_t_4);
-      PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_3);
-      PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
-      __pyx_t_4 = 0;
+      PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
+      __Pyx_GIVEREF(__pyx_t_4);
+      PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
       __pyx_t_3 = 0;
-      __pyx_t_14 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_cigar, __pyx_t_5); if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __pyx_t_4 = 0;
+      __pyx_t_13 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_cigar, __pyx_t_5); if (unlikely(__pyx_t_13 == -1)) __PYX_ERR(0, 157, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
 
-    /* "mappy.pyx":151
+    /* "mappy.pyx":158
  * 				c = h.cigar32[k]
  * 				cigar.append([c>>4, c&0xf])
  * 			yield Alignment(h.ctg, h.ctg_len, h.ctg_start, h.ctg_end, h.strand, h.qry_start, h.qry_end, h.mapq, cigar, h.is_primary, h.mlen, h.blen, h.NM, h.trans_strand, h.seg_id)             # <<<<<<<<<<<<<<
  * 			cmappy.mm_free_reg1(&regs[i])
  * 		free(regs)
  */
-    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_h.ctg); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_h.ctg); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.ctg_len); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.ctg_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.ctg_len); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.ctg_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 151, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = __Pyx_PyInt_From_int8_t(__pyx_cur_scope->__pyx_v_h.strand); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.ctg_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.ctg_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_15 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.qry_start); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyInt_From_int8_t(__pyx_cur_scope->__pyx_v_h.strand); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_14);
+    __pyx_t_15 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.qry_start); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
-    __pyx_t_16 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.qry_end); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.qry_end); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
-    __pyx_t_17 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_h.mapq); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_h.mapq); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_17);
-    __pyx_t_18 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_h.is_primary); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_h.is_primary); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
-    __pyx_t_19 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.mlen); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.mlen); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
-    __pyx_t_20 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.blen); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.blen); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_20);
-    __pyx_t_21 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.NM); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_21 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.NM); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_21);
-    __pyx_t_22 = __Pyx_PyInt_From_int8_t(__pyx_cur_scope->__pyx_v_h.trans_strand); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_22 = __Pyx_PyInt_From_int8_t(__pyx_cur_scope->__pyx_v_h.trans_strand); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_22);
-    __pyx_t_23 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.seg_id); if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_23 = __Pyx_PyInt_From_int32_t(__pyx_cur_scope->__pyx_v_h.seg_id); if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_23);
-    __pyx_t_24 = PyTuple_New(15); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_24 = PyTuple_New(15); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_24);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_24, 0, __pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_24, 1, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_24, 2, __pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_24, 3, __pyx_t_8);
+    PyTuple_SET_ITEM(__pyx_t_24, 1, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_24, 2, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_24, 4, __pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_24, 3, __pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_14);
+    PyTuple_SET_ITEM(__pyx_t_24, 4, __pyx_t_14);
     __Pyx_GIVEREF(__pyx_t_15);
     PyTuple_SET_ITEM(__pyx_t_24, 5, __pyx_t_15);
     __Pyx_GIVEREF(__pyx_t_16);
     PyTuple_SET_ITEM(__pyx_t_24, 6, __pyx_t_16);
     __Pyx_GIVEREF(__pyx_t_17);
     PyTuple_SET_ITEM(__pyx_t_24, 7, __pyx_t_17);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_cigar);
@@ -4570,65 +4558,65 @@
     __Pyx_GIVEREF(__pyx_t_21);
     PyTuple_SET_ITEM(__pyx_t_24, 12, __pyx_t_21);
     __Pyx_GIVEREF(__pyx_t_22);
     PyTuple_SET_ITEM(__pyx_t_24, 13, __pyx_t_22);
     __Pyx_GIVEREF(__pyx_t_23);
     PyTuple_SET_ITEM(__pyx_t_24, 14, __pyx_t_23);
     __pyx_t_5 = 0;
-    __pyx_t_3 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_8 = 0;
+    __pyx_t_3 = 0;
     __pyx_t_6 = 0;
+    __pyx_t_14 = 0;
     __pyx_t_15 = 0;
     __pyx_t_16 = 0;
     __pyx_t_17 = 0;
     __pyx_t_18 = 0;
     __pyx_t_19 = 0;
     __pyx_t_20 = 0;
     __pyx_t_21 = 0;
     __pyx_t_22 = 0;
     __pyx_t_23 = 0;
-    __pyx_t_23 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5mappy_Alignment), __pyx_t_24, NULL); if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_23 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5mappy_Alignment), __pyx_t_24, NULL); if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_23);
     __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
     __pyx_r = __pyx_t_23;
     __pyx_t_23 = 0;
-    __pyx_cur_scope->__pyx_t_0 = __pyx_t_10;
-    __pyx_cur_scope->__pyx_t_1 = __pyx_t_11;
+    __pyx_cur_scope->__pyx_t_0 = __pyx_t_9;
+    __pyx_cur_scope->__pyx_t_1 = __pyx_t_10;
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L11_resume_from_yield:;
-    __pyx_t_10 = __pyx_cur_scope->__pyx_t_0;
-    __pyx_t_11 = __pyx_cur_scope->__pyx_t_1;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_9 = __pyx_cur_scope->__pyx_t_0;
+    __pyx_t_10 = __pyx_cur_scope->__pyx_t_1;
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 158, __pyx_L1_error)
 
-    /* "mappy.pyx":152
+    /* "mappy.pyx":159
  * 				cigar.append([c>>4, c&0xf])
  * 			yield Alignment(h.ctg, h.ctg_len, h.ctg_start, h.ctg_end, h.strand, h.qry_start, h.qry_end, h.mapq, cigar, h.is_primary, h.mlen, h.blen, h.NM, h.trans_strand, h.seg_id)
  * 			cmappy.mm_free_reg1(&regs[i])             # <<<<<<<<<<<<<<
  * 		free(regs)
  * 
  */
     mm_free_reg1((&(__pyx_cur_scope->__pyx_v_regs[__pyx_cur_scope->__pyx_v_i])));
   }
 
-  /* "mappy.pyx":153
+  /* "mappy.pyx":160
  * 			yield Alignment(h.ctg, h.ctg_len, h.ctg_start, h.ctg_end, h.strand, h.qry_start, h.qry_end, h.mapq, cigar, h.is_primary, h.mlen, h.blen, h.NM, h.trans_strand, h.seg_id)
  * 			cmappy.mm_free_reg1(&regs[i])
  * 		free(regs)             # <<<<<<<<<<<<<<
  * 
- * def fastx_read(fn):
+ * 	def seq(self, str name, int start=0, int end=0x7fffffff):
  */
   free(__pyx_cur_scope->__pyx_v_regs);
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "mappy.pyx":133
+  /* "mappy.pyx":135
  * 		return (self._idx != NULL)
  * 
  * 	def map(self, seq, seq2=None, buf=None):             # <<<<<<<<<<<<<<
  * 		cdef cmappy.mm_reg1_t *regs
  * 		cdef cmappy.mm_hitpy_t h
  */
 
@@ -4636,15 +4624,15 @@
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_XDECREF(__pyx_t_18);
   __Pyx_XDECREF(__pyx_t_19);
   __Pyx_XDECREF(__pyx_t_20);
   __Pyx_XDECREF(__pyx_t_21);
@@ -4656,34 +4644,390 @@
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "mappy.pyx":162
+ * 		free(regs)
+ * 
+ * 	def seq(self, str name, int start=0, int end=0x7fffffff):             # <<<<<<<<<<<<<<
+ * 		cdef int l
+ * 		cdef char *s = cmappy.mappy_fetch_seq(self._idx, name.encode(), start, end, &l)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5mappy_7Aligner_10seq(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_5mappy_7Aligner_10seq(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_name = 0;
+  int __pyx_v_start;
+  int __pyx_v_end;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("seq (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_start,&__pyx_n_s_end,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = PyDict_GetItem(__pyx_kwds, __pyx_n_s_start);
+          if (value) { values[1] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = PyDict_GetItem(__pyx_kwds, __pyx_n_s_end);
+          if (value) { values[2] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "seq") < 0)) __PYX_ERR(0, 162, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_name = ((PyObject*)values[0]);
+    if (values[1]) {
+      __pyx_v_start = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L3_error)
+    } else {
+      __pyx_v_start = ((int)0);
+    }
+    if (values[2]) {
+      __pyx_v_end = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L3_error)
+    } else {
+      __pyx_v_end = ((int)0x7fffffff);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("seq", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 162, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("mappy.Aligner.seq", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyString_Type), 1, "name", 1))) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_r = __pyx_pf_5mappy_7Aligner_9seq(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self), __pyx_v_name, __pyx_v_start, __pyx_v_end);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5mappy_7Aligner_9seq(struct __pyx_obj_5mappy_Aligner *__pyx_v_self, PyObject *__pyx_v_name, int __pyx_v_start, int __pyx_v_end) {
+  int __pyx_v_l;
+  char *__pyx_v_s;
+  PyObject *__pyx_v_r = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  char const *__pyx_t_4;
+  int __pyx_t_5;
+  __Pyx_RefNannySetupContext("seq", 0);
+
+  /* "mappy.pyx":164
+ * 	def seq(self, str name, int start=0, int end=0x7fffffff):
+ * 		cdef int l
+ * 		cdef char *s = cmappy.mappy_fetch_seq(self._idx, name.encode(), start, end, &l)             # <<<<<<<<<<<<<<
+ * 		if l == 0: return None
+ * 		r = s[:l] if isinstance(s, str) else s[:l].decode()
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  if (__pyx_t_3) {
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  } else {
+    __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+  }
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_v_s = mappy_fetch_seq(__pyx_v_self->_idx, __pyx_t_4, __pyx_v_start, __pyx_v_end, (&__pyx_v_l));
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "mappy.pyx":165
+ * 		cdef int l
+ * 		cdef char *s = cmappy.mappy_fetch_seq(self._idx, name.encode(), start, end, &l)
+ * 		if l == 0: return None             # <<<<<<<<<<<<<<
+ * 		r = s[:l] if isinstance(s, str) else s[:l].decode()
+ * 		free(s)
+ */
+  __pyx_t_5 = ((__pyx_v_l == 0) != 0);
+  if (__pyx_t_5) {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(Py_None);
+    __pyx_r = Py_None;
+    goto __pyx_L0;
+  }
+
+  /* "mappy.pyx":166
+ * 		cdef char *s = cmappy.mappy_fetch_seq(self._idx, name.encode(), start, end, &l)
+ * 		if l == 0: return None
+ * 		r = s[:l] if isinstance(s, str) else s[:l].decode()             # <<<<<<<<<<<<<<
+ * 		free(s)
+ * 		return r
+ */
+  __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = PyString_Check(__pyx_t_2); 
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if ((__pyx_t_5 != 0)) {
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s + 0, __pyx_v_l - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __pyx_t_2;
+    __pyx_t_2 = 0;
+  } else {
+    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_s, 0, __pyx_v_l, NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __pyx_t_2;
+    __pyx_t_2 = 0;
+  }
+  __pyx_v_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "mappy.pyx":167
+ * 		if l == 0: return None
+ * 		r = s[:l] if isinstance(s, str) else s[:l].decode()
+ * 		free(s)             # <<<<<<<<<<<<<<
+ * 		return r
+ * 
+ */
+  free(__pyx_v_s);
+
+  /* "mappy.pyx":168
+ * 		r = s[:l] if isinstance(s, str) else s[:l].decode()
+ * 		free(s)
+ * 		return r             # <<<<<<<<<<<<<<
+ * 
+ * 	@property
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_r);
+  __pyx_r = __pyx_v_r;
+  goto __pyx_L0;
+
+  /* "mappy.pyx":162
+ * 		free(regs)
+ * 
+ * 	def seq(self, str name, int start=0, int end=0x7fffffff):             # <<<<<<<<<<<<<<
+ * 		cdef int l
+ * 		cdef char *s = cmappy.mappy_fetch_seq(self._idx, name.encode(), start, end, &l)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("mappy.Aligner.seq", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_r);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "mappy.pyx":171
+ * 
+ * 	@property
+ * 	def k(self): return self._idx.k             # <<<<<<<<<<<<<<
+ * 
+ * 	@property
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5mappy_7Aligner_1k_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5mappy_7Aligner_1k_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5mappy_7Aligner_1k___get__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5mappy_7Aligner_1k___get__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_self->_idx->k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("mappy.Aligner.k.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "mappy.pyx":174
+ * 
+ * 	@property
+ * 	def w(self): return self._idx.w             # <<<<<<<<<<<<<<
+ * 
+ * 	@property
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5mappy_7Aligner_1w_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5mappy_7Aligner_1w_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5mappy_7Aligner_1w___get__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5mappy_7Aligner_1w___get__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_self->_idx->w); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("mappy.Aligner.w.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "mappy.pyx":177
+ * 
+ * 	@property
+ * 	def n_seq(self): return self._idx.n_seq             # <<<<<<<<<<<<<<
+ * 
+ * def fastx_read(fn, read_comment=False):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5mappy_7Aligner_5n_seq_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5mappy_7Aligner_5n_seq_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5mappy_7Aligner_5n_seq___get__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5mappy_7Aligner_5n_seq___get__(struct __pyx_obj_5mappy_Aligner *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_idx->n_seq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("mappy.Aligner.n_seq.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5mappy_7Aligner_10__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_5mappy_7Aligner_10__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_5mappy_7Aligner_12__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_5mappy_7Aligner_12__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5mappy_7Aligner_9__reduce_cython__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5mappy_7Aligner_11__reduce_cython__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5mappy_7Aligner_9__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self) {
+static PyObject *__pyx_pf_5mappy_7Aligner_11__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
@@ -4717,27 +5061,27 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5mappy_7Aligner_12__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_5mappy_7Aligner_12__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_5mappy_7Aligner_14__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_5mappy_7Aligner_14__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5mappy_7Aligner_11__setstate_cython__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_5mappy_7Aligner_13__setstate_cython__(((struct __pyx_obj_5mappy_Aligner *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5mappy_7Aligner_11__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_5mappy_7Aligner_13__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5mappy_Aligner *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
@@ -4764,54 +5108,109 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_5mappy_2generator1(__pyx_CoroutineObject *__pyx_generator, PyObject *__pyx_sent_value); /* proto */
 
-/* "mappy.pyx":155
- * 		free(regs)
+/* "mappy.pyx":179
+ * 	def n_seq(self): return self._idx.n_seq
  * 
- * def fastx_read(fn):             # <<<<<<<<<<<<<<
+ * def fastx_read(fn, read_comment=False):             # <<<<<<<<<<<<<<
  * 	cdef cmappy.kseq_t *ks
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5mappy_1fastx_read(PyObject *__pyx_self, PyObject *__pyx_v_fn); /*proto*/
-static PyMethodDef __pyx_mdef_5mappy_1fastx_read = {"fastx_read", (PyCFunction)__pyx_pw_5mappy_1fastx_read, METH_O, 0};
-static PyObject *__pyx_pw_5mappy_1fastx_read(PyObject *__pyx_self, PyObject *__pyx_v_fn) {
+static PyObject *__pyx_pw_5mappy_1fastx_read(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5mappy_1fastx_read = {"fastx_read", (PyCFunction)__pyx_pw_5mappy_1fastx_read, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5mappy_1fastx_read(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_fn = 0;
+  PyObject *__pyx_v_read_comment = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fastx_read (wrapper)", 0);
-  __pyx_r = __pyx_pf_5mappy_fastx_read(__pyx_self, ((PyObject *)__pyx_v_fn));
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fn,&__pyx_n_s_read_comment,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)Py_False);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = PyDict_GetItem(__pyx_kwds, __pyx_n_s_fn)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = PyDict_GetItem(__pyx_kwds, __pyx_n_s_read_comment);
+          if (value) { values[1] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fastx_read") < 0)) __PYX_ERR(0, 179, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_fn = values[0];
+    __pyx_v_read_comment = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("fastx_read", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 179, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("mappy.fastx_read", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_5mappy_fastx_read(__pyx_self, __pyx_v_fn, __pyx_v_read_comment);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5mappy_fastx_read(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fn) {
+static PyObject *__pyx_pf_5mappy_fastx_read(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fn, PyObject *__pyx_v_read_comment) {
   struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fastx_read", 0);
   __pyx_cur_scope = (struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *)__pyx_tp_new_5mappy___pyx_scope_struct_1_fastx_read(__pyx_ptype_5mappy___pyx_scope_struct_1_fastx_read, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 155, __pyx_L1_error)
+    __PYX_ERR(0, 179, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_fn = __pyx_v_fn;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_fn);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_fn);
+  __pyx_cur_scope->__pyx_v_read_comment = __pyx_v_read_comment;
+  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_read_comment);
+  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_read_comment);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_5mappy_2generator1, (PyObject *) __pyx_cur_scope, __pyx_n_s_fastx_read, __pyx_n_s_fastx_read, __pyx_n_s_mappy); if (unlikely(!gen)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_5mappy_2generator1, (PyObject *) __pyx_cur_scope, __pyx_n_s_fastx_read, __pyx_n_s_fastx_read, __pyx_n_s_mappy); if (unlikely(!gen)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4834,252 +5233,355 @@
   char const *__pyx_t_5;
   int __pyx_t_6;
   char *__pyx_t_7;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("None", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
-    case 1: goto __pyx_L8_resume_from_yield;
+    case 1: goto __pyx_L10_resume_from_yield;
+    case 2: goto __pyx_L11_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 155, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "mappy.pyx":157
- * def fastx_read(fn):
+  /* "mappy.pyx":181
+ * def fastx_read(fn, read_comment=False):
  * 	cdef cmappy.kseq_t *ks
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))             # <<<<<<<<<<<<<<
  * 	if ks is NULL: return None
  * 	while cmappy.kseq_read(ks) >= 0:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyString_Type)), __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   if (!__pyx_t_3) {
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_cur_scope->__pyx_v_fn); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_cur_scope->__pyx_v_fn); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
   } else {
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[2] = {__pyx_t_3, __pyx_cur_scope->__pyx_v_fn};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[2] = {__pyx_t_3, __pyx_cur_scope->__pyx_v_fn};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     {
-      __pyx_t_4 = PyTuple_New(1+1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(1+1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3); __pyx_t_3 = NULL;
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_fn);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_fn);
       PyTuple_SET_ITEM(__pyx_t_4, 0+1, __pyx_cur_scope->__pyx_v_fn);
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
   __pyx_cur_scope->__pyx_v_ks = mm_fastx_open(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mappy.pyx":158
+  /* "mappy.pyx":182
  * 	cdef cmappy.kseq_t *ks
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))
  * 	if ks is NULL: return None             # <<<<<<<<<<<<<<
  * 	while cmappy.kseq_read(ks) >= 0:
  * 		if ks.qual.l > 0: qual = ks.qual.s if isinstance(ks.qual.s, str) else ks.qual.s.decode()
  */
   __pyx_t_6 = ((__pyx_cur_scope->__pyx_v_ks == NULL) != 0);
   if (__pyx_t_6) {
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = NULL; __Pyx_ReturnWithStopIteration(Py_None);
     goto __pyx_L0;
   }
 
-  /* "mappy.pyx":159
+  /* "mappy.pyx":183
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))
  * 	if ks is NULL: return None
  * 	while cmappy.kseq_read(ks) >= 0:             # <<<<<<<<<<<<<<
  * 		if ks.qual.l > 0: qual = ks.qual.s if isinstance(ks.qual.s, str) else ks.qual.s.decode()
  * 		else: qual = None
  */
   while (1) {
     __pyx_t_6 = ((kseq_read(__pyx_cur_scope->__pyx_v_ks) >= 0) != 0);
     if (!__pyx_t_6) break;
 
-    /* "mappy.pyx":160
+    /* "mappy.pyx":184
  * 	if ks is NULL: return None
  * 	while cmappy.kseq_read(ks) >= 0:
  * 		if ks.qual.l > 0: qual = ks.qual.s if isinstance(ks.qual.s, str) else ks.qual.s.decode()             # <<<<<<<<<<<<<<
  * 		else: qual = None
  * 		name = ks.name.s if isinstance(ks.name.s, str) else ks.name.s.decode()
  */
     __pyx_t_6 = ((__pyx_cur_scope->__pyx_v_ks->qual.l > 0) != 0);
     if (__pyx_t_6) {
-      __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->qual.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->qual.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_6 = PyString_Check(__pyx_t_2); 
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if ((__pyx_t_6 != 0)) {
-        __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->qual.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->qual.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_1 = __pyx_t_2;
         __pyx_t_2 = 0;
       } else {
         __pyx_t_7 = __pyx_cur_scope->__pyx_v_ks->qual.s;
-        __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_2);
         __pyx_t_1 = __pyx_t_2;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_qual);
       __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_qual, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_1);
       __pyx_t_1 = 0;
       goto __pyx_L7;
     }
 
-    /* "mappy.pyx":161
+    /* "mappy.pyx":185
  * 	while cmappy.kseq_read(ks) >= 0:
  * 		if ks.qual.l > 0: qual = ks.qual.s if isinstance(ks.qual.s, str) else ks.qual.s.decode()
  * 		else: qual = None             # <<<<<<<<<<<<<<
  * 		name = ks.name.s if isinstance(ks.name.s, str) else ks.name.s.decode()
  * 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()
  */
     /*else*/ {
       __Pyx_INCREF(Py_None);
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_qual);
       __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_qual, Py_None);
       __Pyx_GIVEREF(Py_None);
     }
     __pyx_L7:;
 
-    /* "mappy.pyx":162
+    /* "mappy.pyx":186
  * 		if ks.qual.l > 0: qual = ks.qual.s if isinstance(ks.qual.s, str) else ks.qual.s.decode()
  * 		else: qual = None
  * 		name = ks.name.s if isinstance(ks.name.s, str) else ks.name.s.decode()             # <<<<<<<<<<<<<<
  * 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()
- * 		yield name, seq, qual
+ * 		if read_comment:
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->name.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->name.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = PyString_Check(__pyx_t_2); 
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if ((__pyx_t_6 != 0)) {
-      __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->name.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->name.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_1 = __pyx_t_2;
       __pyx_t_2 = 0;
     } else {
       __pyx_t_7 = __pyx_cur_scope->__pyx_v_ks->name.s;
-      __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_2);
       __pyx_t_1 = __pyx_t_2;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_name);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_name, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "mappy.pyx":163
+    /* "mappy.pyx":187
  * 		else: qual = None
  * 		name = ks.name.s if isinstance(ks.name.s, str) else ks.name.s.decode()
  * 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()             # <<<<<<<<<<<<<<
- * 		yield name, seq, qual
- * 	cmappy.mm_fastx_close(ks)
+ * 		if read_comment:
+ * 			if ks.comment.l > 0: comment = ks.comment.s if isinstance(ks.comment.s, str) else ks.comment.s.decode()
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->seq.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->seq.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = PyString_Check(__pyx_t_2); 
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if ((__pyx_t_6 != 0)) {
-      __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->seq.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->seq.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_1 = __pyx_t_2;
       __pyx_t_2 = 0;
     } else {
       __pyx_t_7 = __pyx_cur_scope->__pyx_v_ks->seq.s;
-      __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_2);
       __pyx_t_1 = __pyx_t_2;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_seq);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_seq, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "mappy.pyx":164
+    /* "mappy.pyx":188
+ * 		name = ks.name.s if isinstance(ks.name.s, str) else ks.name.s.decode()
+ * 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()
+ * 		if read_comment:             # <<<<<<<<<<<<<<
+ * 			if ks.comment.l > 0: comment = ks.comment.s if isinstance(ks.comment.s, str) else ks.comment.s.decode()
+ * 			else: comment = None
+ */
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_read_comment); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
+    if (__pyx_t_6) {
+
+      /* "mappy.pyx":189
+ * 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()
+ * 		if read_comment:
+ * 			if ks.comment.l > 0: comment = ks.comment.s if isinstance(ks.comment.s, str) else ks.comment.s.decode()             # <<<<<<<<<<<<<<
+ * 			else: comment = None
+ * 			yield name, seq, qual, comment
+ */
+      __pyx_t_6 = ((__pyx_cur_scope->__pyx_v_ks->comment.l > 0) != 0);
+      if (__pyx_t_6) {
+        __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->comment.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_6 = PyString_Check(__pyx_t_2); 
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if ((__pyx_t_6 != 0)) {
+          __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_cur_scope->__pyx_v_ks->comment.s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_1 = __pyx_t_2;
+          __pyx_t_2 = 0;
+        } else {
+          __pyx_t_7 = __pyx_cur_scope->__pyx_v_ks->comment.s;
+          __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_2);
+          __pyx_t_1 = __pyx_t_2;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        }
+        __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_comment);
+        __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_comment, __pyx_t_1);
+        __Pyx_GIVEREF(__pyx_t_1);
+        __pyx_t_1 = 0;
+        goto __pyx_L9;
+      }
+
+      /* "mappy.pyx":190
+ * 		if read_comment:
+ * 			if ks.comment.l > 0: comment = ks.comment.s if isinstance(ks.comment.s, str) else ks.comment.s.decode()
+ * 			else: comment = None             # <<<<<<<<<<<<<<
+ * 			yield name, seq, qual, comment
+ * 		else:
+ */
+      /*else*/ {
+        __Pyx_INCREF(Py_None);
+        __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_comment);
+        __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_comment, Py_None);
+        __Pyx_GIVEREF(Py_None);
+      }
+      __pyx_L9:;
+
+      /* "mappy.pyx":191
+ * 			if ks.comment.l > 0: comment = ks.comment.s if isinstance(ks.comment.s, str) else ks.comment.s.decode()
+ * 			else: comment = None
+ * 			yield name, seq, qual, comment             # <<<<<<<<<<<<<<
+ * 		else:
+ * 			yield name, seq, qual
+ */
+      __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name);
+      PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_v_name);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_seq);
+      PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_cur_scope->__pyx_v_seq);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_qual);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_qual);
+      PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_cur_scope->__pyx_v_qual);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_comment);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_comment);
+      PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_cur_scope->__pyx_v_comment);
+      __pyx_r = __pyx_t_1;
+      __pyx_t_1 = 0;
+      __Pyx_XGIVEREF(__pyx_r);
+      __Pyx_RefNannyFinishContext();
+      /* return from generator, yielding value */
+      __pyx_generator->resume_label = 1;
+      return __pyx_r;
+      __pyx_L10_resume_from_yield:;
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 191, __pyx_L1_error)
+
+      /* "mappy.pyx":188
  * 		name = ks.name.s if isinstance(ks.name.s, str) else ks.name.s.decode()
  * 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()
- * 		yield name, seq, qual             # <<<<<<<<<<<<<<
+ * 		if read_comment:             # <<<<<<<<<<<<<<
+ * 			if ks.comment.l > 0: comment = ks.comment.s if isinstance(ks.comment.s, str) else ks.comment.s.decode()
+ * 			else: comment = None
+ */
+      goto __pyx_L8;
+    }
+
+    /* "mappy.pyx":193
+ * 			yield name, seq, qual, comment
+ * 		else:
+ * 			yield name, seq, qual             # <<<<<<<<<<<<<<
  * 	cmappy.mm_fastx_close(ks)
  * 
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name);
-    __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_v_name);
-    __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq);
-    __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_seq);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_cur_scope->__pyx_v_seq);
-    __Pyx_INCREF(__pyx_cur_scope->__pyx_v_qual);
-    __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_qual);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_cur_scope->__pyx_v_qual);
-    __pyx_r = __pyx_t_1;
-    __pyx_t_1 = 0;
-    __Pyx_XGIVEREF(__pyx_r);
-    __Pyx_RefNannyFinishContext();
-    /* return from generator, yielding value */
-    __pyx_generator->resume_label = 1;
-    return __pyx_r;
-    __pyx_L8_resume_from_yield:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 164, __pyx_L1_error)
+    /*else*/ {
+      __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_name);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_name);
+      PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_v_name);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_seq);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_seq);
+      PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_cur_scope->__pyx_v_seq);
+      __Pyx_INCREF(__pyx_cur_scope->__pyx_v_qual);
+      __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_qual);
+      PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_cur_scope->__pyx_v_qual);
+      __pyx_r = __pyx_t_1;
+      __pyx_t_1 = 0;
+      __Pyx_XGIVEREF(__pyx_r);
+      __Pyx_RefNannyFinishContext();
+      /* return from generator, yielding value */
+      __pyx_generator->resume_label = 2;
+      return __pyx_r;
+      __pyx_L11_resume_from_yield:;
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 193, __pyx_L1_error)
+    }
+    __pyx_L8:;
   }
 
-  /* "mappy.pyx":165
- * 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()
- * 		yield name, seq, qual
+  /* "mappy.pyx":194
+ * 		else:
+ * 			yield name, seq, qual
  * 	cmappy.mm_fastx_close(ks)             # <<<<<<<<<<<<<<
  * 
- * def verbose(v=None):
+ * def revcomp(seq):
  */
   mm_fastx_close(__pyx_cur_scope->__pyx_v_ks);
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "mappy.pyx":155
- * 		free(regs)
+  /* "mappy.pyx":179
+ * 	def n_seq(self): return self._idx.n_seq
  * 
- * def fastx_read(fn):             # <<<<<<<<<<<<<<
+ * def fastx_read(fn, read_comment=False):             # <<<<<<<<<<<<<<
  * 	cdef cmappy.kseq_t *ks
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))
  */
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -5093,26 +5595,192 @@
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mappy.pyx":167
+/* "mappy.pyx":196
  * 	cmappy.mm_fastx_close(ks)
  * 
+ * def revcomp(seq):             # <<<<<<<<<<<<<<
+ * 	l = len(seq)
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5mappy_4revcomp(PyObject *__pyx_self, PyObject *__pyx_v_seq); /*proto*/
+static PyMethodDef __pyx_mdef_5mappy_4revcomp = {"revcomp", (PyCFunction)__pyx_pw_5mappy_4revcomp, METH_O, 0};
+static PyObject *__pyx_pw_5mappy_4revcomp(PyObject *__pyx_self, PyObject *__pyx_v_seq) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("revcomp (wrapper)", 0);
+  __pyx_r = __pyx_pf_5mappy_3revcomp(__pyx_self, ((PyObject *)__pyx_v_seq));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5mappy_3revcomp(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq) {
+  Py_ssize_t __pyx_v_l;
+  PyObject *__pyx_v_bseq = NULL;
+  char *__pyx_v_s;
+  PyObject *__pyx_v_r = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  uint8_t const *__pyx_t_7;
+  __Pyx_RefNannySetupContext("revcomp", 0);
+
+  /* "mappy.pyx":197
+ * 
+ * def revcomp(seq):
+ * 	l = len(seq)             # <<<<<<<<<<<<<<
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()
+ * 	cdef char *s = cmappy.mappy_revcomp(l, bseq)
+ */
+  __pyx_t_1 = PyObject_Length(__pyx_v_seq); if (unlikely(__pyx_t_1 == -1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_v_l = __pyx_t_1;
+
+  /* "mappy.pyx":198
+ * def revcomp(seq):
+ * 	l = len(seq)
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()             # <<<<<<<<<<<<<<
+ * 	cdef char *s = cmappy.mappy_revcomp(l, bseq)
+ * 	r = s[:l] if isinstance(s, str) else s[:l].decode()
+ */
+  __pyx_t_3 = PyBytes_Check(__pyx_v_seq); 
+  if ((__pyx_t_3 != 0)) {
+    __Pyx_INCREF(__pyx_v_seq);
+    __pyx_t_2 = __pyx_v_seq;
+  } else {
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_seq, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+      }
+    }
+    if (__pyx_t_6) {
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    } else {
+      __pyx_t_4 = __Pyx_PyObject_CallNoArg(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
+    }
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_2 = __pyx_t_4;
+    __pyx_t_4 = 0;
+  }
+  __pyx_v_bseq = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "mappy.pyx":199
+ * 	l = len(seq)
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()
+ * 	cdef char *s = cmappy.mappy_revcomp(l, bseq)             # <<<<<<<<<<<<<<
+ * 	r = s[:l] if isinstance(s, str) else s[:l].decode()
+ * 	free(s)
+ */
+  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_bseq); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_v_s = mappy_revcomp(__pyx_v_l, __pyx_t_7);
+
+  /* "mappy.pyx":200
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()
+ * 	cdef char *s = cmappy.mappy_revcomp(l, bseq)
+ * 	r = s[:l] if isinstance(s, str) else s[:l].decode()             # <<<<<<<<<<<<<<
+ * 	free(s)
+ * 	return r
+ */
+  __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_s); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = PyString_Check(__pyx_t_4); 
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if ((__pyx_t_3 != 0)) {
+    __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s + 0, __pyx_v_l - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_2 = __pyx_t_4;
+    __pyx_t_4 = 0;
+  } else {
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_s, 0, __pyx_v_l, NULL, NULL, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_2 = __pyx_t_4;
+    __pyx_t_4 = 0;
+  }
+  __pyx_v_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "mappy.pyx":201
+ * 	cdef char *s = cmappy.mappy_revcomp(l, bseq)
+ * 	r = s[:l] if isinstance(s, str) else s[:l].decode()
+ * 	free(s)             # <<<<<<<<<<<<<<
+ * 	return r
+ * 
+ */
+  free(__pyx_v_s);
+
+  /* "mappy.pyx":202
+ * 	r = s[:l] if isinstance(s, str) else s[:l].decode()
+ * 	free(s)
+ * 	return r             # <<<<<<<<<<<<<<
+ * 
+ * def verbose(v=None):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_r);
+  __pyx_r = __pyx_v_r;
+  goto __pyx_L0;
+
+  /* "mappy.pyx":196
+ * 	cmappy.mm_fastx_close(ks)
+ * 
+ * def revcomp(seq):             # <<<<<<<<<<<<<<
+ * 	l = len(seq)
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("mappy.revcomp", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_bseq);
+  __Pyx_XDECREF(__pyx_v_r);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "mappy.pyx":204
+ * 	return r
+ * 
  * def verbose(v=None):             # <<<<<<<<<<<<<<
  * 	if v is None: v = -1
  * 	return cmappy.mm_verbose_level(v)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5mappy_4verbose(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_5mappy_4verbose = {"verbose", (PyCFunction)__pyx_pw_5mappy_4verbose, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_5mappy_4verbose(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5mappy_6verbose(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_5mappy_6verbose = {"verbose", (PyCFunction)__pyx_pw_5mappy_6verbose, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_5mappy_6verbose(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_v = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("verbose (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_v,0};
     PyObject* values[1] = {0};
@@ -5131,79 +5799,79 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = PyDict_GetItem(__pyx_kwds, __pyx_n_s_v);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "verbose") < 0)) __PYX_ERR(0, 167, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "verbose") < 0)) __PYX_ERR(0, 204, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_v = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("verbose", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 167, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("verbose", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 204, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("mappy.verbose", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_5mappy_3verbose(__pyx_self, __pyx_v_v);
+  __pyx_r = __pyx_pf_5mappy_5verbose(__pyx_self, __pyx_v_v);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5mappy_3verbose(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_v) {
+static PyObject *__pyx_pf_5mappy_5verbose(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_v) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("verbose", 0);
   __Pyx_INCREF(__pyx_v_v);
 
-  /* "mappy.pyx":168
+  /* "mappy.pyx":205
  * 
  * def verbose(v=None):
  * 	if v is None: v = -1             # <<<<<<<<<<<<<<
  * 	return cmappy.mm_verbose_level(v)
  */
   __pyx_t_1 = (__pyx_v_v == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
     __Pyx_INCREF(__pyx_int_neg_1);
     __Pyx_DECREF_SET(__pyx_v_v, __pyx_int_neg_1);
   }
 
-  /* "mappy.pyx":169
+  /* "mappy.pyx":206
  * def verbose(v=None):
  * 	if v is None: v = -1
  * 	return cmappy.mm_verbose_level(v)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_v); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyInt_From_int(mm_verbose_level(__pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_v); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(mm_verbose_level(__pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "mappy.pyx":167
- * 	cmappy.mm_fastx_close(ks)
+  /* "mappy.pyx":204
+ * 	return r
  * 
  * def verbose(v=None):             # <<<<<<<<<<<<<<
  * 	if v is None: v = -1
  * 	return cmappy.mm_verbose_level(v)
  */
 
   /* function exit code */
@@ -5546,21 +6214,41 @@
     __pyx_pw_5mappy_7Aligner_3__dealloc__(o);
     --Py_REFCNT(o);
     PyErr_Restore(etype, eval, etb);
   }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
+static PyObject *__pyx_getprop_5mappy_7Aligner_k(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5mappy_7Aligner_1k_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_5mappy_7Aligner_w(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5mappy_7Aligner_1w_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_5mappy_7Aligner_n_seq(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5mappy_7Aligner_5n_seq_1__get__(o);
+}
+
 static PyMethodDef __pyx_methods_5mappy_Aligner[] = {
   {"map", (PyCFunction)__pyx_pw_5mappy_7Aligner_7map, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_5mappy_7Aligner_10__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_5mappy_7Aligner_12__setstate_cython__, METH_O, 0},
+  {"seq", (PyCFunction)__pyx_pw_5mappy_7Aligner_10seq, METH_VARARGS|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_5mappy_7Aligner_12__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_5mappy_7Aligner_14__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
+static struct PyGetSetDef __pyx_getsets_5mappy_Aligner[] = {
+  {(char *)"k", __pyx_getprop_5mappy_7Aligner_k, 0, (char *)0, 0},
+  {(char *)"w", __pyx_getprop_5mappy_7Aligner_w, 0, (char *)0, 0},
+  {(char *)"n_seq", __pyx_getprop_5mappy_7Aligner_n_seq, 0, (char *)0, 0},
+  {0, 0, 0, 0, 0}
+};
+
 static PyNumberMethods __pyx_tp_as_number_Aligner = {
   0, /*nb_add*/
   0, /*nb_subtract*/
   0, /*nb_multiply*/
   #if PY_MAJOR_VERSION < 3 || (CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x03050000)
   0, /*nb_divide*/
   #endif
@@ -5650,15 +6338,15 @@
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_5mappy_Aligner, /*tp_methods*/
   0, /*tp_members*/
-  0, /*tp_getset*/
+  __pyx_getsets_5mappy_Aligner, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
@@ -5693,14 +6381,16 @@
   }
   return o;
 }
 
 static void __pyx_tp_dealloc_5mappy___pyx_scope_struct__map(PyObject *o) {
   struct __pyx_obj_5mappy___pyx_scope_struct__map *p = (struct __pyx_obj_5mappy___pyx_scope_struct__map *)o;
   PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->__pyx_v__seq);
+  Py_CLEAR(p->__pyx_v__seq2);
   Py_CLEAR(p->__pyx_v_b);
   Py_CLEAR(p->__pyx_v_buf);
   Py_CLEAR(p->__pyx_v_c);
   Py_CLEAR(p->__pyx_v_cigar);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_seq);
   Py_CLEAR(p->__pyx_v_seq2);
@@ -5710,14 +6400,20 @@
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_5mappy___pyx_scope_struct__map(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_5mappy___pyx_scope_struct__map *p = (struct __pyx_obj_5mappy___pyx_scope_struct__map *)o;
+  if (p->__pyx_v__seq) {
+    e = (*v)(p->__pyx_v__seq, a); if (e) return e;
+  }
+  if (p->__pyx_v__seq2) {
+    e = (*v)(p->__pyx_v__seq2, a); if (e) return e;
+  }
   if (p->__pyx_v_b) {
     e = (*v)(((PyObject *)p->__pyx_v_b), a); if (e) return e;
   }
   if (p->__pyx_v_buf) {
     e = (*v)(p->__pyx_v_buf, a); if (e) return e;
   }
   if (p->__pyx_v_c) {
@@ -5737,14 +6433,20 @@
   }
   return 0;
 }
 
 static int __pyx_tp_clear_5mappy___pyx_scope_struct__map(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_5mappy___pyx_scope_struct__map *p = (struct __pyx_obj_5mappy___pyx_scope_struct__map *)o;
+  tmp = ((PyObject*)p->__pyx_v__seq);
+  p->__pyx_v__seq = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->__pyx_v__seq2);
+  p->__pyx_v__seq2 = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_b);
   p->__pyx_v_b = ((struct __pyx_obj_5mappy_ThreadBuffer *)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_buf);
   p->__pyx_v_buf = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_c);
@@ -5839,55 +6541,69 @@
   }
   return o;
 }
 
 static void __pyx_tp_dealloc_5mappy___pyx_scope_struct_1_fastx_read(PyObject *o) {
   struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *p = (struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *)o;
   PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->__pyx_v_comment);
   Py_CLEAR(p->__pyx_v_fn);
   Py_CLEAR(p->__pyx_v_name);
   Py_CLEAR(p->__pyx_v_qual);
+  Py_CLEAR(p->__pyx_v_read_comment);
   Py_CLEAR(p->__pyx_v_seq);
   if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_5mappy___pyx_scope_struct_1_fastx_read < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read)))) {
     __pyx_freelist_5mappy___pyx_scope_struct_1_fastx_read[__pyx_freecount_5mappy___pyx_scope_struct_1_fastx_read++] = ((struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
 static int __pyx_tp_traverse_5mappy___pyx_scope_struct_1_fastx_read(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *p = (struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *)o;
+  if (p->__pyx_v_comment) {
+    e = (*v)(p->__pyx_v_comment, a); if (e) return e;
+  }
   if (p->__pyx_v_fn) {
     e = (*v)(p->__pyx_v_fn, a); if (e) return e;
   }
   if (p->__pyx_v_name) {
     e = (*v)(p->__pyx_v_name, a); if (e) return e;
   }
   if (p->__pyx_v_qual) {
     e = (*v)(p->__pyx_v_qual, a); if (e) return e;
   }
+  if (p->__pyx_v_read_comment) {
+    e = (*v)(p->__pyx_v_read_comment, a); if (e) return e;
+  }
   if (p->__pyx_v_seq) {
     e = (*v)(p->__pyx_v_seq, a); if (e) return e;
   }
   return 0;
 }
 
 static int __pyx_tp_clear_5mappy___pyx_scope_struct_1_fastx_read(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *p = (struct __pyx_obj_5mappy___pyx_scope_struct_1_fastx_read *)o;
+  tmp = ((PyObject*)p->__pyx_v_comment);
+  p->__pyx_v_comment = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_fn);
   p->__pyx_v_fn = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_name);
   p->__pyx_v_name = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_qual);
   p->__pyx_v_qual = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->__pyx_v_read_comment);
+  p->__pyx_v_read_comment = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
   tmp = ((PyObject*)p->__pyx_v_seq);
   p->__pyx_v_seq = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyTypeObject __pyx_type_5mappy___pyx_scope_struct_1_fastx_read = {
@@ -5980,36 +6696,41 @@
   {&__pyx_kp_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 0},
   {&__pyx_kp_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 0},
   {&__pyx_kp_s__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 1, 0},
   {&__pyx_kp_s__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 1, 0},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_best_n, __pyx_k_best_n, sizeof(__pyx_k_best_n), 0, 0, 1, 1},
   {&__pyx_n_s_blen, __pyx_k_blen, sizeof(__pyx_k_blen), 0, 0, 1, 1},
+  {&__pyx_n_s_bseq, __pyx_k_bseq, sizeof(__pyx_k_bseq), 0, 0, 1, 1},
   {&__pyx_n_s_buf, __pyx_k_buf, sizeof(__pyx_k_buf), 0, 0, 1, 1},
   {&__pyx_n_s_bw, __pyx_k_bw, sizeof(__pyx_k_bw), 0, 0, 1, 1},
   {&__pyx_n_s_ce, __pyx_k_ce, sizeof(__pyx_k_ce), 0, 0, 1, 1},
   {&__pyx_kp_s_cg_Z, __pyx_k_cg_Z, sizeof(__pyx_k_cg_Z), 0, 0, 1, 0},
   {&__pyx_n_s_cigar, __pyx_k_cigar, sizeof(__pyx_k_cigar), 0, 0, 1, 1},
   {&__pyx_n_s_cigar_str, __pyx_k_cigar_str, sizeof(__pyx_k_cigar_str), 0, 0, 1, 1},
   {&__pyx_n_s_cl, __pyx_k_cl, sizeof(__pyx_k_cl), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+  {&__pyx_n_s_comment, __pyx_k_comment, sizeof(__pyx_k_comment), 0, 0, 1, 1},
   {&__pyx_n_s_cs, __pyx_k_cs, sizeof(__pyx_k_cs), 0, 0, 1, 1},
   {&__pyx_n_s_ctg, __pyx_k_ctg, sizeof(__pyx_k_ctg), 0, 0, 1, 1},
   {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
+  {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
   {&__pyx_n_s_fastx_read, __pyx_k_fastx_read, sizeof(__pyx_k_fastx_read), 0, 0, 1, 1},
   {&__pyx_n_s_fn, __pyx_k_fn, sizeof(__pyx_k_fn), 0, 0, 1, 1},
   {&__pyx_n_s_fn_idx_in, __pyx_k_fn_idx_in, sizeof(__pyx_k_fn_idx_in), 0, 0, 1, 1},
   {&__pyx_n_s_fn_idx_out, __pyx_k_fn_idx_out, sizeof(__pyx_k_fn_idx_out), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_is_primary, __pyx_k_is_primary, sizeof(__pyx_k_is_primary), 0, 0, 1, 1},
   {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_ks, __pyx_k_ks, sizeof(__pyx_k_ks), 0, 0, 1, 1},
+  {&__pyx_n_s_l, __pyx_k_l, sizeof(__pyx_k_l), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_map, __pyx_k_map, sizeof(__pyx_k_map), 0, 0, 1, 1},
   {&__pyx_n_s_mappy, __pyx_k_mappy, sizeof(__pyx_k_mappy), 0, 0, 1, 1},
   {&__pyx_n_s_mapq, __pyx_k_mapq, sizeof(__pyx_k_mapq), 0, 0, 1, 1},
   {&__pyx_n_s_min_chain_score, __pyx_k_min_chain_score, sizeof(__pyx_k_min_chain_score), 0, 0, 1, 1},
   {&__pyx_n_s_min_cnt, __pyx_k_min_cnt, sizeof(__pyx_k_min_cnt), 0, 0, 1, 1},
   {&__pyx_n_s_min_dp_score, __pyx_k_min_dp_score, sizeof(__pyx_k_min_dp_score), 0, 0, 1, 1},
@@ -6019,42 +6740,48 @@
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_preset, __pyx_k_preset, sizeof(__pyx_k_preset), 0, 0, 1, 1},
   {&__pyx_kp_s_python_mappy_pyx, __pyx_k_python_mappy_pyx, sizeof(__pyx_k_python_mappy_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_qe, __pyx_k_qe, sizeof(__pyx_k_qe), 0, 0, 1, 1},
   {&__pyx_n_s_qs, __pyx_k_qs, sizeof(__pyx_k_qs), 0, 0, 1, 1},
   {&__pyx_n_s_qual, __pyx_k_qual, sizeof(__pyx_k_qual), 0, 0, 1, 1},
+  {&__pyx_n_s_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+  {&__pyx_n_s_read_comment, __pyx_k_read_comment, sizeof(__pyx_k_read_comment), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+  {&__pyx_n_s_revcomp, __pyx_k_revcomp, sizeof(__pyx_k_revcomp), 0, 0, 1, 1},
+  {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_s_seg_id, __pyx_k_seg_id, sizeof(__pyx_k_seg_id), 0, 0, 1, 1},
   {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
   {&__pyx_n_s_seq, __pyx_k_seq, sizeof(__pyx_k_seq), 0, 0, 1, 1},
   {&__pyx_n_s_seq2, __pyx_k_seq2, sizeof(__pyx_k_seq2), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_strand, __pyx_k_strand, sizeof(__pyx_k_strand), 0, 0, 1, 1},
+  {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_kp_s_tp_A_P, __pyx_k_tp_A_P, sizeof(__pyx_k_tp_A_P), 0, 0, 1, 0},
   {&__pyx_kp_s_tp_A_S, __pyx_k_tp_A_S, sizeof(__pyx_k_tp_A_S), 0, 0, 1, 0},
   {&__pyx_n_s_trans_strand, __pyx_k_trans_strand, sizeof(__pyx_k_trans_strand), 0, 0, 1, 1},
   {&__pyx_kp_s_ts_A, __pyx_k_ts_A, sizeof(__pyx_k_ts_A), 0, 0, 1, 0},
   {&__pyx_kp_s_ts_A_2, __pyx_k_ts_A_2, sizeof(__pyx_k_ts_A_2), 0, 0, 1, 0},
   {&__pyx_kp_s_ts_A_3, __pyx_k_ts_A_3, sizeof(__pyx_k_ts_A_3), 0, 0, 1, 0},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_verbose, __pyx_k_verbose, sizeof(__pyx_k_verbose), 0, 0, 1, 1},
   {&__pyx_n_s_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 75, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 152, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6113,37 +6840,49 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "mappy.pyx":155
- * 		free(regs)
+  /* "mappy.pyx":179
+ * 	def n_seq(self): return self._idx.n_seq
  * 
- * def fastx_read(fn):             # <<<<<<<<<<<<<<
+ * def fastx_read(fn, read_comment=False):             # <<<<<<<<<<<<<<
  * 	cdef cmappy.kseq_t *ks
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))
  */
-  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_fn, __pyx_n_s_ks, __pyx_n_s_qual, __pyx_n_s_name_2, __pyx_n_s_seq); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(7, __pyx_n_s_fn, __pyx_n_s_read_comment, __pyx_n_s_ks, __pyx_n_s_qual, __pyx_n_s_name, __pyx_n_s_seq, __pyx_n_s_comment); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, 0, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_mappy_pyx, __pyx_n_s_fastx_read, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, 0, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_mappy_pyx, __pyx_n_s_fastx_read, 179, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "mappy.pyx":167
+  /* "mappy.pyx":196
  * 	cmappy.mm_fastx_close(ks)
  * 
+ * def revcomp(seq):             # <<<<<<<<<<<<<<
+ * 	l = len(seq)
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()
+ */
+  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_seq, __pyx_n_s_l, __pyx_n_s_bseq, __pyx_n_s_s, __pyx_n_s_r); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, 0, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_mappy_pyx, __pyx_n_s_revcomp, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 196, __pyx_L1_error)
+
+  /* "mappy.pyx":204
+ * 	return r
+ * 
  * def verbose(v=None):             # <<<<<<<<<<<<<<
  * 	if v is None: v = -1
  * 	return cmappy.mm_verbose_level(v)
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_v); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 167, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, 0, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_mappy_pyx, __pyx_n_s_verbose, 167, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_v); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, 0, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_python_mappy_pyx, __pyx_n_s_verbose, 204, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -6239,74 +6978,98 @@
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global init code ---*/
   /*--- Variable export code ---*/
   /*--- Function export code ---*/
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_5mappy_Alignment) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5mappy_Alignment) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __pyx_type_5mappy_Alignment.tp_print = 0;
-  if (PyObject_SetAttrString(__pyx_m, "Alignment", (PyObject *)&__pyx_type_5mappy_Alignment) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5mappy_Alignment) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "Alignment", (PyObject *)&__pyx_type_5mappy_Alignment) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5mappy_Alignment) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __pyx_ptype_5mappy_Alignment = &__pyx_type_5mappy_Alignment;
-  if (PyType_Ready(&__pyx_type_5mappy_ThreadBuffer) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5mappy_ThreadBuffer) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
   __pyx_type_5mappy_ThreadBuffer.tp_print = 0;
-  if (PyObject_SetAttrString(__pyx_m, "ThreadBuffer", (PyObject *)&__pyx_type_5mappy_ThreadBuffer) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5mappy_ThreadBuffer) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "ThreadBuffer", (PyObject *)&__pyx_type_5mappy_ThreadBuffer) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5mappy_ThreadBuffer) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
   __pyx_ptype_5mappy_ThreadBuffer = &__pyx_type_5mappy_ThreadBuffer;
-  if (PyType_Ready(&__pyx_type_5mappy_Aligner) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5mappy_Aligner) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   __pyx_type_5mappy_Aligner.tp_print = 0;
-  if (PyObject_SetAttrString(__pyx_m, "Aligner", (PyObject *)&__pyx_type_5mappy_Aligner) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5mappy_Aligner) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "Aligner", (PyObject *)&__pyx_type_5mappy_Aligner) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5mappy_Aligner) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   __pyx_ptype_5mappy_Aligner = &__pyx_type_5mappy_Aligner;
-  if (PyType_Ready(&__pyx_type_5mappy___pyx_scope_struct__map) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5mappy___pyx_scope_struct__map) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
   __pyx_type_5mappy___pyx_scope_struct__map.tp_print = 0;
   __pyx_ptype_5mappy___pyx_scope_struct__map = &__pyx_type_5mappy___pyx_scope_struct__map;
-  if (PyType_Ready(&__pyx_type_5mappy___pyx_scope_struct_1_fastx_read) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5mappy___pyx_scope_struct_1_fastx_read) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __pyx_type_5mappy___pyx_scope_struct_1_fastx_read.tp_print = 0;
   __pyx_ptype_5mappy___pyx_scope_struct_1_fastx_read = &__pyx_type_5mappy___pyx_scope_struct_1_fastx_read;
   /*--- Type import code ---*/
   /*--- Variable import code ---*/
   /*--- Function import code ---*/
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "mappy.pyx":5
+  /* "mappy.pyx":4
+ * from libc.stdlib cimport free
  * cimport cmappy
+ * import sys             # <<<<<<<<<<<<<<
+ * 
+ * cmappy.mm_reset_timer()
+ */
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_sys, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sys, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "mappy.pyx":6
+ * import sys
  * 
  * cmappy.mm_reset_timer()             # <<<<<<<<<<<<<<
  * 
  * cdef class Alignment:
  */
   mm_reset_timer();
 
-  /* "mappy.pyx":155
- * 		free(regs)
+  /* "mappy.pyx":179
+ * 	def n_seq(self): return self._idx.n_seq
  * 
- * def fastx_read(fn):             # <<<<<<<<<<<<<<
+ * def fastx_read(fn, read_comment=False):             # <<<<<<<<<<<<<<
  * 	cdef cmappy.kseq_t *ks
  * 	ks = cmappy.mm_fastx_open(str.encode(fn))
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5mappy_1fastx_read, NULL, __pyx_n_s_mappy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5mappy_1fastx_read, NULL, __pyx_n_s_mappy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fastx_read, __pyx_t_1) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fastx_read, __pyx_t_1) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mappy.pyx":167
+  /* "mappy.pyx":196
  * 	cmappy.mm_fastx_close(ks)
  * 
+ * def revcomp(seq):             # <<<<<<<<<<<<<<
+ * 	l = len(seq)
+ * 	bseq = seq if isinstance(seq, bytes) else seq.encode()
+ */
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5mappy_4revcomp, NULL, __pyx_n_s_mappy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_revcomp, __pyx_t_1) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "mappy.pyx":204
+ * 	return r
+ * 
  * def verbose(v=None):             # <<<<<<<<<<<<<<
  * 	if v is None: v = -1
  * 	return cmappy.mm_verbose_level(v)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5mappy_4verbose, NULL, __pyx_n_s_mappy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5mappy_6verbose, NULL, __pyx_n_s_mappy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_verbose, __pyx_t_1) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_verbose, __pyx_t_1) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "mappy.pyx":1
  * from libc.stdint cimport uint8_t, int8_t             # <<<<<<<<<<<<<<
  * from libc.stdlib cimport free
  * cimport cmappy
  */
@@ -7947,14 +8710,41 @@
         
     }
     #endif
     return (inplace ? PyNumber_InPlaceAnd : PyNumber_And)(op1, op2);
 }
 #endif
 
+/* ArgTypeTest */
+        static void __Pyx_RaiseArgumentTypeInvalid(const char* name, PyObject *obj, PyTypeObject *type) {
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
+}
+static CYTHON_INLINE int __Pyx_ArgTypeTest(PyObject *obj, PyTypeObject *type, int none_allowed,
+    const char *name, int exact)
+{
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (none_allowed && obj == Py_None) return 1;
+    else if (exact) {
+        if (likely(Py_TYPE(obj) == type)) return 1;
+        #if PY_MAJOR_VERSION == 2
+        else if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(PyObject_TypeCheck(obj, type))) return 1;
+    }
+    __Pyx_RaiseArgumentTypeInvalid(name, obj, type);
+    return 0;
+}
+
 /* decode_c_string */
         static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
     if (unlikely((start < 0) | (stop < 0))) {
@@ -7984,15 +8774,15 @@
     }
 }
 
 /* SetupReduce */
         static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
-  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name);
+  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
   }
   if (unlikely(ret < 0)) {
       PyErr_Clear();
@@ -8056,14 +8846,88 @@
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
+/* Import */
+        static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *empty_list = 0;
+    PyObject *module = 0;
+    PyObject *global_dict = 0;
+    PyObject *empty_dict = 0;
+    PyObject *list;
+    #if PY_VERSION_HEX < 0x03030000
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (!py_import)
+        goto bad;
+    #endif
+    if (from_list)
+        list = from_list;
+    else {
+        empty_list = PyList_New(0);
+        if (!empty_list)
+            goto bad;
+        list = empty_list;
+    }
+    global_dict = PyModule_GetDict(__pyx_m);
+    if (!global_dict)
+        goto bad;
+    empty_dict = PyDict_New();
+    if (!empty_dict)
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if (strchr(__Pyx_MODULE_NAME, '.')) {
+                #if PY_VERSION_HEX < 0x03030000
+                PyObject *py_level = PyInt_FromLong(1);
+                if (!py_level)
+                    goto bad;
+                module = PyObject_CallFunctionObjArgs(py_import,
+                    name, global_dict, empty_dict, list, py_level, NULL);
+                Py_DECREF(py_level);
+                #else
+                module = PyImport_ImportModuleLevelObject(
+                    name, global_dict, empty_dict, list, 1);
+                #endif
+                if (!module) {
+                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_VERSION_HEX < 0x03030000
+            PyObject *py_level = PyInt_FromLong(level);
+            if (!py_level)
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, global_dict, empty_dict, list, py_level, NULL);
+            Py_DECREF(py_level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, global_dict, empty_dict, list, level);
+            #endif
+        }
+    }
+bad:
+    #if PY_VERSION_HEX < 0x03030000
+    Py_XDECREF(py_import);
+    #endif
+    Py_XDECREF(empty_list);
+    Py_XDECREF(empty_dict);
+    return module;
+}
+
 /* CLineInTraceback */
         static int __Pyx_CLineForTraceback(int c_line) {
 #ifdef CYTHON_CLINE_IN_TRACEBACK
     return ((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0;
 #else
     PyObject *use_cline;
 #if CYTHON_COMPILING_IN_CPYTHON
```

### Comparing `mappy-2.8/python/mappy.pyx` & `mappy-2.9/python/mappy.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from libc.stdint cimport uint8_t, int8_t
 from libc.stdlib cimport free
 cimport cmappy
+import sys
 
 cmappy.mm_reset_timer()
 
 cdef class Alignment:
 	cdef int _ctg_len, _r_st, _r_en
 	cdef int _q_st, _q_en
 	cdef int _NM, _mlen, _blen
@@ -107,25 +108,26 @@
 		self.idx_opt.batch_size = 0x7fffffffffffffffL # always build a uni-part index
 		if k is not None: self.idx_opt.k = k
 		if w is not None: self.idx_opt.w = w
 		if min_cnt is not None: self.map_opt.min_cnt = min_cnt
 		if min_chain_score is not None: self.map_opt.min_chain_score = min_chain_score
 		if min_dp_score is not None: self.map_opt.min_dp_max = min_dp_score
 		if bw is not None: self.map_opt.bw = bw
-		if best_n is not None: self.best_n = best_n
+		if best_n is not None: self.map_opt.best_n = best_n
 
 		cdef cmappy.mm_idx_reader_t *r;
 		if fn_idx_out is None:
 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, NULL)
 		else:
 			r = cmappy.mm_idx_reader_open(str.encode(fn_idx_in), &self.idx_opt, fn_idx_out)
 		if r is not NULL:
 			self._idx = cmappy.mm_idx_reader_read(r, n_threads) # NB: ONLY read the first part
 			cmappy.mm_idx_reader_close(r)
 			cmappy.mm_mapopt_update(&self.map_opt, self._idx)
+			cmappy.mm_idx_index_name(self._idx)
 
 	def __dealloc__(self):
 		if self._idx is not NULL:
 			cmappy.mm_idx_destroy(self._idx)
 
 	def __bool__(self):
 		return (self._idx != NULL)
@@ -135,35 +137,70 @@
 		cdef cmappy.mm_hitpy_t h
 		cdef ThreadBuffer b
 		cdef int n_regs
 
 		if self._idx is NULL: return None
 		if buf is None: b = ThreadBuffer()
 		else: b = buf
-		if seq2 is None: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), NULL, &n_regs, b._b, &self.map_opt)
-		else: regs = cmappy.mm_map_aux(self._idx, str.encode(seq), str.encode(seq2), &n_regs, b._b, &self.map_opt)
+
+		_seq = seq if isinstance(seq, bytes) else seq.encode()
+		if seq2 is None:
+			regs = cmappy.mm_map_aux(self._idx, _seq, NULL,  &n_regs, b._b, &self.map_opt)
+		else:
+			_seq2 = seq2 if isinstance(seq2, bytes) else seq2.encode()
+			regs = cmappy.mm_map_aux(self._idx, _seq, _seq2, &n_regs, b._b, &self.map_opt)
 
 		for i in range(n_regs):
 			cmappy.mm_reg2hitpy(self._idx, &regs[i], &h)
 			cigar = []
 			for k in range(h.n_cigar32):
 				c = h.cigar32[k]
 				cigar.append([c>>4, c&0xf])
 			yield Alignment(h.ctg, h.ctg_len, h.ctg_start, h.ctg_end, h.strand, h.qry_start, h.qry_end, h.mapq, cigar, h.is_primary, h.mlen, h.blen, h.NM, h.trans_strand, h.seg_id)
 			cmappy.mm_free_reg1(&regs[i])
 		free(regs)
 
-def fastx_read(fn):
+	def seq(self, str name, int start=0, int end=0x7fffffff):
+		cdef int l
+		cdef char *s = cmappy.mappy_fetch_seq(self._idx, name.encode(), start, end, &l)
+		if l == 0: return None
+		r = s[:l] if isinstance(s, str) else s[:l].decode()
+		free(s)
+		return r
+
+	@property
+	def k(self): return self._idx.k
+
+	@property
+	def w(self): return self._idx.w
+
+	@property
+	def n_seq(self): return self._idx.n_seq
+
+def fastx_read(fn, read_comment=False):
 	cdef cmappy.kseq_t *ks
 	ks = cmappy.mm_fastx_open(str.encode(fn))
 	if ks is NULL: return None
 	while cmappy.kseq_read(ks) >= 0:
 		if ks.qual.l > 0: qual = ks.qual.s if isinstance(ks.qual.s, str) else ks.qual.s.decode()
 		else: qual = None
 		name = ks.name.s if isinstance(ks.name.s, str) else ks.name.s.decode()
 		seq = ks.seq.s if isinstance(ks.seq.s, str) else ks.seq.s.decode()
-		yield name, seq, qual
+		if read_comment:
+			if ks.comment.l > 0: comment = ks.comment.s if isinstance(ks.comment.s, str) else ks.comment.s.decode()
+			else: comment = None
+			yield name, seq, qual, comment
+		else:
+			yield name, seq, qual
 	cmappy.mm_fastx_close(ks)
 
+def revcomp(seq):
+	l = len(seq)
+	bseq = seq if isinstance(seq, bytes) else seq.encode()
+	cdef char *s = cmappy.mappy_revcomp(l, bseq)
+	r = s[:l] if isinstance(s, str) else s[:l].decode()
+	free(s)
+	return r
+
 def verbose(v=None):
 	if v is None: v = -1
 	return cmappy.mm_verbose_level(v)
```

### Comparing `mappy-2.8/python/minimap2.py` & `mappy-2.9/python/minimap2.py`

 * *Files identical despite different names*

### Comparing `mappy-2.8/python/README.rst` & `mappy-2.9/python/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 The following Python script demonstrates the key functionality of mappy:
 
 .. code:: python
 
 	import mappy as mp
 	a = mp.Aligner("test/MT-human.fa")  # load or build index
 	if not a: raise Exception("ERROR: failed to load/build index")
+	s = a.seq("MT_human", 100, 200)     # retrieve a subsequence from the index
+	print(mp.revcomp(s))                # reverse complement
 	for name, seq, qual in mp.fastx_read("test/MT-orang.fa"): # read a fasta/q sequence
 		for hit in a.map(seq): # traverse alignments
 			print("{}\t{}\t{}\t{}".format(hit.ctg, hit.r_st, hit.r_en, hit.cigar_str))
 
 APIs
 ----
 
@@ -83,15 +85,23 @@
 
 	mappy.Aligner.map(seq, seq2=None)
 
 This method aligns :code:`seq` against the index. It is a generator, *yielding*
 a series of :code:`mappy.Alignment` objects. If :code:`seq2` is present, mappy
 performs paired-end alignment, assuming the two ends are in the FR orientation.
 Alignments of the two ends can be distinguished by the :code:`read_num` field
-(see below).
+(see Class mappy.Alignment below).
+
+.. code:: python
+
+	mappy.Aligner.seq(name, start=0, end=0x7fffffff)
+
+This method retrieves a (sub)sequence from the index and returns it as a Python
+string. :code:`None` is returned if :code:`name` is not present in the index or
+the start/end coordinates are invalid.
 
 Class mappy.Alignment
 ~~~~~~~~~~~~~~~~~~~~~
 
 This class describes an alignment. An object of this class has the following
 properties:
 
@@ -135,17 +145,26 @@
 ::
 
 	q_st  q_en  strand  ctg  ctg_len  r_st  r_en  mlen  blen  mapq  cg:Z:cigar_str
 
 It is effectively the PAF format without the QueryName and QueryLength columns
 (the first two columns in PAF).
 
-Function mappy.fastx_read
-~~~~~~~~~~~~~~~~~~~~~~~~~
+Miscellaneous Functions
+~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: python
 
-	mappy.fastx_read(fn)
+	mappy.fastx_read(fn, read_comment=False)
 
 This generator function opens a FASTA/FASTQ file and *yields* a
 :code:`(name,seq,qual)` tuple for each sequence entry. The input file may be
-optionally gzip'd.
+optionally gzip'd. If :code:`read_comment` is True, this generator yields
+a :code:`(name,seq,qual,comment)` tuple instead.
+
+.. code:: python
+
+	mappy.revcomp(seq)
+
+Return the reverse complement of DNA string :code:`seq`. This function
+recognizes IUB code and preserves the letter cases. Uracil :code:`U` is
+complemented to :code:`A`.
```

### Comparing `mappy-2.8/README.md` & `mappy-2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     - [Map long mRNA/cDNA reads](#map-long-splice)
     - [Find overlaps between long reads](#long-overlap)
     - [Map short accurate genomic reads](#short-genomic)
     - [Full genome/assembly alignment](#full-genome)
   - [Advanced features](#advanced)
     - [Working with >65535 CIGAR operations](#long-cigar)
     - [The cs optional tag](#cs)
-    - [Evaluation scripts](#eval)
+    - [Working with the PAF format](#paftools)
   - [Algorithm overview](#algo)
   - [Getting help](#help)
   - [Citing minimap2](#cite)
 - [Developers' Guide](#dguide)
 - [Limitations](#limit)
 
 ## <a name="uguide"></a>Users' Guide
@@ -64,17 +64,17 @@
 Detailed evaluations are available from the [minimap2 preprint][preprint].
 
 ### <a name="install"></a>Installation
 
 Minimap2 is optimized for x86-64 CPUs. You can acquire precompiled binaries from
 the [release page][release] with:
 ```sh
-curl -L https://github.com/lh3/minimap2/releases/download/v2.8/minimap2-2.8_x64-linux.tar.bz2 \
+curl -L https://github.com/lh3/minimap2/releases/download/v2.9/minimap2-2.9_x64-linux.tar.bz2 \
   | tar -jxvf -
-./minimap2-2.8_x64-linux/minimap2
+./minimap2-2.9_x64-linux/minimap2
 ```
 If you want to compile from the source, you need to have a C compiler, GNU make
 and zlib development files installed. Then type `make` in the source code
 directory to compile. If you see compilation errors, try `make sse2only=1`
 to disable SSE4 code, which will make minimap2 slightly slower.
 
 Minimap2 also works with ARM CPUs supporting the NEON instruction sets. To
@@ -252,34 +252,21 @@
 similar to the `MD` SAM tag but is standalone and easier to parse.
 
 If `--cs=long` is used, the `cs` string also contains identical sequences in
 the alignment. The above example will become
 `=CGATCG-ata=AATAGAGTAG+gtc=GAAT*at=GCA`. The long form of `cs` encodes both
 reference and query sequences in one string.
 
-#### <a name="eval"></a>Evaluation scripts
+#### <a name="paftools"></a>Working with the PAF format
 
-Minimap2 comes with several (java)scripts for evaluating the accuracy of
-minimap2. These scripts require the [k8][k8] javascript shell to run.
-Recent minimap2 binary release tar-balls contain a copy of k8 executable, a
-single file. Here are a few examples on how to use these scripts:
-
-```sh
-# Generate reads from PBSIM alignment (truth encoded in read names)
-k8 misc/sim-pbsim.js ref.fa.fai pbsim-aln.maf > pbsim-reads.fq
-# Generate reads from mason2 alignment (not tested for simulated SVs)
-k8 misc/sim-mason2.js mason2-aln.sam > mason2-reads.fq
-# Evaluate mapping accuracy with ROC-like curve
-k8 misc/sim-eval.js my-aln.sam.gz > result.txt
-k8 misc/sim-eval.js my-aln.paf.gz > result.txt
-# Collect alignment statistics
-k8 misc/mapstat.js my-aln.sam > result.txt
-# Compare spliced junctions to existing gene annotations
-k8 misc/intron-eval.js anno.gtf my-spliced-aln.sam > result.txt
-```
+Minimap2 also comes with a (java)script [paftools.js](misc/paftools.js) that
+processes alignments in the PAF format. It calls variants from
+assembly-to-reference alignment, lifts over BED files based on alignment,
+converts between formats and provides utilities for various evaluations. For
+details, please see [misc/README.md](misc/README.md).
 
 ### <a name="algo"></a>Algorithm overview
 
 In the following, minimap2 command line options have a dash ahead and are
 highlighted in bold. The description may help to tune minimap2 parameters.
 
 1. Read **-I** [=*4G*] reference bases, extract (**-k**,**-w**)-minimizers and
```

### Comparing `mappy-2.8/sdust.c` & `mappy-2.9/sdust.c`

 * *Files identical despite different names*

### Comparing `mappy-2.8/sdust.h` & `mappy-2.9/sdust.h`

 * *Files identical despite different names*

### Comparing `mappy-2.8/setup.py` & `mappy-2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def readme():
     with open('python/README.rst') as f:
         return f.read()
 
 setup(
 	name = 'mappy',
-	version = '2.8',
+	version = '2.9',
 	url = 'https://github.com/lh3/minimap2',
 	description = 'Minimap2 python binding',
 	long_description = readme(),
 	author = 'Heng Li',
 	author_email = 'lh3@me.com',
 	license = 'MIT',
 	keywords = 'sequence-alignment',
@@ -39,15 +39,15 @@
 		depends = ['minimap.h', 'bseq.h', 'kalloc.h', 'kdq.h', 'khash.h', 'kseq.h', 'ksort.h',
 				   'ksw2.h', 'kthread.h', 'kvec.h', 'mmpriv.h', 'sdust.h',
 				   'python/cmappy.h', 'python/cmappy.pxd'],
 		extra_compile_args = ['-DHAVE_KALLOC', '-msse4'], # WARNING: ancient x86_64 CPUs don't have SSE4
 		include_dirs = ['.'],
 		libraries = ['z', 'm', 'pthread'])],
 	classifiers = [
-		'Development Status :: 4 - Beta',
+		'Development Status :: 5 - Production/Stable',
 		'License :: OSI Approved :: MIT License',
 		'Operating System :: POSIX',
 		'Programming Language :: C',
 		'Programming Language :: Cython',
 		'Programming Language :: Python :: 2.7',
 		'Programming Language :: Python :: 3',
 		'Intended Audience :: Science/Research',
```

### Comparing `mappy-2.8/sketch.c` & `mappy-2.9/sketch.c`

 * *Files identical despite different names*

