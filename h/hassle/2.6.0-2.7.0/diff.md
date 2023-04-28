# Comparing `tmp/hassle-2.6.0.tar.gz` & `tmp/hassle-2.7.0.tar.gz`

## Comparing `hassle-2.6.0.tar` & `hassle-2.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 hassle-2.6.0/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/index.html
--rw-r--r--   0        0        0    42579 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/search.js
--rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   121512 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   112334 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165766 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/new_project.html
--rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/new_project.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.6.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.6.0/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.6.0/README.md
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 hassle-2.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/index.html
+-rw-r--r--   0        0        0    42579 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/search.js
+-rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   122450 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   112334 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165766 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/new_project.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.7.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.7.0/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.7.0/README.md
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.7.0/PKG-INFO
```

### Comparing `hassle-2.6.0/CHANGELOG.md` & `hassle-2.7.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/docs/hassle.html` & `hassle-2.7.0/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/docs/search.js` & `hassle-2.7.0/docs/search.js`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/docs/hassle/generate_tests.html` & `hassle-2.7.0/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/docs/hassle/hassle.html` & `hassle-2.7.0/docs/hassle/hassle.html`

 * *Files 0% similar despite different names*

```diff
@@ -248,43 +248,46 @@
 </span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
 </span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
 </span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
 </span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
 </span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="c1"># commit changelog first</span>
 </span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="nb">input</span><span class="p">(</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="p">)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -490,39 +493,42 @@
 </span><span id="main-190"><a href="#main-190"><span class="linenos">190</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="main-191"><a href="#main-191"><span class="linenos">191</span></a>
 </span><span id="main-192"><a href="#main-192"><span class="linenos">192</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
 </span><span id="main-193"><a href="#main-193"><span class="linenos">193</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
 </span><span id="main-194"><a href="#main-194"><span class="linenos">194</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
 </span><span id="main-195"><a href="#main-195"><span class="linenos">195</span></a>        <span class="c1"># commit changelog first</span>
 </span><span id="main-196"><a href="#main-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-197"><a href="#main-197"><span class="linenos">197</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-198"><a href="#main-198"><span class="linenos">198</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="main-199"><a href="#main-199"><span class="linenos">199</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="main-200"><a href="#main-200"><span class="linenos">200</span></a>
-</span><span id="main-201"><a href="#main-201"><span class="linenos">201</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="main-202"><a href="#main-202"><span class="linenos">202</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-203"><a href="#main-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>
-</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-197"><a href="#main-197"><span class="linenos">197</span></a>            <span class="nb">input</span><span class="p">(</span>
+</span><span id="main-198"><a href="#main-198"><span class="linenos">198</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
+</span><span id="main-199"><a href="#main-199"><span class="linenos">199</span></a>            <span class="p">)</span>
+</span><span id="main-200"><a href="#main-200"><span class="linenos">200</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-201"><a href="#main-201"><span class="linenos">201</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
+</span><span id="main-202"><a href="#main-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
+</span><span id="main-203"><a href="#main-203"><span class="linenos">203</span></a>
+</span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
+</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>
-</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
 </span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>
-</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>
-</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
+</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>
+</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
+</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -208,45 +208,49 @@
 189        os.system(f"py -m build {args.package}")
 190
 191    if args.update_changelog:
 192        hassle_utilities.update_changelog(pyproject_path)
 193        # If we're going to add tag for current version
 194        # commit changelog first
 195        if args.tag_version:
-196            os.chdir(args.package)
-197            os.system("git add CHANGELOG.md")
-198            os.system('git commit CHANGELOG.md -m "chore: update
+196            input(
+197                "Press enter to continue after optionally pruning the
+updated changelog..."
+198            )
+199            os.chdir(args.package)
+200            os.system("git add CHANGELOG.md")
+201            os.system('git commit CHANGELOG.md -m "chore: update
 changelog"')
-199
-200    if args.commit_all:
-201        os.chdir(args.package)
-202        if args.commit_all == "build":
-203            version = pyproject_path.loads()["project"]["version"]
-204            args.commit_all = f"chore: build v{version}"
-205        os.system("git add .")
-206        os.system(f'git commit -m "{args.commit_all}"')
-207
-208    if args.tag_version:
-209        hassle_utilities.tag_version(args.package)
+202
+203    if args.commit_all:
+204        os.chdir(args.package)
+205        if args.commit_all == "build":
+206            version = pyproject_path.loads()["project"]["version"]
+207            args.commit_all = f"chore: build v{version}"
+208        os.system("git add .")
+209        os.system(f'git commit -m "{args.commit_all}"')
 210
-211    if args.publish:
-212        os.system(f"twine upload {args.package / 'dist' / '*'}")
+211    if args.tag_version:
+212        hassle_utilities.tag_version(args.package)
 213
-214    if args.install:
-215        os.system(f"pip install {args.package} --no-deps --upgrade --no-
-cache-dir")
+214    if args.publish:
+215        os.system(f"twine upload {args.package / 'dist' / '*'}")
 216
-217    if args.sync:
-218        os.chdir(args.package)
-219        os.system(f"git pull --tags origin main")
-220        os.system(f"git push origin main:main --tags")
-221
-222
-223if __name__ == "__main__":
-224    main(get_args())
+217    if args.install:
+218        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+cache-dir")
+219
+220    if args.sync:
+221        os.chdir(args.package)
+222        os.system(f"git pull --tags origin main")
+223        os.system(f"git push origin main:main --tags")
+224
+225
+226if __name__ == "__main__":
+227    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
 _14def get_args() -> argparse.Namespace:
 _15    parser = argparse.ArgumentParser()
 _16
 _17    parser.add_argument(
 _18        "package",
@@ -432,35 +436,39 @@
 190        os.system(f"py -m build {args.package}")
 191
 192    if args.update_changelog:
 193        hassle_utilities.update_changelog(pyproject_path)
 194        # If we're going to add tag for current version
 195        # commit changelog first
 196        if args.tag_version:
-197            os.chdir(args.package)
-198            os.system("git add CHANGELOG.md")
-199            os.system('git commit CHANGELOG.md -m "chore: update
+197            input(
+198                "Press enter to continue after optionally pruning the
+updated changelog..."
+199            )
+200            os.chdir(args.package)
+201            os.system("git add CHANGELOG.md")
+202            os.system('git commit CHANGELOG.md -m "chore: update
 changelog"')
-200
-201    if args.commit_all:
-202        os.chdir(args.package)
-203        if args.commit_all == "build":
-204            version = pyproject_path.loads()["project"]["version"]
-205            args.commit_all = f"chore: build v{version}"
-206        os.system("git add .")
-207        os.system(f'git commit -m "{args.commit_all}"')
-208
-209    if args.tag_version:
-210        hassle_utilities.tag_version(args.package)
+203
+204    if args.commit_all:
+205        os.chdir(args.package)
+206        if args.commit_all == "build":
+207            version = pyproject_path.loads()["project"]["version"]
+208            args.commit_all = f"chore: build v{version}"
+209        os.system("git add .")
+210        os.system(f'git commit -m "{args.commit_all}"')
 211
-212    if args.publish:
-213        os.system(f"twine upload {args.package / 'dist' / '*'}")
+212    if args.tag_version:
+213        hassle_utilities.tag_version(args.package)
 214
-215    if args.install:
-216        os.system(f"pip install {args.package} --no-deps --upgrade --no-
-cache-dir")
+215    if args.publish:
+216        os.system(f"twine upload {args.package / 'dist' / '*'}")
 217
-218    if args.sync:
-219        os.chdir(args.package)
-220        os.system(f"git pull --tags origin main")
-221        os.system(f"git push origin main:main --tags")
+218    if args.install:
+219        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+cache-dir")
+220
+221    if args.sync:
+222        os.chdir(args.package)
+223        os.system(f"git pull --tags origin main")
+224        os.system(f"git push origin main:main --tags")
```

