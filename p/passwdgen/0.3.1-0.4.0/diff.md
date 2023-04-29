# Comparing `tmp/passwdgen-0.3.1.tar.gz` & `tmp/passwdgen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/passwdgen-0.3.1.tar", last modified: Mon Nov  4 20:37:18 2019, max compression
+gzip compressed data, was "passwdgen-0.4.0.tar", last modified: Sat Apr 29 12:10:33 2023, max compression
```

## Comparing `passwdgen-0.3.1.tar` & `passwdgen-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,11 @@
-drwxr-xr-x   0 thane      (501) staff       (20)        0 2019-11-04 20:37:18.000000 passwdgen-0.3.1/
--rw-r--r--   0 thane      (501) staff       (20)     1084 2019-11-04 20:06:55.000000 passwdgen-0.3.1/LICENSE.md
--rw-r--r--   0 thane      (501) staff       (20)       91 2019-11-04 20:33:50.000000 passwdgen-0.3.1/MANIFEST.in
--rw-r--r--   0 thane      (501) staff       (20)    23075 2019-11-04 20:37:18.000000 passwdgen-0.3.1/PKG-INFO
--rw-r--r--   0 thane      (501) staff       (20)    18704 2019-11-04 20:30:06.000000 passwdgen-0.3.1/README.md
-drwxr-xr-x   0 thane      (501) staff       (20)        0 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen/
--rw-r--r--   0 thane      (501) staff       (20)       96 2019-11-04 20:06:55.000000 passwdgen-0.3.1/passwdgen/__init__.py
--rw-r--r--   0 thane      (501) staff       (20)     8703 2019-11-04 20:14:30.000000 passwdgen-0.3.1/passwdgen/cmdline.py
--rw-r--r--   0 thane      (501) staff       (20)     3425 2019-11-04 20:22:19.000000 passwdgen-0.3.1/passwdgen/constants.py
-drwxr-xr-x   0 thane      (501) staff       (20)        0 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen/data/
--rw-r--r--   0 thane      (501) staff       (20)   648933 2019-11-04 20:06:55.000000 passwdgen-0.3.1/passwdgen/data/default-word-list.txt
--rw-r--r--   0 thane      (501) staff       (20)     5852 2019-11-04 20:14:12.000000 passwdgen-0.3.1/passwdgen/generator.py
--rw-r--r--   0 thane      (501) staff       (20)     8055 2019-11-04 20:13:42.000000 passwdgen-0.3.1/passwdgen/utils.py
-drwxr-xr-x   0 thane      (501) staff       (20)        0 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen.egg-info/
--rw-r--r--   0 thane      (501) staff       (20)    23075 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen.egg-info/PKG-INFO
--rw-r--r--   0 thane      (501) staff       (20)      403 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen.egg-info/SOURCES.txt
--rw-r--r--   0 thane      (501) staff       (20)        1 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen.egg-info/dependency_links.txt
--rw-r--r--   0 thane      (501) staff       (20)       54 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen.egg-info/entry_points.txt
--rw-r--r--   0 thane      (501) staff       (20)       17 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen.egg-info/requires.txt
--rw-r--r--   0 thane      (501) staff       (20)       10 2019-11-04 20:37:18.000000 passwdgen-0.3.1/passwdgen.egg-info/top_level.txt
--rw-r--r--   0 thane      (501) staff       (20)       17 2019-11-04 20:10:13.000000 passwdgen-0.3.1/requirements.txt
--rw-r--r--   0 thane      (501) staff       (20)       38 2019-11-04 20:37:18.000000 passwdgen-0.3.1/setup.cfg
--rw-r--r--   0 thane      (501) staff       (20)     1388 2019-11-04 20:32:15.000000 passwdgen-0.3.1/setup.py
+-rw-r--r--   0        0        0     1098 2023-04-29 11:44:23.203274 passwdgen-0.4.0/LICENSE
+-rw-r--r--   0        0        0    18581 2023-04-29 12:00:20.564979 passwdgen-0.4.0/README.md
+-rw-r--r--   0        0        0      118 2023-04-29 11:44:23.203274 passwdgen-0.4.0/passwdgen/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-29 11:44:23.203274 passwdgen-0.4.0/passwdgen/__main__.py
+-rw-r--r--   0        0        0     8717 2023-04-29 11:44:23.203274 passwdgen-0.4.0/passwdgen/cmdline.py
+-rw-r--r--   0        0        0     3478 2023-04-29 11:44:23.203274 passwdgen-0.4.0/passwdgen/constants.py
+-rw-r--r--   0        0        0   648933 2021-08-26 11:21:29.732268 passwdgen-0.4.0/passwdgen/data/default-word-list.txt
+-rw-r--r--   0        0        0     6009 2023-04-29 11:44:23.203274 passwdgen-0.4.0/passwdgen/generator.py
+-rw-r--r--   0        0        0     8190 2023-04-29 11:44:23.203274 passwdgen-0.4.0/passwdgen/utils.py
+-rw-r--r--   0        0        0      896 2023-04-29 11:44:23.203274 passwdgen-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    19312 1970-01-01 00:00:00.000000 passwdgen-0.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `passwdgen-0.3.1/LICENSE.md` & `passwdgen-0.4.0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-# The MIT License (MIT)
+The MIT License (MIT)
 
-Copyright (c) 2016 Thane Thomson
+Copyright (c) 2016- Thane Thomson and contributors
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `passwdgen-0.3.1/PKG-INFO` & `passwdgen-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,478 +1,456 @@
-Metadata-Version: 2.1
-Name: passwdgen
-Version: 0.3.1
-Summary: A password generation utility
-Home-page: https://github.com/thanethomson/passwdgen
-Author: Thane Thomson
-Author-email: connect@thanethomson.com
-License: UNKNOWN
-Description: # passwdgen
-        
-        [![Build Status](https://travis-ci.org/thanethomson/passwdgen.svg?branch=master)](https://travis-ci.org/thanethomson/passwdgen)
-        [![PyPI](https://img.shields.io/pypi/v/passwdgen.svg)](https://pypi.python.org/pypi/passwdgen)
-        [![PyPI](https://img.shields.io/pypi/pyversions/passwdgen.svg)](https://pypi.python.org/pypi/passwdgen)
-        
-        ## Overview
-        `passwdgen` is a simple password generation utility with a couple of
-        powerful extra features (including password entropy calculation and
-        entropy-based password generation).
-        
-        
-        ## Installation
-        To use `passwdgen`, you will need to install Python 3.6+.
-        
-        ```bash
-        > pip install passwdgen
-        ```
-        
-        If you want `passwdgen` to be globally accessible, you'll need to
-        install it with `sudo`/`root` privileges:
-        
-        ```bash
-        > sudo pip install passwdgen
-        ```
-        
-        
-        ## Usage
-        The simplest password generation command you can execute is:
-        
-        ```bash
-        > passwdgen generate
-        totems-representing-sachem-tarrier
-        ```
-        
-        ## Commands
-        To find out more detailed help about a particular command, simply
-        run:
-        
-        ```bash
-        > passwdgen <command> --help
-        
-        # For example:
-        > passwdgen generate --help
-        ```
-        
-        ### `info`
-        Allows you to calculate the entropy of a particular password. For
-        example, on UNIX-like systems, you can simply pipe the password into
-        the info command:
-        
-        ```bash
-        > echo "some-password" | passwdgen info
-        > cat /path/to/password/file | passwdgen info
-        ```
-        
-        If you do not pipe text into `passwdgen`, it will prompt you to enter
-        the password on the command line:
-        
-        ```bash
-        > passwdgen info
-        Please enter the password to check: <type your password here>
-        ```
-        
-        For more information on password entropy, please see the section
-        on **Entropy** further on in this README.
-        
-        ### `generate`
-        Generate a password. Two kinds of passwords can be generated:
-        
-        * dictionary-based passwords (the default), or
-        * character-based passwords (see this [XKCD](http://xkcd.com/936/)
-          before you choose this mechanism).
-        
-        Some examples of **dictionary-based** password generation:
-        
-        ```bash
-        # Generate a dictionary-based password 6 words long
-        > passwdgen generate -l 6
-        
-        # Generate a dictionary-based password with minimum entropy 70 bits
-        > passwdgen generate -m 70
-        
-        # Generate a dictionary-based password and copy it to the clipboard
-        > passwdgen generate -c
-        
-        # Generate a dictionary-based password with colons (:) as a separator
-        > passwdgen generate -s colon
-        
-        # Generate a dictionary-based password and display its entropy info
-        > passwdgen generate -i
-        
-        # Generate a dictionary-based password based on the given starting letters
-        > passwdgen generate --starting-letters hello
-        ```
-        
-        Some examples of **character-based** password generation:
-        
-        ```bash
-        # Generate a password 15 characters long comprising numbers and letters
-        > passwdgen generate -t alpha-numeric -l 15
-        
-        # Generate a password 18 characters long comprising numbers, letters and
-        # special characters
-        > passwdgen generate -t special -l 18
-        
-        # Generate a password 12 characters long and display its entropy info
-        > passwdgen generate -t special -l 12 -i
-        
-        # Generate a character-based password, copy it to the clipboard, and
-        # display its entropy info
-        > passwdgen generate -t special -c -i
-        ```
-        
-        ### `rng`
-        Runs a quick test of your OS' pseudorandom number generator (PRNG).
-        Computes a sample set (by default, 1 million entries) of random
-        numbers between 0 and 100 (inclusive)
-        
-        For example:
-        
-        ```bash
-        > passwdgen rng
-        Testing OS RNG. Attempting to generate 1000000 samples between 0 and 100 (inclusive). Please wait...
-        
-        Statistics
-        ----------
-        Mean               : 49.966455 (should approach 50.000 as the sample size increases; 0.067% difference)
-        Standard deviation : 29.151161 (should be as close to 29.154759 as possible; 0.012% difference)
-        Time taken         : 2.083 seconds
-        
-        ```
-        
-        The expected standard deviation for a random variable with a discrete
-        uniform random distribution is expected to be calculated as per
-        [this Wikipedia entry](https://en.wikipedia.org/wiki/Discrete_uniform_distribution).
-        
-        ### `wordlist`
-        At present, this command has only one sub-command: `clean`. To take
-        an arbitrary word list (a text file with one word per line) and
-        clean it up, do the following:
-        
-        ```bash
-        > passwdgen wordlist clean /path/to/input/file.txt /path/to/output/file.txt
-        ```
-        
-        This command will:
-        
-        * remove empty lines,
-        * strip out any plurals (`'s` at the end of strings),
-        * convert all words to lowercase,
-        * deduplicate entries, and
-        * sort everything alphabetically.
-        
-        
-        ## API
-        Using `passwdgen` from your own Python project is easy:
-        
-        ```python
-        import passwdgen
-        
-        # Generate a dictionary-based password using the built-in dictionary
-        my_password = passwdgen.words()
-        
-        # Generate a character-based password
-        my_password = passwdgen.chars()
-        
-        # Generate a dictionary-based password with 6 words
-        long_password = passwdgen.words(word_count=6)
-        
-        # Generate a dictionary-based password with minimum entropy 80
-        difficult_password = passwdgen.words(min_entropy=80)
-        
-        # Generate a dictionary-based password with a custom dictionary
-        my_dictionary = passwdgen.load_word_list("/path/to/my/dict.txt")
-        password = passwdgen.words(my_dictionary)
-        ```
-        
-        ### `passwdgen.words(dict_set, separator, word_count, min_entropy, starting_letters)`
-        Generates a dictionary-based password. All arguments are keyword
-        arguments and are optional:
-        
-        * `dict_set`: A `set` containing all of the possible words from which to
-          generate a password. If not supplied, this will default to the
-          built-in dictionary.
-        * `separator`: The separator character to use between the words.
-          Default value: `-` (hyphen)
-        * `word_count`: The number of words to use when generating the password.
-          If not specified, and `min_entropy` is not specified, this defaults
-          to `4`.
-        * `min_entropy`: The minimum required entropy of the generated
-          password. If `word_count` is specified, this parameter is ignored.
-        * `starting_letters`: A string containing the desired starting letters
-          of each word in the generated password. Note: if `word_count` or
-          `min_entropy` are specified, this string must contain at least
-          the relevant number of characters to match the number of generated
-          words. Otherwise the generated password will have exactly the same
-          number of words as this string has characters.
-        
-        Returns a string.
-        
-        ### `passwdgen.chars(charset, length, min_entropy)`
-        Generates a character-based password. All arguments are keyword
-        arguments and are optional:
-        
-        * `charset`: The ID of the character set from which to source characters
-          for the generated password. Default: `special`. See the
-          section on **Character Sets** below.
-        * `length`: The required number of characters in the generated password.
-          If neither `length` nor `min_entropy` are specified, this defaults
-          to `12`.
-        * `min_entropy`: The minimum required entropy of the generated
-          password. If `length` is specified, this parameter is ignored.
-        
-        Returns a string.
-        
-        ### `passwdgen.load_word_list(filename, encoding)`
-        Loads a word list into memory. All arguments are keyword arguments
-        and are optional:
-        
-        * `filename`: The path to the file from which to load the words. This
-          file must be a plain text file containing one word per line. If
-          not specified, this loads the built-in dictionary into memory.
-        * `encoding`: The character encoding to use when reading the file.
-        
-        Returns a `set` containing the loaded words.
-        
-        ### `passwdgen.secure_random(a, b)`
-        Securely generates a random number using the given limits.
-        
-        * `a` (required): If `b` is specified, `a` represents the lower limit
-          (inclusive) of the resulting random number. If `b` is not specified,
-          `a` represents the upper limit (exclusive) of the generated number,
-          and the lower limit defaults to `0`.
-        * `b` (optional): The upper limit (exclusive) of the generated random
-          number.
-        
-        Returns a securely generated random number with `a <= result < b` if
-        `b` is specified, or `0 <= result < a` if `b` is not specified.
-        
-        ### `passwdgen.calculate_entropy(password, dict_set)`
-        Attempts to calculate the entropy of the given password based on
-        the preconfigured character sets and the dictionary.
-        
-        * `password` (required): The password whose entropy is to be calculated.
-        * `dict_set` (optional): A `set` of words comprising the dictionary
-          for which to perform the dictionary-based entropy calculation.
-        
-        Returns a `dict` whose keys represent the IDs of the different character
-        sets tested, and values represent the corresponding entropies.
-        
-        
-        ## Character Sets
-        The following character sets are available at present (for use with the
-        `generate --charset <charset>` command).
-        
-        * `dict`: Dictionary-based password generation.
-        * `alpha-lower`: Lowercase alphabetical letters (`a-z`).
-        * `alpha-upper`: Uppercase alphabetical letters (`A-Z`).
-        * `alpha`: Alphabetical (`a-z`, `A-Z`).
-        * `alpha-numeric`: Alphanumeric characters (`a-z`, `A-Z`, `0-9`).
-        * `alpha-numeric-spaced`: Alphanumeric characters and spaces (`a-z`,
-          `A-Z`, `0-9`, ` `).
-        * `numeric`: Numeric characters (`0-9`).
-        * `alpha-lower-sep`: Lowercase alphabetical letters and separators
-          (`a-z`, `-_. ,;:`).
-        * `alpha-upper-sep`: Uppercase alphabetical letters and separators
-          (`A-Z`, `-_. ,;:`).
-        * `special`: Alphanumeric characters and special characters
-          (`a-z`, `A-Z`, `0-9`, ``-_. ,;:!@#$%^&*()+={}[]'\"\\/?<>`~``).
-        
-        
-        ## Entropy
-        Entropy, in the context of information theory, provides a convenient
-        way to quantify the amount of information in a particular set of
-        data. With regard to password strength, the higher the entropy of
-        a password, the more difficult it is for an attacker to guess.
-        
-        From the perspective of the generator, the password strength is measured
-        by way of the information source. From the perspective of an attacker,
-        the more information is known about the information source that
-        generated the password (e.g. the kind of random number generator used,
-        the character set to which the password belongs), the lower the entropy
-        of that password.
-        
-        ### Secure random number generation
-        Entropy calculations are based on the assumption that the random number
-        source is of *good quality* (see [CSPRNG](https://en.wikipedia.org/wiki/Cryptographically_secure_pseudorandom_number_generator))
-        and generates [uniformly distributed](https://en.wikipedia.org/wiki/Discrete_uniform_distribution)
-        random numbers. The random number generator (RNG) used in `passwd`
-        is provided by the `os.urandom()` function, which uses `/dev/urandom`
-        on POSIX systems and `CryptGenRandom()` on Windows systems.
-        
-        ### Character-based calculation
-        This password generator uses the following definition for entropy: a
-        single character `c` from a character set of size `n` characters has
-        an entropy of `log2(n)` bits (per character). Entropy adds up as the
-        length of the password increases, i.e. two characters from the character
-        set of size `n` will have a combined overall entropy of `2 x log2(n)`.
-        
-        For example, if the lowercase alphabet `a..z` is used as the character
-        set, it has `n=26`. Each character would have an entropy of
-        `log2(26) = 4.700439718141093` bits per character. A password string,
-        therefore, such as `mysuperweakpassword` of length 19 characters, will
-        have a total entropy of `19 x log2(26) = 89.31` bits.
-        
-        As the size of the character set increases, so does the entropy of the
-        password of a certain length, as an attacker attempting a brute force
-        attack would have to search a much larger set of possibilities to
-        find the password.
-        
-        ### Dictionary-based calculation
-        The dictionary-based method of entropy calculation assumes that an
-        attacker has prior knowledge that the password was generated using a
-        dictionary of words, and even knows which dictionary was used. This
-        would obviously be the case if you personally used `passwdgen` to
-        generate a dictionary-based password, as all the code and the dictionary
-        are out in the open.
-        
-        In this case, instead of assuming a character set (which would mean
-        a far higher entropy in passwords with 2 or more words), a
-        dictionary-based attack could be performed much quicker.
-        
-        For example, the password `dog-far-nightly-can` is 19 characters long
-        and makes use of the lowercase alphabet and hyphens (resulting in a
-        character set of 27 possible characters). This means that a
-        brute force attacker using the full lowercase alphabet and hyphens
-        would be faced with a potential password entropy of
-        `19 x log2(27) = 90.34` bits.
-        
-        If, however, the attacker knows that the password is dictionary-based
-        and that the words are separated by hyphens, the attacker would only
-        have to guess the 4 words from the dictionary making up the password.
-        This results in a potential entropy from the perspective of the
-        attacker of `4 x log2(275,185) = 72.28` bits (assuming dictionary
-        size of 275,185 words). This is still a pretty strong password, but
-        it is still easier to crack than a password where the attacker does not
-        know that it is dictionary-based.
-        
-        ### How much entropy is enough?
-        So how does one select an appropriate entropy for trying to prevent
-        brute force attacks? This is difficult to estimate, because it depends
-        entirely on the resources available to an attacker. Usually it's cheaper
-        and easier to perform social engineering attacks if someone wants to
-        obtain your password, but if you're paranoid about security and want to
-        cover all your bases, you have to think about the kinds of computing
-        power available to attackers.
-        
-        Assuming that whichever service stores your password does not store the
-        clear password itself, but a [SHA-256](https://en.wikipedia.org/wiki/SHA-2)
-        hash of the password (common practice today), and an attacker manages
-        to get hold of this SHA-256 hash, they will have to try many possible
-        permutations of input passwords that will eventually match to that
-        SHA-256 hash.
-        
-        In general, [GPU-based hash attacks are much faster](https://blog.codinghorror.com/speed-hashing/)
-        than CPU-based hash attacks. At the time of this writing, it would seem
-        as though high-end GPUs have the ability to perform around 1,000
-        megahashes per second (that's 1,000,000,000 hashes per second, or
-        `10^9` hashes per second).
-        
-        Let's assume you generate a dictionary-based password, where the
-        source dictionary size is **71,188** words. Let's also assume that the
-        attacker has the same source dictionary, and knows which character you
-        use to separate the words in your password (in this case, a hyphen).
-        
-        | Words | Permutations                      | Time to Crack    | Entropy    |
-        | ----- | --------------------------------- | ---------------- | ---------- |
-        | 2     | 5,067,660,156                     | 5.07 seconds     | 32.24 bits |
-        | 3     | 360,746,455,865,016               | 4.175 days       | 48.36 bits |
-        | 4     | 25,679,736,460,751,163,960        | 814 years        | 64.47 bits |
-        | 5     | 1,827,986,360,222,110,855,328,640 | 57,965,067 years | 80.6 bits  |
-        
-        Of course, if an attacker splits the work up evenly across multiple
-        GPUs, the time to crack goes down linearly, so a 4-word password being
-        brute-force cracked by 2 GPUs would take 407 years, 3 GPUs would take
-        203.5 years, 10 GPUs 81.4 years, 100 GPUs 8.1 years, 1,000 GPUs
-        would take about 9.5 months, and 10,000 GPUs would take 29.7 days.
-        
-        So, as you see, it really depends on the resources available to an
-        attacker. In general though, right now, a password with entropy
-        80 bits and upwards, from the perspective of an attacker, is pretty
-        much infeasible to crack (so a 5-word password from a significantly
-        sized source dictionary and a good quality PRNG). This will, of course,
-        possibly change in the age of quantum computers.
-        
-        
-        ## Dictionary
-        The included dictionary is a "cleaned out" (see the `wordlist clean`
-        command provided by `passwdgen`) version of a dictionary created
-        through [SCOWL (And Friends)](http://wordlist.aspell.net/), using their
-        [word list generator](http://app.aspell.net/create).
-        
-        At present, the embedded dictionary contains **71,188** words, ensuring
-        an entropy of `log2(71,188) = 16.119` bits per word.
-        
-        ### Legal
-        Copyright 2000-2014 by Kevin Atkinson
-        
-        > Permission to use, copy, modify, distribute and sell these word
-        > lists, the associated scripts, the output created from the scripts,
-        > and its documentation for any purpose is hereby granted without fee,
-        > provided that the above copyright notice appears in all copies and
-        > that both that copyright notice and this permission notice appear in
-        > supporting documentation. Kevin Atkinson makes no representations
-        > about the suitability of this array for any purpose. It is provided
-        > "as is" without express or implied warranty.
-        
-        Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
-        
-        > The following restriction is placed on the use of this publication:
-        > if The UK Advanced Cryptics Dictionary is used in a software package
-        > or redistributed in any form, the copyright notice must be
-        > prominently displayed and the text of this document must be included
-        > verbatim.
-        >
-        > There are no other restrictions: I would like to see the list
-        > distributed as widely as possible.
-        
-        Many sources were used in the creation of SCOWL, most of them were in
-        the public domain or used indirectly.  For a full list please see the
-        SCOWL readme.
-        
-        [http://wordlist.aspell.net/](http://wordlist.aspell.net/)
-        
-        
-        ## References
-        The following sources were consulted in building the password generator:
-        
-        * [Entropy (information theory) ~ Wikipedia](https://en.wikipedia.org/wiki/Entropy_(information_theory))
-        * [How should I calculate the entropy of a password? ~ Cryptography StackExchange](http://crypto.stackexchange.com/questions/374/how-should-i-calculate-the-entropy-of-a-password)
-        * [How to calculate password entropy](https://ritcyberselfdefense.wordpress.com/2011/09/24/how-to-calculate-password-entropy/)
-        * [Permutation ~ Wikipedia](https://en.wikipedia.org/wiki/Permutation)
-        
-        
-        ## License
-        **The MIT License (MIT)**
-        
-        Copyright (c) 2016 Thane Thomson
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of
-        this software and associated documentation files (the "Software"), to deal in
-        the Software without restriction, including without limitation the rights to
-        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-        of the Software, and to permit persons to whom the Software is furnished to do
-        so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
+# passwdgen
+
+[![PyPI](https://img.shields.io/pypi/v/passwdgen.svg)](https://pypi.python.org/pypi/passwdgen)
+[![PyPI](https://img.shields.io/pypi/pyversions/passwdgen.svg)](https://pypi.python.org/pypi/passwdgen)
+
+## Overview
+`passwdgen` is a simple password generation utility with a couple of
+powerful extra features (including password entropy calculation and
+entropy-based password generation).
+
+
+## Installation
+To use `passwdgen`, you will need to install Python 3.9+.
+
+```bash
+> pip install passwdgen
+```
+
+If you want `passwdgen` to be globally accessible, you'll need to
+install it with `sudo`/`root` privileges:
+
+```bash
+> sudo pip install passwdgen
+```
+
+
+## Usage
+The simplest password generation command you can execute is:
+
+```bash
+> passwdgen generate
+totems-representing-sachem-tarrier
+```
+
+## Commands
+To find out more detailed help about a particular command, simply
+run:
+
+```bash
+> passwdgen <command> --help
+
+# For example:
+> passwdgen generate --help
+```
+
+### `info`
+Allows you to calculate the entropy of a particular password. For
+example, on UNIX-like systems, you can simply pipe the password into
+the info command:
+
+```bash
+> echo "some-password" | passwdgen info
+> cat /path/to/password/file | passwdgen info
+```
+
+If you do not pipe text into `passwdgen`, it will prompt you to enter
+the password on the command line:
+
+```bash
+> passwdgen info
+Please enter the password to check: <type your password here>
+```
+
+For more information on password entropy, please see the section
+on **Entropy** further on in this README.
+
+### `generate`
+Generate a password. Two kinds of passwords can be generated:
+
+* dictionary-based passwords (the default), or
+* character-based passwords (see this [XKCD](http://xkcd.com/936/)
+  before you choose this mechanism).
+
+Some examples of **dictionary-based** password generation:
+
+```bash
+# Generate a dictionary-based password 6 words long
+> passwdgen generate -l 6
+
+# Generate a dictionary-based password with minimum entropy 70 bits
+> passwdgen generate -m 70
+
+# Generate a dictionary-based password and copy it to the clipboard
+> passwdgen generate -c
+
+# Generate a dictionary-based password with colons (:) as a separator
+> passwdgen generate -s colon
+
+# Generate a dictionary-based password and display its entropy info
+> passwdgen generate -i
+
+# Generate a dictionary-based password based on the given starting letters
+> passwdgen generate --starting-letters hello
+```
+
+Some examples of **character-based** password generation:
+
+```bash
+# Generate a password 15 characters long comprising numbers and letters
+> passwdgen generate -t alpha-numeric -l 15
+
+# Generate a password 18 characters long comprising numbers, letters and
+# special characters
+> passwdgen generate -t special -l 18
+
+# Generate a password 12 characters long and display its entropy info
+> passwdgen generate -t special -l 12 -i
+
+# Generate a character-based password, copy it to the clipboard, and
+# display its entropy info
+> passwdgen generate -t special -c -i
+```
+
+### `rng`
+Runs a quick test of your OS' pseudorandom number generator (PRNG).
+Computes a sample set (by default, 1 million entries) of random
+numbers between 0 and 100 (inclusive)
+
+For example:
+
+```bash
+> passwdgen rng
+Testing OS RNG. Attempting to generate 1000000 samples between 0 and 100 (inclusive). Please wait...
+
+Statistics
+----------
+Mean               : 49.966455 (should approach 50.000 as the sample size increases; 0.067% difference)
+Standard deviation : 29.151161 (should be as close to 29.154759 as possible; 0.012% difference)
+Time taken         : 2.083 seconds
+
+```
+
+The expected standard deviation for a random variable with a discrete
+uniform random distribution is expected to be calculated as per
+[this Wikipedia entry](https://en.wikipedia.org/wiki/Discrete_uniform_distribution).
+
+### `wordlist`
+At present, this command has only one sub-command: `clean`. To take
+an arbitrary word list (a text file with one word per line) and
+clean it up, do the following:
+
+```bash
+> passwdgen wordlist clean /path/to/input/file.txt /path/to/output/file.txt
+```
+
+This command will:
+
+* remove empty lines,
+* strip out any plurals (`'s` at the end of strings),
+* convert all words to lowercase,
+* deduplicate entries, and
+* sort everything alphabetically.
+
+
+## API
+Using `passwdgen` from your own Python project is easy:
+
+```python
+import passwdgen
+
+# Generate a dictionary-based password using the built-in dictionary
+my_password = passwdgen.words()
+
+# Generate a character-based password
+my_password = passwdgen.chars()
+
+# Generate a dictionary-based password with 6 words
+long_password = passwdgen.words(word_count=6)
+
+# Generate a dictionary-based password with minimum entropy 80
+difficult_password = passwdgen.words(min_entropy=80)
+
+# Generate a dictionary-based password with a custom dictionary
+my_dictionary = passwdgen.load_word_list("/path/to/my/dict.txt")
+password = passwdgen.words(my_dictionary)
+```
+
+### `passwdgen.words(dict_set, separator, word_count, min_entropy, starting_letters)`
+Generates a dictionary-based password. All arguments are keyword
+arguments and are optional:
+
+* `dict_set`: A `set` containing all of the possible words from which to
+  generate a password. If not supplied, this will default to the
+  built-in dictionary.
+* `separator`: The separator character to use between the words.
+  Default value: `-` (hyphen)
+* `word_count`: The number of words to use when generating the password.
+  If not specified, and `min_entropy` is not specified, this defaults
+  to `4`.
+* `min_entropy`: The minimum required entropy of the generated
+  password. If `word_count` is specified, this parameter is ignored.
+* `starting_letters`: A string containing the desired starting letters
+  of each word in the generated password. Note: if `word_count` or
+  `min_entropy` are specified, this string must contain at least
+  the relevant number of characters to match the number of generated
+  words. Otherwise the generated password will have exactly the same
+  number of words as this string has characters.
+
+Returns a string.
+
+### `passwdgen.chars(charset, length, min_entropy)`
+Generates a character-based password. All arguments are keyword
+arguments and are optional:
+
+* `charset`: The ID of the character set from which to source characters
+  for the generated password. Default: `special`. See the
+  section on **Character Sets** below.
+* `length`: The required number of characters in the generated password.
+  If neither `length` nor `min_entropy` are specified, this defaults
+  to `12`.
+* `min_entropy`: The minimum required entropy of the generated
+  password. If `length` is specified, this parameter is ignored.
+
+Returns a string.
+
+### `passwdgen.load_word_list(filename, encoding)`
+Loads a word list into memory. All arguments are keyword arguments
+and are optional:
+
+* `filename`: The path to the file from which to load the words. This
+  file must be a plain text file containing one word per line. If
+  not specified, this loads the built-in dictionary into memory.
+* `encoding`: The character encoding to use when reading the file.
+
+Returns a `set` containing the loaded words.
+
+### `passwdgen.secure_random(a, b)`
+Securely generates a random number using the given limits.
+
+* `a` (required): If `b` is specified, `a` represents the lower limit
+  (inclusive) of the resulting random number. If `b` is not specified,
+  `a` represents the upper limit (exclusive) of the generated number,
+  and the lower limit defaults to `0`.
+* `b` (optional): The upper limit (exclusive) of the generated random
+  number.
+
+Returns a securely generated random number with `a <= result < b` if
+`b` is specified, or `0 <= result < a` if `b` is not specified.
+
+### `passwdgen.calculate_entropy(password, dict_set)`
+Attempts to calculate the entropy of the given password based on
+the preconfigured character sets and the dictionary.
+
+* `password` (required): The password whose entropy is to be calculated.
+* `dict_set` (optional): A `set` of words comprising the dictionary
+  for which to perform the dictionary-based entropy calculation.
+
+Returns a `dict` whose keys represent the IDs of the different character
+sets tested, and values represent the corresponding entropies.
+
+
+## Character Sets
+The following character sets are available at present (for use with the
+`generate --charset <charset>` command).
+
+* `dict`: Dictionary-based password generation.
+* `alpha-lower`: Lowercase alphabetical letters (`a-z`).
+* `alpha-upper`: Uppercase alphabetical letters (`A-Z`).
+* `alpha`: Alphabetical (`a-z`, `A-Z`).
+* `alpha-numeric`: Alphanumeric characters (`a-z`, `A-Z`, `0-9`).
+* `alpha-numeric-spaced`: Alphanumeric characters and spaces (`a-z`,
+  `A-Z`, `0-9`, ` `).
+* `numeric`: Numeric characters (`0-9`).
+* `alpha-lower-sep`: Lowercase alphabetical letters and separators
+  (`a-z`, `-_. ,;:`).
+* `alpha-upper-sep`: Uppercase alphabetical letters and separators
+  (`A-Z`, `-_. ,;:`).
+* `special`: Alphanumeric characters and special characters
+  (`a-z`, `A-Z`, `0-9`, ``-_. ,;:!@#$%^&*()+={}[]'\"\\/?<>`~``).
+
+
+## Entropy
+Entropy, in the context of information theory, provides a convenient
+way to quantify the amount of information in a particular set of
+data. With regard to password strength, the higher the entropy of
+a password, the more difficult it is for an attacker to guess.
+
+From the perspective of the generator, the password strength is measured
+by way of the information source. From the perspective of an attacker,
+the more information is known about the information source that
+generated the password (e.g. the kind of random number generator used,
+the character set to which the password belongs), the lower the entropy
+of that password.
+
+### Secure random number generation
+Entropy calculations are based on the assumption that the random number
+source is of *good quality* (see [CSPRNG](https://en.wikipedia.org/wiki/Cryptographically_secure_pseudorandom_number_generator))
+and generates [uniformly distributed](https://en.wikipedia.org/wiki/Discrete_uniform_distribution)
+random numbers. The random number generator (RNG) used in `passwd`
+is provided by the `os.urandom()` function, which uses `/dev/urandom`
+on POSIX systems and `CryptGenRandom()` on Windows systems.
+
+### Character-based calculation
+This password generator uses the following definition for entropy: a
+single character `c` from a character set of size `n` characters has
+an entropy of `log2(n)` bits (per character). Entropy adds up as the
+length of the password increases, i.e. two characters from the character
+set of size `n` will have a combined overall entropy of `2 x log2(n)`.
+
+For example, if the lowercase alphabet `a..z` is used as the character
+set, it has `n=26`. Each character would have an entropy of
+`log2(26) = 4.700439718141093` bits per character. A password string,
+therefore, such as `mysuperweakpassword` of length 19 characters, will
+have a total entropy of `19 x log2(26) = 89.31` bits.
+
+As the size of the character set increases, so does the entropy of the
+password of a certain length, as an attacker attempting a brute force
+attack would have to search a much larger set of possibilities to
+find the password.
+
+### Dictionary-based calculation
+The dictionary-based method of entropy calculation assumes that an
+attacker has prior knowledge that the password was generated using a
+dictionary of words, and even knows which dictionary was used. This
+would obviously be the case if you personally used `passwdgen` to
+generate a dictionary-based password, as all the code and the dictionary
+are out in the open.
+
+In this case, instead of assuming a character set (which would mean
+a far higher entropy in passwords with 2 or more words), a
+dictionary-based attack could be performed much quicker.
+
+For example, the password `dog-far-nightly-can` is 19 characters long
+and makes use of the lowercase alphabet and hyphens (resulting in a
+character set of 27 possible characters). This means that a
+brute force attacker using the full lowercase alphabet and hyphens
+would be faced with a potential password entropy of
+`19 x log2(27) = 90.34` bits.
+
+If, however, the attacker knows that the password is dictionary-based
+and that the words are separated by hyphens, the attacker would only
+have to guess the 4 words from the dictionary making up the password.
+This results in a potential entropy from the perspective of the
+attacker of `4 x log2(275,185) = 72.28` bits (assuming dictionary
+size of 275,185 words). This is still a pretty strong password, but
+it is still easier to crack than a password where the attacker does not
+know that it is dictionary-based.
+
+### How much entropy is enough?
+So how does one select an appropriate entropy for trying to prevent
+brute force attacks? This is difficult to estimate, because it depends
+entirely on the resources available to an attacker. Usually it's cheaper
+and easier to perform social engineering attacks if someone wants to
+obtain your password, but if you're paranoid about security and want to
+cover all your bases, you have to think about the kinds of computing
+power available to attackers.
+
+Assuming that whichever service stores your password does not store the
+clear password itself, but a [SHA-256](https://en.wikipedia.org/wiki/SHA-2)
+hash of the password (common practice today), and an attacker manages
+to get hold of this SHA-256 hash, they will have to try many possible
+permutations of input passwords that will eventually match to that
+SHA-256 hash.
+
+In general, [GPU-based hash attacks are much faster](https://blog.codinghorror.com/speed-hashing/)
+than CPU-based hash attacks. At the time of this writing, it would seem
+as though high-end GPUs have the ability to perform around 1,000
+megahashes per second (that's 1,000,000,000 hashes per second, or
+`10^9` hashes per second).
+
+Let's assume you generate a dictionary-based password, where the
+source dictionary size is **71,188** words. Let's also assume that the
+attacker has the same source dictionary, and knows which character you
+use to separate the words in your password (in this case, a hyphen).
+
+| Words | Permutations                      | Time to Crack    | Entropy    |
+|-------|-----------------------------------|------------------|------------|
+| 2     | 5,067,660,156                     | 5.07 seconds     | 32.24 bits |
+| 3     | 360,746,455,865,016               | 4.175 days       | 48.36 bits |
+| 4     | 25,679,736,460,751,163,960        | 814 years        | 64.47 bits |
+| 5     | 1,827,986,360,222,110,855,328,640 | 57,965,067 years | 80.6 bits  |
+
+Of course, if an attacker splits the work up evenly across multiple
+GPUs, the time to crack goes down linearly, so a 4-word password being
+brute-force cracked by 2 GPUs would take 407 years, 3 GPUs would take
+203.5 years, 10 GPUs 81.4 years, 100 GPUs 8.1 years, 1,000 GPUs
+would take about 9.5 months, and 10,000 GPUs would take 29.7 days.
+
+So, as you see, it really depends on the resources available to an
+attacker. In general though, right now, a password with entropy
+80 bits and upwards, from the perspective of an attacker, is pretty
+much infeasible to crack (so a 5-word password from a significantly
+sized source dictionary and a good quality PRNG). This will, of course,
+possibly change in the age of quantum computers.
+
+
+## Dictionary
+The included dictionary is a "cleaned out" (see the `wordlist clean`
+command provided by `passwdgen`) version of a dictionary created
+through [SCOWL (And Friends)](http://wordlist.aspell.net/), using their
+[word list generator](http://app.aspell.net/create).
+
+At present, the embedded dictionary contains **71,188** words, ensuring
+an entropy of `log2(71,188) = 16.119` bits per word.
+
+### Legal
+Copyright 2000-2014 by Kevin Atkinson
+
+> Permission to use, copy, modify, distribute and sell these word
+> lists, the associated scripts, the output created from the scripts,
+> and its documentation for any purpose is hereby granted without fee,
+> provided that the above copyright notice appears in all copies and
+> that both that copyright notice and this permission notice appear in
+> supporting documentation. Kevin Atkinson makes no representations
+> about the suitability of this array for any purpose. It is provided
+> "as is" without express or implied warranty.
+
+Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
+
+> The following restriction is placed on the use of this publication:
+> if The UK Advanced Cryptics Dictionary is used in a software package
+> or redistributed in any form, the copyright notice must be
+> prominently displayed and the text of this document must be included
+> verbatim.
+>
+> There are no other restrictions: I would like to see the list
+> distributed as widely as possible.
+
+Many sources were used in the creation of SCOWL, most of them were in
+the public domain or used indirectly.  For a full list please see the
+SCOWL readme.
+
+[http://wordlist.aspell.net/](http://wordlist.aspell.net/)
+
+
+## References
+The following sources were consulted in building the password generator:
+
+* [Entropy (information theory) ~ Wikipedia](https://en.wikipedia.org/wiki/Entropy_(information_theory))
+* [How should I calculate the entropy of a password? ~ Cryptography StackExchange](http://crypto.stackexchange.com/questions/374/how-should-i-calculate-the-entropy-of-a-password)
+* [How to calculate password entropy](https://ritcyberselfdefense.wordpress.com/2011/09/24/how-to-calculate-password-entropy/)
+* [Permutation ~ Wikipedia](https://en.wikipedia.org/wiki/Permutation)
+
+
+## License
+**The MIT License (MIT)**
+
+Copyright (c) 2016-2019 Thane Thomson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `passwdgen-0.3.1/README.md` & `passwdgen-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,40 @@
+Metadata-Version: 2.1
+Name: passwdgen
+Version: 0.4.0
+Summary: A password generation utility
+Author-email: Thane Thomson <connect@thanethomson.com>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Utilities
+Requires-Dist: pyperclip >= 1.8.2
+Project-URL: Homepage, https://github.com/thanethomson/passwdgen
+
 # passwdgen
 
-[![Build Status](https://travis-ci.org/thanethomson/passwdgen.svg?branch=master)](https://travis-ci.org/thanethomson/passwdgen)
 [![PyPI](https://img.shields.io/pypi/v/passwdgen.svg)](https://pypi.python.org/pypi/passwdgen)
 [![PyPI](https://img.shields.io/pypi/pyversions/passwdgen.svg)](https://pypi.python.org/pypi/passwdgen)
 
 ## Overview
 `passwdgen` is a simple password generation utility with a couple of
 powerful extra features (including password entropy calculation and
 entropy-based password generation).
 
 
 ## Installation
-To use `passwdgen`, you will need to install Python 3.6+.
+To use `passwdgen`, you will need to install Python 3.9+.
 
 ```bash
 > pip install passwdgen
 ```
 
 If you want `passwdgen` to be globally accessible, you'll need to
 install it with `sudo`/`root` privileges:
@@ -361,15 +380,15 @@
 
 Let's assume you generate a dictionary-based password, where the
 source dictionary size is **71,188** words. Let's also assume that the
 attacker has the same source dictionary, and knows which character you
 use to separate the words in your password (in this case, a hyphen).
 
 | Words | Permutations                      | Time to Crack    | Entropy    |
-| ----- | --------------------------------- | ---------------- | ---------- |
+|-------|-----------------------------------|------------------|------------|
 | 2     | 5,067,660,156                     | 5.07 seconds     | 32.24 bits |
 | 3     | 360,746,455,865,016               | 4.175 days       | 48.36 bits |
 | 4     | 25,679,736,460,751,163,960        | 814 years        | 64.47 bits |
 | 5     | 1,827,986,360,222,110,855,328,640 | 57,965,067 years | 80.6 bits  |
 
 Of course, if an attacker splits the work up evenly across multiple
 GPUs, the time to crack goes down linearly, so a 4-word password being
@@ -432,15 +451,15 @@
 * [How to calculate password entropy](https://ritcyberselfdefense.wordpress.com/2011/09/24/how-to-calculate-password-entropy/)
 * [Permutation ~ Wikipedia](https://en.wikipedia.org/wiki/Permutation)
 
 
 ## License
 **The MIT License (MIT)**
 
-Copyright (c) 2016 Thane Thomson
+Copyright (c) 2016-2019 Thane Thomson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
@@ -451,7 +470,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `passwdgen-0.3.1/passwdgen/cmdline.py` & `passwdgen-0.4.0/passwdgen/cmdline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,177 +1,189 @@
 # -*- coding: utf-8 -*-
 
 import sys
 from getpass import getpass
 import argparse
-import pkg_resources
 import pyperclip
 
 from .generator import *
 from .utils import *
 from .constants import *
+from . import __version__
 
 
 def show_password_entropy(passwd, word_list):
     """Displays the password entropy calculation results."""
     entropy = calculate_entropy(passwd, dict_set=word_list)
     print("\nPassword length: %d characters" % len(passwd))
     print("\nEntropy")
     print("-------")
     for charset, charset_name in list(PASSWORD_CHARSET_NAMES):
-        print(("{:<%d}" % LONGEST_CHARSET_NAME_LEN).format(charset_name) + " : " +
-              (("%.6f" % entropy[charset]) if charset in entropy else "not in character set"))
+        print(
+            ("{:<%d}" % LONGEST_CHARSET_NAME_LEN).format(charset_name)
+            + " : "
+            + (
+                ("%.6f" % entropy[charset])
+                if charset in entropy
+                else "not in character set"
+            )
+        )
     print("")
 
 
 def main():
     """Main routine for handling command line functionality for passwdgen."""
 
-    version = pkg_resources.require("passwdgen")[0].version
-    parser = argparse.ArgumentParser(description="A password generation utility (v%s)." % version)
+    parser = argparse.ArgumentParser(
+        description="A password generation utility (v%s)." % __version__
+    )
     subparsers = parser.add_subparsers(help="The command to execute.", dest="command")
 
     parser_info = subparsers.add_parser(
         "info",
         help=(
-            "Compute information about a password. If passwdgen has input piped into it via stdin, that " +
-            "will be interpreted as the password."
-        )
+            "Compute information about a password. If passwdgen has input piped into it via stdin, that "
+            + "will be interpreted as the password."
+        ),
     )
     parser_info.add_argument(
-        "-d", "--dictionary",
+        "-d",
+        "--dictionary",
         default=None,
-        help="Path to the dictionary file to use. This must be a plain text file with one word per line."
+        help="Path to the dictionary file to use. This must be a plain text file with one word per line.",
     )
     parser_info.add_argument(
-        "-e", "--encoding",
+        "-e",
+        "--encoding",
         default=None,
         help=(
-            "The encoding to use when read/writing input/output files. " +
-            "(See https://docs.python.org/2/library/codecs.html#standard-encodings)"
-        )
+            "The encoding to use when read/writing input/output files. "
+            + "(See https://docs.python.org/2/library/codecs.html#standard-encodings)"
+        ),
     )
 
-    parser_generate = subparsers.add_parser(
-        "generate",
-        help="Generate password(s)."
-    )
+    parser_generate = subparsers.add_parser("generate", help="Generate password(s).")
     parser_generate.add_argument(
-        "-c", "--clipboard",
+        "-c",
+        "--clipboard",
         action="store_true",
         help=(
-            "Copy the generated password to the clipboard (only for when generating a single password) instead of "+
-            "writing the password to stdout"
-        )
+            "Copy the generated password to the clipboard (only for when generating a single password) instead of "
+            + "writing the password to stdout"
+        ),
     )
     parser_generate.add_argument(
-        "-d", "--dictionary",
+        "-d",
+        "--dictionary",
         default=None,
-        help="Path to the dictionary file to use. This must be a plain text file with one word per line."
+        help="Path to the dictionary file to use. This must be a plain text file with one word per line.",
     )
     parser_generate.add_argument(
-        "-e", "--encoding",
+        "-e",
+        "--encoding",
         default=None,
         help=(
-            "The encoding to use when read/writing input/output files. " +
-            "(See https://docs.python.org/2/library/codecs.html#standard-encodings)"
-        )
+            "The encoding to use when read/writing input/output files. "
+            + "(See https://docs.python.org/2/library/codecs.html#standard-encodings)"
+        ),
     )
     parser_generate.add_argument(
-        "-i", "--info",
+        "-i",
+        "--info",
         action="store_true",
-        help="Additionally display information about the generated password, including password entropy."
+        help="Additionally display information about the generated password, including password entropy.",
     )
     parser_generate.add_argument(
-        "-l", "--length",
+        "-l",
+        "--length",
         type=int,
         default=None,
         help=(
-            "The default number of characters or words to generate, depending on which kind of password " +
-            "is being generated (a character- or dictionary-based one). Defaults: %d characters or %d words."
-        ) % (DEFAULT_CHAR_PASSWORD_LENGTH, DEFAULT_WORD_PASSWORD_WORDS)
+            "The default number of characters or words to generate, depending on which kind of password "
+            + "is being generated (a character- or dictionary-based one). Defaults: %d characters or %d words."
+        )
+        % (DEFAULT_CHAR_PASSWORD_LENGTH, DEFAULT_WORD_PASSWORD_WORDS),
     )
     parser_generate.add_argument(
-        "-m", "--min-entropy",
+        "-m",
+        "--min-entropy",
         default=None,
         type=int,
-        help="The minimum entropy of the required password (optional). If length is specified, this will be ignored."
+        help="The minimum entropy of the required password (optional). If length is specified, this will be ignored.",
     )
     parser_generate.add_argument(
-        "-s", "--separator",
+        "-s",
+        "--separator",
         choices=PASSWORD_SEPARATOR_IDS,
         default=SEP_DASH,
         help=(
             "The separator to use when generating passwords from dictionaries (default=%s)."
-        ) % SEP_DASH
+        )
+        % SEP_DASH,
     )
     parser_generate.add_argument(
         "--starting-letters",
         default=None,
-        help=(
-            "The letters to use as initials for the generated words."
-        )
+        help=("The letters to use as initials for the generated words."),
     )
     parser_generate.add_argument(
-        "-t", "--charset",
+        "-t",
+        "--charset",
         choices=PASSWORD_CHARSET_IDS,
         default=PC_DICT,
         help=(
-                 "Which character set/approach to use when generating the password (default=\"%s\"). See the " +
-                 "README.md file at https://github.com/thanethomson/passwdgen for more details."
-             ) % PC_DICT
+            'Which character set/approach to use when generating the password (default="%s"). See the '
+            + "README.md file at https://github.com/thanethomson/passwdgen for more details."
+        )
+        % PC_DICT,
     )
 
     parser_rng = subparsers.add_parser(
         "rng",
-        help="Test the quality of the operating system's random number generator."
+        help="Test the quality of the operating system's random number generator.",
     )
     parser_rng.add_argument(
-        "-s", "--sample-size",
+        "-s",
+        "--sample-size",
         type=int,
         default=1000000,
-        help="Define the sample size to test with (default = 1,000,000)."
+        help="Define the sample size to test with (default = 1,000,000).",
     )
 
-    subparsers.add_parser(
-        "version",
-        help="Display the version of passwdgen and exit."
-    )
+    subparsers.add_parser("version", help="Display the version of passwdgen and exit.")
 
     parser_wordlist = subparsers.add_parser(
-        "wordlist",
-        help="Utilities relating to word list manipulation."
+        "wordlist", help="Utilities relating to word list manipulation."
     )
     subparsers_wordlist = parser_wordlist.add_subparsers(dest="wordlist_subcommand")
 
     parser_wordlist_clean = subparsers_wordlist.add_parser(
         "clean",
-        help="Cleans up a given word list, stripping punctuation, digits and whitespace."
+        help="Cleans up a given word list, stripping punctuation, digits and whitespace.",
     )
     parser_wordlist_clean.add_argument(
-        "input_file",
-        help="The input text file, one word per line, to be cleaned."
+        "input_file", help="The input text file, one word per line, to be cleaned."
     )
     parser_wordlist_clean.add_argument(
-        "output_file",
-        help="The output file into which to write the cleaned word list."
+        "output_file", help="The output file into which to write the cleaned word list."
     )
     parser_wordlist_clean.add_argument(
-        "-e", "--encoding",
+        "-e",
+        "--encoding",
         default=None,
         help=(
-            "The encoding to use when read/writing input/output files. " +
-            "(See https://docs.python.org/2/library/codecs.html#standard-encodings)"
-        )
+            "The encoding to use when read/writing input/output files. "
+            + "(See https://docs.python.org/2/library/codecs.html#standard-encodings)"
+        ),
     )
 
     args = parser.parse_args()
 
     if args.command == "version":
-        print("passwdgen v%s" % version)
+        print("passwdgen v%s" % __version__)
 
     elif args.command == "info":
         if sys.stdin.isatty():
             passwd = getpass("Please enter the password to check: ")
         else:
             # if the input's been piped in
             passwd = sys.stdin.read()
@@ -179,49 +191,48 @@
             if passwd.endswith("\n"):
                 passwd = passwd[:-1]
 
         word_list = load_word_list(filename=args.dictionary, encoding=args.encoding)
         show_password_entropy(passwd, word_list)
 
     elif args.command == "rng":
-        print("Testing OS RNG. Attempting to generate %d samples between 0 and 100 (inclusive). Please wait..." % args.sample_size)
+        print(
+            "Testing OS RNG. Attempting to generate %d samples between 0 and 100 (inclusive). Please wait..."
+            % args.sample_size
+        )
         result = secure_random_quality(args.sample_size)
         print("\nStatistics")
         print("----------")
-        print("Mean               : %.6f (should approach %.3f as the sample size increases; %.3f%% difference)" % (
-            result['mean'],
-            result['expected_mean'],
-            result['mean_diff']
-        ))
-        print("Standard deviation : %.6f (should be as close to %.6f as possible; %.3f%% difference)" % (
-            result['stddev'],
-            result['expected_stddev'],
-            result['stddev_diff']
-        ))
-        print("Time taken         : %.3f seconds\n" % result['time'])
+        print(
+            "Mean               : %.6f (should approach %.3f as the sample size increases; %.3f%% difference)"
+            % (result["mean"], result["expected_mean"], result["mean_diff"])
+        )
+        print(
+            "Standard deviation : %.6f (should be as close to %.6f as possible; %.3f%% difference)"
+            % (result["stddev"], result["expected_stddev"], result["stddev_diff"])
+        )
+        print("Time taken         : %.3f seconds\n" % result["time"])
 
     elif args.command == "generate":
         try:
             word_list = load_word_list(filename=args.dictionary, encoding=args.encoding)
 
             # dictionary-based password generation
             if args.charset == PC_DICT:
                 # load our dictionary
                 passwd = words(
                     word_list,
                     separator=PASSWORD_SEPARATORS[args.separator],
                     word_count=args.length,
                     min_entropy=args.min_entropy,
-                    starting_letters=args.starting_letters
+                    starting_letters=args.starting_letters,
                 )
             else:
                 passwd = chars(
-                    args.charset,
-                    length=args.length,
-                    min_entropy=args.min_entropy
+                    args.charset, length=args.length, min_entropy=args.min_entropy
                 )
 
             if args.clipboard:
                 pyperclip.copy(passwd)
                 print("Password copied to clipboard.")
             else:
                 print(passwd)
@@ -232,16 +243,13 @@
         except ValueError as e:
             print("Error: %s" % e)
 
     elif args.command == "wordlist":
         if args.wordlist_subcommand == "clean":
             print("Attempting to clean word list: %s" % args.input_file)
             result = clean_word_list(
-                args.input_file,
-                args.output_file,
-                encoding=args.encoding
+                args.input_file, args.output_file, encoding=args.encoding
+            )
+            print(
+                "Cleaned file in %.3f seconds. Read %d words, wrote %d."
+                % (result["time"], result["words_read"], result["words_written"])
             )
-            print("Cleaned file in %.3f seconds. Read %d words, wrote %d." % (
-                result["time"],
-                result["words_read"],
-                result["words_written"]
-            ))
```

### Comparing `passwdgen-0.3.1/passwdgen/constants.py` & `passwdgen-0.4.0/passwdgen/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "PASSWORD_CHARSET_IDS",
     "LONGEST_CHARSET_NAME_LEN",
     "DEFAULT_WORD_LIST",
     "DEFAULT_CHAR_PASSWORD_LENGTH",
     "DEFAULT_WORD_PASSWORD_WORDS",
     "DEFAULT_MIN_WORD_LEN",
     "MIN_DICT_SIZE",
-    "DEFAULT_WORD_SEPARATOR"
+    "DEFAULT_WORD_SEPARATOR",
 ]
 
 PC_ALPHA_LOWER = "alpha-lower"
 PC_ALPHA_UPPER = "alpha-upper"
 PC_ALPHA = "alpha"
 PC_ALPHA_NUMERIC = "alpha-numeric"
 PC_ALPHA_NUMERIC_SPACED = "alpha-numeric-spaced"
@@ -65,54 +65,60 @@
     SEP_NONE: "",
     SEP_DASH: "-",
     SEP_UNDERSCORE: "_",
     SEP_PERIOD: ".",
     SEP_SPACE: " ",
     SEP_COMMA: ",",
     SEP_SEMICOLON: ";",
-    SEP_COLON: ":"
+    SEP_COLON: ":",
 }
 
 PASSWORD_SEPARATOR_IDS = [
     SEP_NONE,
     SEP_DASH,
     SEP_UNDERSCORE,
     SEP_PERIOD,
     SEP_SPACE,
     SEP_COMMA,
     SEP_SEMICOLON,
-    SEP_COLON
+    SEP_COLON,
 ]
 
 PASSWORD_CHARSETS = {
     PC_ALPHA_LOWER: set(string.ascii_lowercase),
     PC_ALPHA_UPPER: set(string.ascii_uppercase),
     PC_ALPHA: set(string.ascii_letters),
     PC_ALPHA_NUMERIC: set(string.ascii_letters + string.digits),
     PC_ALPHA_NUMERIC_SPACED: set(string.ascii_letters + string.digits + " "),
     PC_ALPHA_LOWER_SEP: set(string.ascii_lowercase + separators),
     PC_ALPHA_UPPER_SEP: set(string.ascii_uppercase + separators),
     PC_SPECIAL: set(string.ascii_letters + string.digits + special_chars),
-    PC_NUMERIC: set(string.digits)
+    PC_NUMERIC: set(string.digits),
 }
 
 PASSWORD_CHARSET_NAMES = (
     (PC_ALPHA_LOWER, "Alphabetical, lowercase (a-z)"),
     (PC_ALPHA_UPPER, "Alphabetical, uppercase (A-Z)"),
     (PC_ALPHA, "Alphabetical (a-z, A-Z)"),
     (PC_ALPHA_NUMERIC, "Alphabetical and numeric (a-z, A-Z, 0-9)"),
-    (PC_ALPHA_NUMERIC_SPACED, "Alphabetical, numeric, with spaces (a-z, A-Z, 0-9, space)"),
+    (
+        PC_ALPHA_NUMERIC_SPACED,
+        "Alphabetical, numeric, with spaces (a-z, A-Z, 0-9, space)",
+    ),
     (PC_NUMERIC, "Numeric (0-9)"),
     (PC_ALPHA_LOWER_SEP, "Alphabetical, lowercase, with separator (a-z, separator)"),
     (PC_ALPHA_UPPER_SEP, "Alphabetical, uppercase, with separator (A-Z, separator)"),
-    (PC_SPECIAL, "Alphabetical, numeric and special characters (a-z, A-Z, 0-9, punctuation)"),
-    (PC_DICT, "Dictionary")
+    (
+        PC_SPECIAL,
+        "Alphabetical, numeric and special characters (a-z, A-Z, 0-9, punctuation)",
+    ),
+    (PC_DICT, "Dictionary"),
 )
 
-PASSWORD_CHARSET_IDS = [id for id, _ in PASSWORD_CHARSET_NAMES]
+PASSWORD_CHARSET_IDS = [_id for _id, _ in PASSWORD_CHARSET_NAMES]
 LONGEST_CHARSET_NAME_LEN = max([len(name) for _, name in list(PASSWORD_CHARSET_NAMES)])
 
 DEFAULT_CHARSET = PC_SPECIAL
 DEFAULT_WORD_LIST = "data/default-word-list.txt"
 DEFAULT_CHAR_PASSWORD_LENGTH = 12
 DEFAULT_WORD_PASSWORD_WORDS = 4
 DEFAULT_WORD_SEPARATOR = "-"
```

### Comparing `passwdgen-0.3.1/passwdgen/data/default-word-list.txt` & `passwdgen-0.4.0/passwdgen/data/default-word-list.txt`

 * *Files identical despite different names*

### Comparing `passwdgen-0.3.1/passwdgen/generator.py` & `passwdgen-0.4.0/passwdgen/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 import math
 
 from .utils import secure_random, load_word_list
 from .constants import *
 
 
-__all__ = [
-    "chars",
-    "words"
-]
+__all__ = ["chars", "words"]
 
 
 def chars(charset=None, length=None, min_entropy=None):
     """Generates a character-based password. If the length parameter is supplied, the min_entropy parameter
     is ignored (i.e. either a length or a minimum entropy is required, but not both). If no length or
     min_entropy parameters are supplied, a default password length is chosen (see
     constants.DEFAULT_CHAR_PASSWORD_LENGTH).
@@ -52,25 +49,31 @@
 
     return password
 
 
 def select_random_words(word_list, count, starting_letters=None):
     if starting_letters is None:
         total_words = len(word_list)
-        return [word_list[secure_random(total_words)] for i in range(count)]
+        return [word_list[secure_random(total_words)] for _ in range(count)]
     else:
         # assume word_list is a dictionary
         result = []
         for i in range(count):
             ch = starting_letters[i]
             result.append(word_list[ch][secure_random(len(word_list[ch]))])
         return result
 
 
-def words(dict_set=None, separator=None, word_count=None, min_entropy=None, starting_letters=None):
+def words(
+    dict_set=None,
+    separator=None,
+    word_count=None,
+    min_entropy=None,
+    starting_letters=None,
+):
     """Generates a word-based password from the given dictionary. If the word_count parameter is supplied,
     the min_entropy parameter is ignored (i.e. either a word count or minimum entropy is required, but not
     both). If no length or min_entropy parameters are supplied, a default word count is chosen (see
     constants.DEFAULT_WORD_PASSWORD_WORDS).
 
     Args:
         dict_set: The word list/dictionary from which to generate a password. Defaults to the built-in word list.
@@ -101,59 +104,67 @@
                 categorised_words[ch].append(word)
             else:
                 categorised_words[ch] = [word]
 
         # check that all of the required starting letters are represented
         for ch in starting_letters:
             if not (ch in categorised_words):
-                raise ValueError("Dictionary does not contain any words beginning with \"%s\"" % ch)
+                raise ValueError(
+                    'Dictionary does not contain any words beginning with "%s"' % ch
+                )
 
     password_words = []
 
     if word_count is None and min_entropy is None:
-        word_count = DEFAULT_WORD_PASSWORD_WORDS if starting_letters is None else len(starting_letters)
+        word_count = (
+            DEFAULT_WORD_PASSWORD_WORDS
+            if starting_letters is None
+            else len(starting_letters)
+        )
 
     if separator is None:
         separator = DEFAULT_WORD_SEPARATOR
 
     if word_count is not None:
         if starting_letters is None:
             password_words.extend(select_random_words(word_list, word_count))
 
         else:
             if len(starting_letters) < word_count:
-                raise ValueError((
-                    "Please supply at least %d starting letters to meet the minimum word count " +
-                    "requirement"
-                ) % word_count)
+                raise ValueError(
+                    (
+                        "Please supply at least %d starting letters to meet the minimum word count "
+                        + "requirement"
+                    )
+                    % word_count
+                )
 
             password_words.extend(
                 select_random_words(
-                    categorised_words,
-                    word_count,
-                    starting_letters=starting_letters
+                    categorised_words, word_count, starting_letters=starting_letters
                 )
             )
 
     else:
         entropy_per_word = math.log(word_list_size, 2.0)
         min_words = int(math.ceil(min_entropy / entropy_per_word))
 
         if starting_letters is None:
             password_words.extend(select_random_words(word_list, min_words))
 
         else:
             if len(starting_letters) < min_words:
-                raise ValueError((
-                    "Please supply at least %d starting letters to meet the minimum word count " +
-                    "requirement"
-                ) % min_words)
+                raise ValueError(
+                    (
+                        "Please supply at least %d starting letters to meet the minimum word count "
+                        + "requirement"
+                    )
+                    % min_words
+                )
 
             password_words.extend(
                 select_random_words(
-                    categorised_words,
-                    min_words,
-                    starting_letters=starting_letters
+                    categorised_words, min_words, starting_letters=starting_letters
                 )
             )
 
     return separator.join(password_words)
```

### Comparing `passwdgen-0.3.1/passwdgen/utils.py` & `passwdgen-0.4.0/passwdgen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 from functools import reduce
 from operator import mul
 from string import ascii_lowercase
 from io import open
 import time
 import math
-import pkg_resources
 import os
 import struct
+import importlib.resources
 
 from .constants import *
 
 
 __all__ = [
     "clean_word_list",
     "permutations",
     "calculate_entropy",
     "load_word_list",
     "secure_random",
-    "secure_random_quality"
+    "secure_random_quality",
 ]
 
 
 def clean_word_list(input_path, output_path, encoding=None, min_word_len=None):
     """Cleans the given word list, ensuring no punctuation or capitalisation or duplicate words. Word lists
     must be plain text files, with one word per line, and sorted alphabetically.
 
@@ -64,15 +64,15 @@
         for word in sorted(list(word_list)):
             output_file.write("%s\n" % word)
 
     end_time = time.time()
     return {
         "time": end_time - start_time,
         "words_read": words_read,
-        "words_written": len(word_list)
+        "words_written": len(word_list),
     }
 
 
 def permutations(n, k):
     """Calculates the number of ordered k-permutations of n.
 
     Args:
@@ -99,15 +99,15 @@
     password_letters = set(password)
     password_len = len(password)
     entropy = dict()
 
     # find the charsets in which we'll find this password
     for charset_name, charset in PASSWORD_CHARSETS.items():
         if password_letters.issubset(charset):
-            entropy[charset_name] = math.log(1.0*len(charset), 2.0) * password_len
+            entropy[charset_name] = math.log(1.0 * len(charset), 2.0) * password_len
 
     if dict_set is not None:
         # we assume our dictionary words are all lowercase, and that our separator is used
         if password_letters.issubset(PASSWORD_CHARSETS[PC_ALPHA_LOWER_SEP]):
             # detect the separator
             sep = None
             for c in password_letters:
@@ -122,15 +122,17 @@
                 all_words_found = True
                 for word in words:
                     if word not in dict_set:
                         all_words_found = False
 
                 # only if all of the words in the password are in our specific dictionary
                 if all_words_found:
-                    entropy[PC_DICT] = math.log(permutations(len(dict_set), len(words)), 2.0)
+                    entropy[PC_DICT] = math.log(
+                        permutations(len(dict_set), len(words)), 2.0
+                    )
 
     return entropy
 
 
 def load_word_list(filename=None, resource=None, encoding=None):
     """Loads a word list from the given filename or resource.
 
@@ -142,24 +144,29 @@
 
     Returns:
         A set containing the entire list of non-zero-length words in the word list.
     """
     words = set()
 
     if filename is None:
-        filename = pkg_resources.resource_filename("passwdgen", resource or DEFAULT_WORD_LIST)
+        filename = importlib.resources.files("passwdgen").joinpath(
+            resource or DEFAULT_WORD_LIST
+        )
 
     with open(filename, "rt", encoding=encoding) as input_file:
         for line in input_file:
             word = line.strip()
             if len(word) > 0:
                 words.add(word)
 
     if len(words) < MIN_DICT_SIZE:
-        raise ValueError("Dictionary is too small. Valid dictionaries must contain at least %d unique words." % MIN_DICT_SIZE)
+        raise ValueError(
+            "Dictionary is too small. Valid dictionaries must contain at least %d unique words."
+            % MIN_DICT_SIZE
+        )
 
     return words
 
 
 def secure_random(a, b=None):
     """Generates integers in the most secure manner possible provided by the operating system. On POSIX machines,
     this will use /dev/urandom. On Windows machines, this will use CryptGenRandom().
@@ -170,19 +177,21 @@
             minimum will be 0.
         b: If supplied, this must provide the maximum value of the randomly generated number (exclusive).
 
     Returns:
         A random integer i, with a <= i < b if b is supplied, otherwise 0 <= i < a.
     """
     if (a < 0) or ((b is not None) and (b < 0)):
-        raise ValueError("Both a and b need to be integers >= 0 for secure random number generation")
+        raise ValueError(
+            "Both a and b need to be integers >= 0 for secure random number generation"
+        )
     if (b is not None) and (b <= a):
         raise ValueError("For secure random number generation, b must be < a")
 
-    (random_val, ) = struct.unpack("Q", os.urandom(8))
+    (random_val,) = struct.unpack("Q", os.urandom(8))
     return (random_val % int(a)) if b is None else (int(a) + (random_val % int(b - a)))
 
 
 def secure_random_quality(sample_size=1000000):
     """Attempts to estimate the quality of the secure random number generator of the operating system.
 
     Args:
@@ -206,20 +215,20 @@
     for val, count in counts.items():
         variance += ((val - mean) ** 2.0) * count
     variance /= float(sample_size) - 1.0
     # ensure variance is positive (sometimes zeros can be negative with floating point numbers)
     if variance < 0.0:
         variance *= -1.0
     stddev = math.sqrt(variance)
-    expected_variance = ((101.0 ** 2.0) - 1.0) / 12.0
+    expected_variance = ((101.0**2.0) - 1.0) / 12.0
     expected_stddev = math.sqrt(expected_variance)
 
     end_time = time.time()
     return {
         "mean": mean,
         "expected_mean": 50.0,
         "mean_diff": 100.0 * (abs(50.0 - mean) / 50.0),
         "stddev": stddev,
         "expected_stddev": expected_stddev,
         "stddev_diff": 100.0 * (abs(expected_stddev - stddev) / expected_stddev),
-        "time": end_time - start_time
+        "time": end_time - start_time,
     }
```