### Comparing `hassle-2.6.0/docs/hassle/hassle_config.html` & `hassle-2.7.0/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/docs/hassle/hassle_utilities.html` & `hassle-2.7.0/docs/hassle/hassle_utilities.html`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/docs/hassle/new_project.html` & `hassle-2.7.0/docs/hassle/new_project.html`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/docs/hassle/run_tests.html` & `hassle-2.7.0/docs/hassle/run_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/src/hassle/generate_tests.py` & `hassle-2.7.0/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/src/hassle/hassle.py` & `hassle-2.7.0/src/hassle/hassle.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,17 @@
         os.system(f"py -m build {args.package}")
 
     if args.update_changelog:
         hassle_utilities.update_changelog(pyproject_path)
         # If we're going to add tag for current version
         # commit changelog first
         if args.tag_version:
+            input(
+                "Press enter to continue after optionally pruning the updated changelog..."
+            )
             os.chdir(args.package)
             os.system("git add CHANGELOG.md")
             os.system('git commit CHANGELOG.md -m "chore: update changelog"')
 
     if args.commit_all:
         os.chdir(args.package)
         if args.commit_all == "build":
```

### Comparing `hassle-2.6.0/src/hassle/hassle_config.py` & `hassle-2.7.0/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/src/hassle/hassle_utilities.py` & `hassle-2.7.0/src/hassle/hassle_utilities.py`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/src/hassle/license_template.txt` & `hassle-2.7.0/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/src/hassle/new_project.py` & `hassle-2.7.0/src/hassle/new_project.py`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/src/hassle/pyproject_template.toml` & `hassle-2.7.0/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/src/hassle/run_tests.py` & `hassle-2.7.0/src/hassle/run_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/LICENSE.txt` & `hassle-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/README.md` & `hassle-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.6.0/pyproject.toml` & `hassle-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 362e 3022 0d0a 7265 7175 6972 6573  2.6.0"..requires
+00000100: 322e 372e 3022 0d0a 7265 7175 6972 6573  2.7.0"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..
```

### Comparing `hassle-2.6.0/PKG-INFO` & `hassle-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.6.0
+Version: 2.7.0
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

