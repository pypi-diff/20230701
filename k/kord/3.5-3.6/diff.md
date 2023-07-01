# Comparing `tmp/kord-3.5.tar.gz` & `tmp/kord-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kord-3.5.tar", last modified: Tue Nov 10 12:54:30 2020, max compression
+gzip compressed data, was "kord-3.6.tar", last modified: Sat Jul  1 00:47:13 2023, max compression
```

## Comparing `kord-3.5.tar` & `kord-3.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 sosa      (1000) sosa      (1000)        0 2020-11-10 12:54:30.788343 kord-3.5/
--rw-rw-r--   0 sosa      (1000) sosa      (1000)    13706 2020-11-10 12:54:30.788343 kord-3.5/PKG-INFO
--rw-rw-r--   0 sosa      (1000) sosa      (1000)    10607 2020-11-10 12:53:37.000000 kord-3.5/README.md
-drwxrwxr-x   0 sosa      (1000) sosa      (1000)        0 2020-11-10 12:54:30.788343 kord-3.5/app/
--rw-rw-r--   0 sosa      (1000) sosa      (1000)     6067 2020-11-08 23:11:56.000000 kord-3.5/app/fretboard.py
--rw-rw-r--   0 sosa      (1000) sosa      (1000)     1455 2020-11-03 08:20:38.000000 kord-3.5/app/tuner.py
-drwxrwxr-x   0 sosa      (1000) sosa      (1000)        0 2020-11-10 12:54:30.788343 kord-3.5/app/tunings/
--rw-rw-r--   0 sosa      (1000) sosa      (1000)       83 2020-11-02 21:30:49.000000 kord-3.5/app/tunings/banjo.json
--rw-rw-r--   0 sosa      (1000) sosa      (1000)      283 2020-11-02 21:30:49.000000 kord-3.5/app/tunings/bass.json
--rw-rw-r--   0 sosa      (1000) sosa      (1000)     1111 2020-11-08 10:58:06.000000 kord-3.5/app/tunings/guitar.json
--rw-rw-r--   0 sosa      (1000) sosa      (1000)      159 2020-11-07 10:43:17.000000 kord-3.5/app/tunings/ukulele.json
-drwxrwxr-x   0 sosa      (1000) sosa      (1000)        0 2020-11-10 12:54:30.788343 kord-3.5/kord/
--rwxrwxr-x   0 sosa      (1000) sosa      (1000)       27 2020-10-25 17:58:18.000000 kord-3.5/kord/__init__.py
--rw-rw-r--   0 sosa      (1000) sosa      (1000)      255 2020-10-22 22:31:00.000000 kord-3.5/kord/errors.py
--rw-rw-r--   0 sosa      (1000) sosa      (1000)     6704 2020-11-08 10:58:11.000000 kord-3.5/kord/instruments.py
--rw-rw-r--   0 sosa      (1000) sosa      (1000)    12560 2020-11-08 10:58:11.000000 kord-3.5/kord/keys.py
--rw-rw-r--   0 sosa      (1000) sosa      (1000)     8416 2020-11-08 23:25:09.000000 kord-3.5/kord/notes.py
--rw-rw-r--   0 sosa      (1000) sosa      (1000)    36722 2020-11-08 23:18:31.000000 kord-3.5/kord/tests.py
-drwxrwxr-x   0 sosa      (1000) sosa      (1000)        0 2020-11-10 12:54:30.788343 kord-3.5/kord.egg-info/
--rw-rw-r--   0 sosa      (1000) sosa      (1000)    13706 2020-11-10 12:54:30.000000 kord-3.5/kord.egg-info/PKG-INFO
--rw-rw-r--   0 sosa      (1000) sosa      (1000)      374 2020-11-10 12:54:30.000000 kord-3.5/kord.egg-info/SOURCES.txt
--rw-rw-r--   0 sosa      (1000) sosa      (1000)        1 2020-11-10 12:54:30.000000 kord-3.5/kord.egg-info/dependency_links.txt
--rw-rw-r--   0 sosa      (1000) sosa      (1000)        7 2020-11-10 12:54:30.000000 kord-3.5/kord.egg-info/requires.txt
--rw-rw-r--   0 sosa      (1000) sosa      (1000)        5 2020-11-10 12:54:30.000000 kord-3.5/kord.egg-info/top_level.txt
--rw-rw-r--   0 sosa      (1000) sosa      (1000)       38 2020-11-10 12:54:30.788343 kord-3.5/setup.cfg
--rw-rw-r--   0 sosa      (1000) sosa      (1000)     1178 2020-11-10 12:54:12.000000 kord-3.5/setup.py
+drwxr-xr-x   0 belusi     (501) staff       (20)        0 2023-07-01 00:47:13.451165 kord-3.6/
+-rw-r--r--   0 belusi     (501) staff       (20)     1075 2022-12-14 20:37:29.000000 kord-3.6/LICENSE
+-rw-r--r--   0 belusi     (501) staff       (20)    11153 2023-07-01 00:47:13.450921 kord-3.6/PKG-INFO
+-rw-r--r--   0 belusi     (501) staff       (20)    10607 2022-12-14 20:37:30.000000 kord-3.6/README.md
+drwxr-xr-x   0 belusi     (501) staff       (20)        0 2023-07-01 00:47:13.448971 kord-3.6/app/
+-rw-r--r--   0 belusi     (501) staff       (20)     6067 2022-12-14 20:37:29.000000 kord-3.6/app/fretboard.py
+-rw-r--r--   0 belusi     (501) staff       (20)     1455 2022-12-14 20:37:29.000000 kord-3.6/app/tuner.py
+drwxr-xr-x   0 belusi     (501) staff       (20)        0 2023-07-01 00:47:13.449397 kord-3.6/app/tunings/
+-rw-r--r--   0 belusi     (501) staff       (20)       83 2022-12-14 20:37:29.000000 kord-3.6/app/tunings/banjo.json
+-rw-r--r--   0 belusi     (501) staff       (20)      283 2022-12-14 20:37:29.000000 kord-3.6/app/tunings/bass.json
+-rw-r--r--   0 belusi     (501) staff       (20)     1111 2022-12-14 20:37:29.000000 kord-3.6/app/tunings/guitar.json
+-rw-r--r--   0 belusi     (501) staff       (20)      159 2022-12-14 20:37:29.000000 kord-3.6/app/tunings/ukulele.json
+drwxr-xr-x   0 belusi     (501) staff       (20)        0 2023-07-01 00:47:13.450040 kord-3.6/kord/
+-rwxr-xr-x   0 belusi     (501) staff       (20)       27 2022-12-14 20:37:30.000000 kord-3.6/kord/__init__.py
+-rw-r--r--   0 belusi     (501) staff       (20)      255 2022-12-14 20:37:30.000000 kord-3.6/kord/errors.py
+-rw-r--r--   0 belusi     (501) staff       (20)     6704 2022-12-14 20:37:30.000000 kord-3.6/kord/instruments.py
+-rw-r--r--   0 belusi     (501) staff       (20)    12560 2022-12-14 20:37:30.000000 kord-3.6/kord/keys.py
+-rw-r--r--   0 belusi     (501) staff       (20)     8416 2022-12-14 20:37:30.000000 kord-3.6/kord/notes.py
+-rw-r--r--   0 belusi     (501) staff       (20)    36722 2022-12-14 20:37:30.000000 kord-3.6/kord/tests.py
+drwxr-xr-x   0 belusi     (501) staff       (20)        0 2023-07-01 00:47:13.450694 kord-3.6/kord.egg-info/
+-rw-r--r--   0 belusi     (501) staff       (20)    11153 2023-07-01 00:47:13.000000 kord-3.6/kord.egg-info/PKG-INFO
+-rw-r--r--   0 belusi     (501) staff       (20)      382 2023-07-01 00:47:13.000000 kord-3.6/kord.egg-info/SOURCES.txt
+-rw-r--r--   0 belusi     (501) staff       (20)        1 2023-07-01 00:47:13.000000 kord-3.6/kord.egg-info/dependency_links.txt
+-rw-r--r--   0 belusi     (501) staff       (20)        7 2023-07-01 00:47:13.000000 kord-3.6/kord.egg-info/requires.txt
+-rw-r--r--   0 belusi     (501) staff       (20)        5 2023-07-01 00:47:13.000000 kord-3.6/kord.egg-info/top_level.txt
+-rw-r--r--   0 belusi     (501) staff       (20)       38 2023-07-01 00:47:13.451204 kord-3.6/setup.cfg
+-rw-r--r--   0 belusi     (501) staff       (20)     1178 2023-07-01 00:45:55.000000 kord-3.6/setup.py
```

### Comparing `kord-3.5/PKG-INFO` & `kord-3.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,334 +1,318 @@
-Metadata-Version: 2.1
-Name: kord
-Version: 3.5
-Summary: a framework for programming music applications
-Home-page: https://github.com/synestematic/kord
-Author: Federico Rizzo
-Author-email: synestem@ticATgmail.com
-License: MIT
-Description: # kord
-        kord is a python framework that provides programmers with a simple api for the creation of music-based applications. While it's mainly intended for theoretical purposes, some of it's modules contain functionality specifically tailored for dealing with plucked-string instruments.
-        
-        ![](https://github.com/synestematic/kord/blob/master/resources/chrom.png?raw=true)
-        
-        ## installation
-        
-        The only dependency for `kord` is the package `bestia`, my own library for creating command-line applications. Both can be automatically installed using pip:
-        
-        ```
-        $  python3 -m pip install kord
-        ```
-        
-        The fretboard application component of the framework can also be run directly in a containerized form. This requires you to install 0 dependencies on your system besides docker. 
-        
-        ```
-        $  docker run -t synestematic/kord  C --scale major
-        ```
-        
-        Scroll to the bottom of the README for more information on the fretboard application.
-        
-        
-        # api reference:
-        
-        Please only expect to understand the following documentation if you have an above basic understanding of music theory. With that said, let's dive into the first module:
-        
-        
-        ## kord.notes
-        
-        ### class MusicNote(object):
-        
-        MusicNote instances are the building blocks of the framework and have 3 main attributes:
-        
-        ```
-        * chr: str    ('C', 'D', 'E', 'F', 'G', 'A', 'B')
-        * alt: str    ('bb', 'b', '', '#', '##')
-        * oct: int    (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
-        ```
-        
-        You can set these values when creating an instance and only the `chr` argument is required. Arguments `alt` and `oct` will default to `''` and `3` respectively. These are __positional__ arguments, not keyword arguments so keep that in mind when creating your objects.
-        
-        ```
-        >>> from kord.notes import MusicNote
-        >>> e3, f3 = MusicNote('e'), MusicNote('f')
-        >>> e3, f3
-        (E³, F³) 
-        >>> MusicNote('G', 'b')
-        G♭³
-        >>> MusicNote('C', 9)
-        C⁹
-        >>> MusicNote('B', 'b', 7)
-        B♭⁷
-        >>> MusicNote('C', '#', 0)
-        C♯⁰
-        ```
-        
-        Notes with double alterations are supported but Notes with triple or more alterations will raise an exception:
-        
-        ```
-        >>> MusicNote('A', 'bb', 1)
-        A𝄫¹
-        >>> MusicNote('F', '##', 1)
-        F𝄪¹
-        >>> MusicNote('G', '###')
-        Traceback (most recent call last):
-          File "<stdin>", line 1, in <module>
-          ...
-        kord.errors.InvalidAlteration: ###
-        ```
-        
-        Similarly, the maximum octave value currently supported is 9.
-        
-        ```
-        >>> MusicNote('D', 10)
-        Traceback (most recent call last):
-          File "<stdin>", line 1, in <module>
-          ...
-        kord.errors.InvalidOctave: 10
-        ```
-        
-        ### Comparing MusicNote objects:
-         
-        The ```-   < >   <= >=   == !=   >>   ** ```  operators allow computation of semitone intervals between MusicNote instances and give insight into their enharmonic relationships. Let's take a quick look at each operator separately:
-        
-        #### - operator
-        
-        The substraction operator lets you compute the difference in semitones between two notes:
-        
-        ```
-        >>> f3 - e3
-        1
-        >>> MusicNote('a', 'b', 2) - MusicNote('g', '#', 2)
-        0
-        >>> MusicNote('a', 8) - MusicNote('c', 4)
-        57
-        >>> MusicNote('a', 8) - MusicNote('c', '##', 4)
-        55
-        ```
-        
-        
-        ####  < >   <= >=   == !=  operators
-        
-        Comparison operators return boolean values based *exclusively* on the interval between the 2 objects. 
-        
-        ```
-        >>> f3 > e3
-        True
-        >>> f3 >= e3
-        True
-        ```
-        
-        While the concept is seemingly straightforward, special attention needs to be taken when using `== !=` with enharmonic notes.
-        
-        ```
-        >>> n1 = MusicNote('F', '#', 5)
-        >>> n2 = MusicNote('G', 'b', 5)
-        >>> n1, n2
-        (F♯⁵, G♭⁵)
-        >>> n1 == n2
-        True
-        ```
-        
-        The notes F♯⁵ and G♭⁵ are NOT the same but since their interval is a unison, the `==` comparison evaluates True. This might seem a bit counter-intuitive at first but you can still check for exact note matches with the use of 2 other operators.
-        
-        #### >> ** operators
-        
-        The power and right-shift operators allow you to compare Notes for equality based not on their intervals, but on their intrinsic `chr`, `alt`, `oct` properties. The strictest operator `>>` compares all 3 attributes for equality while the looser `**` ignores `oct`: 
-        
-        ```
-        >>> ab1, ab5 = MusicNote('A', 'b', 1),  MusicNote('A', 'b', 5)
-        >>> ab1 == ab5
-        False
-        >>> ab1 ** ab5
-        True
-        ```
-        
-        Notice `**` evaluates True since both instances are A flat notes, even when there is a wide interval between them.
-        
-        ```
-        >>> ab1 >> ab5
-        False
-        >>> ab1.oct = 5
-        >>> ab1 >> ab5
-        True
-        ```
-        
-        For the `>>` operator to evaluate True, the octaves of the notes must match as well.
-        
-        
-        <hr/>
-        
-        
-        
-        
-        ## kord.keys
-        
-        
-        ### class MusicKey(object):
-        
-        Think of MusicKey objects as generators of MusicNote objects. You can define a new class which inherits MusicKey and use any theoretical arrangement of `intervals` from the root note in order to create chords, scales, modes, etc. You can further taylor these child classes by restricting `degrees` to specific values, this is very useful for creating chords.
-        
-        These are a couple of pre-defined examples to give you an idea of how it works:
-        
-        ```
-        class ChromaticScale(MusicKey):
-            intervals = (
-                UNISON,
-                MINOR_SECOND,
-                MAJOR_SECOND,
-                MINOR_THIRD,
-                MAJOR_THIRD,
-                PERFECT_FOURTH,
-                AUGMENTED_FOURTH,
-                PERFECT_FIFTH,
-                MINOR_SIXTH,
-                MAJOR_SIXTH,
-                MINOR_SEVENTH,
-                MAJOR_SEVENTH,
-            )
-        
-        class MajorScale(MusicKey):
-            intervals = (
-                UNISON,
-                MAJOR_SECOND,
-                MAJOR_THIRD,
-                PERFECT_FOURTH,
-                PERFECT_FIFTH,
-                MAJOR_SIXTH,
-                MAJOR_SEVENTH,
-            )
-            
-        class MajorPentatonicScale(MajorScale):
-            degrees = (1, 2, 3, 5, 6)
-        
-        class MajorTriad(MajorScale):
-            degrees = (1, 3, 5)
-        ```
-        
-        Bare in mind that MusicKey objects are initialized with `chr` and `alt` attributes, `oct` values are not taken into consideration. These allows us to simply unpack MusicNote objects in order to create MusicKey instances based off of them. Once we have a MusicKey object, we can access it's single degrees using list index notation:
-        
-        ```
-        >>> from kord.keys import ChromaticScale
-        >>> c = MusicNote('C')
-        >>> c_chromatic_scale = ChromaticScale(*c)
-        >>> c_chromatic_scale[2]
-        C♯⁰
-        >>> c_chromatic_scale[12]
-        B⁰
-        ```
-        
-        ### MusicKey.spell()
-        
-        Retrieving individual degrees is good, but it is perhaps more interesting to look at a more dynamic way of getting notes out of our MusicKey instances. The `spell()` method provides such an interface for generating MusicNote instances on the fly. Let's take a look at a couple of examples and the several arguments that we can use when calling this method:
-        
-        ```
-        >>> for note in c_chromatic_scale.spell():
-        ...     print(note, end=' ')
-        ...
-        C⁰ C♯⁰ D⁰ D♯⁰ E⁰ F⁰ F♯⁰ G⁰ G♯⁰ A⁰ A♯⁰ B⁰ C¹ >>> 
-        ```
-        
-        As seen above the method will generate the first octave of degrees of the object when called without arguments.
-        
-        The `note_count` argument is an `int` and it allows us to set a specific amount of notes to retrieve:
-        
-        ```
-        >>> from kord.keys import MinorScale
-        >>> a_minor_scale = MinorScale('A')
-        >>> for note in a_minor_scale.spell(note_count=4):
-        ...     print(note, end=' ')
-        ...
-        A⁰ B⁰ C¹ D¹ >>> 
-        ```
-        
-        Be careful, ask for too many notes and kord will throw and Exception when `oct` 9 has been exceeded.
-        
-        The `yield_all` argument is a `bool` that will make the method yield not just `MusicNote` instances, but also `None` objects for every non-diatonic semitone found:
-        
-        ```
-        >>> for note in a_minor_scale.spell(note_count=4, yield_all=True):
-        ...     print(note, end=' ')
-        ...
-        A⁰ None B⁰ C¹ None D¹ >>> 
-        ```
-        
-        
-        The `start_note` argument is a `MusicNote` object that can be used to start getting notes only after a specific note has been found. This can be done even if the note is not diatonic to the scale:
-        
-        ```
-        >>> Db1 = MusicNote('D', 'b', 1)
-        >>> for note in a_minor_scale.spell(note_count=4, yield_all=True, start_note=Db1):
-        ...     print(note, end=' ')
-        ...
-        None D¹ None E¹ F¹ None G¹ >>> 
-        ```
-        
-        
-        
-        ## fretboard tool
-        
-        A sample application `fretboard.py` comes built-in with `kord` and gives some insight into the possibilities of the framework. It displays a representation of your instrument's fretboard, tuned to your liking along with note patterns for any given mode (scale/chord) for any given root note. 
-        
-        If you installed via pip (as opposed to cloning this repo) installation path will depend on your system, it's usually something like `/usr/local/fretboard` or `~/.local/fretboard`. You will also find a `tunings` directory with some pre-defined instrument tunings in the form of .json files. Feel free to modify them or add your own and they should immediately become available to the run-time.
-        
-        ```
-        $  python3 fretboard.py --help
-        usage: fretboard.py [-h] [-d] [-s  | -c ] [-i] [-t] [-f] [-v] root
-        
-        <<< Fretboard visualizer sample tool for the kord music framework >>>
-        
-        positional arguments:
-          root                select key ROOT note
-        
-        optional arguments:
-          -h, --help          show this help message and exit
-          -d, --degrees       show degree numbers instead of note pitches
-          -s , --scale        major, minor, melodic_minor, harmonic_minor, major_pentatonic, minor_pentatonic,
-                              ionian, lydian, mixolydian, aeolian, dorian, phrygian, locrian, chromatic
-          -c , --chord        maj, min, aug, dim, maj7, min7, 7, dim7, min7dim5, maj9, min9, 9
-          -i , --instrument   banjo, guitar, pedal, bass, ukulele
-          -t , --tuning       check .json files for available options
-          -f , --frets        1, 2, .., 36
-          -v , --verbosity    0, 1, 2
-        ```
-        
-        The only required parameter is the `root` note. 
-        
-        The `--scale` and `--chord` options let you choose which note pattern to display for the selected root. They are mutually exclusive and the default value is `--chord maj` when left blank.
-        
-        The `--instrument` and `--tuning` options refer to the json files you will find in the tunings directory. Default values are `--instrument guitar   --tuning standard`.
-        
-        The `--frets` option let's you choose how many frets to visualize, maximum value is 36. Default value will fill your terminal screen.
-        
-        The `--verbosity` option let's you choose how much information to see on-screen from 0 to 2. Default value is 1.
-        
-        The `--degrees` option let's you display degree numbers instead of notes. Default value is false.
-        
-        
-        ## screenshots
-        
-        Here are a couple of pics to get you excited:
-        
-        ### chords
-        
-        ![](https://github.com/synestematic/kord/blob/master/resources/e7.png?raw=true)
-        
-        ![](https://github.com/synestematic/kord/blob/master/resources/dim7.png?raw=true)
-        
-        ### scales
-        
-        ![](https://github.com/synestematic/kord/blob/master/resources/penta.png?raw=true)
-        
-        ![](https://github.com/synestematic/kord/blob/master/resources/cs.png?raw=true)
-        
-        ![](https://github.com/synestematic/kord/blob/master/resources/lydian.png?raw=true)
-        
-        
-        Keep on rocking!
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Description-Content-Type: text/markdown
+# kord
+kord is a python framework that provides programmers with a simple api for the creation of music-based applications. While it's mainly intended for theoretical purposes, some of it's modules contain functionality specifically tailored for dealing with plucked-string instruments.
+
+![](https://github.com/synestematic/kord/blob/master/resources/chrom.png?raw=true)
+
+## installation
+
+The only dependency for `kord` is the package `bestia`, my own library for creating command-line applications. Both can be automatically installed using pip:
+
+```
+$  python3 -m pip install kord
+```
+
+The fretboard application component of the framework can also be run directly in a containerized form. This requires you to install 0 dependencies on your system besides docker. 
+
+```
+$  docker run -t synestematic/kord  C --scale major
+```
+
+Scroll to the bottom of the README for more information on the fretboard application.
+
+
+# api reference:
+
+Please only expect to understand the following documentation if you have an above basic understanding of music theory. With that said, let's dive into the first module:
+
+
+## kord.notes
+
+### class MusicNote(object):
+
+MusicNote instances are the building blocks of the framework and have 3 main attributes:
+
+```
+* chr: str    ('C', 'D', 'E', 'F', 'G', 'A', 'B')
+* alt: str    ('bb', 'b', '', '#', '##')
+* oct: int    (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
+```
+
+You can set these values when creating an instance and only the `chr` argument is required. Arguments `alt` and `oct` will default to `''` and `3` respectively. These are __positional__ arguments, not keyword arguments so keep that in mind when creating your objects.
+
+```
+>>> from kord.notes import MusicNote
+>>> e3, f3 = MusicNote('e'), MusicNote('f')
+>>> e3, f3
+(E³, F³) 
+>>> MusicNote('G', 'b')
+G♭³
+>>> MusicNote('C', 9)
+C⁹
+>>> MusicNote('B', 'b', 7)
+B♭⁷
+>>> MusicNote('C', '#', 0)
+C♯⁰
+```
+
+Notes with double alterations are supported but Notes with triple or more alterations will raise an exception:
+
+```
+>>> MusicNote('A', 'bb', 1)
+A𝄫¹
+>>> MusicNote('F', '##', 1)
+F𝄪¹
+>>> MusicNote('G', '###')
+Traceback (most recent call last):
+  File "<stdin>", line 1, in <module>
+  ...
+kord.errors.InvalidAlteration: ###
+```
+
+Similarly, the maximum octave value currently supported is 9.
+
+```
+>>> MusicNote('D', 10)
+Traceback (most recent call last):
+  File "<stdin>", line 1, in <module>
+  ...
+kord.errors.InvalidOctave: 10
+```
+
+### Comparing MusicNote objects:
+ 
+The ```-   < >   <= >=   == !=   >>   ** ```  operators allow computation of semitone intervals between MusicNote instances and give insight into their enharmonic relationships. Let's take a quick look at each operator separately:
+
+#### - operator
+
+The substraction operator lets you compute the difference in semitones between two notes:
+
+```
+>>> f3 - e3
+1
+>>> MusicNote('a', 'b', 2) - MusicNote('g', '#', 2)
+0
+>>> MusicNote('a', 8) - MusicNote('c', 4)
+57
+>>> MusicNote('a', 8) - MusicNote('c', '##', 4)
+55
+```
+
+
+####  < >   <= >=   == !=  operators
+
+Comparison operators return boolean values based *exclusively* on the interval between the 2 objects. 
+
+```
+>>> f3 > e3
+True
+>>> f3 >= e3
+True
+```
+
+While the concept is seemingly straightforward, special attention needs to be taken when using `== !=` with enharmonic notes.
+
+```
+>>> n1 = MusicNote('F', '#', 5)
+>>> n2 = MusicNote('G', 'b', 5)
+>>> n1, n2
+(F♯⁵, G♭⁵)
+>>> n1 == n2
+True
+```
+
+The notes F♯⁵ and G♭⁵ are NOT the same but since their interval is a unison, the `==` comparison evaluates True. This might seem a bit counter-intuitive at first but you can still check for exact note matches with the use of 2 other operators.
+
+#### >> ** operators
+
+The power and right-shift operators allow you to compare Notes for equality based not on their intervals, but on their intrinsic `chr`, `alt`, `oct` properties. The strictest operator `>>` compares all 3 attributes for equality while the looser `**` ignores `oct`: 
+
+```
+>>> ab1, ab5 = MusicNote('A', 'b', 1),  MusicNote('A', 'b', 5)
+>>> ab1 == ab5
+False
+>>> ab1 ** ab5
+True
+```
+
+Notice `**` evaluates True since both instances are A flat notes, even when there is a wide interval between them.
+
+```
+>>> ab1 >> ab5
+False
+>>> ab1.oct = 5
+>>> ab1 >> ab5
+True
+```
+
+For the `>>` operator to evaluate True, the octaves of the notes must match as well.
+
+
+<hr/>
+
+
+
+
+## kord.keys
+
+
+### class MusicKey(object):
+
+Think of MusicKey objects as generators of MusicNote objects. You can define a new class which inherits MusicKey and use any theoretical arrangement of `intervals` from the root note in order to create chords, scales, modes, etc. You can further taylor these child classes by restricting `degrees` to specific values, this is very useful for creating chords.
+
+These are a couple of pre-defined examples to give you an idea of how it works:
+
+```
+class ChromaticScale(MusicKey):
+    intervals = (
+        UNISON,
+        MINOR_SECOND,
+        MAJOR_SECOND,
+        MINOR_THIRD,
+        MAJOR_THIRD,
+        PERFECT_FOURTH,
+        AUGMENTED_FOURTH,
+        PERFECT_FIFTH,
+        MINOR_SIXTH,
+        MAJOR_SIXTH,
+        MINOR_SEVENTH,
+        MAJOR_SEVENTH,
+    )
+
+class MajorScale(MusicKey):
+    intervals = (
+        UNISON,
+        MAJOR_SECOND,
+        MAJOR_THIRD,
+        PERFECT_FOURTH,
+        PERFECT_FIFTH,
+        MAJOR_SIXTH,
+        MAJOR_SEVENTH,
+    )
+    
+class MajorPentatonicScale(MajorScale):
+    degrees = (1, 2, 3, 5, 6)
+
+class MajorTriad(MajorScale):
+    degrees = (1, 3, 5)
+```
+
+Bare in mind that MusicKey objects are initialized with `chr` and `alt` attributes, `oct` values are not taken into consideration. These allows us to simply unpack MusicNote objects in order to create MusicKey instances based off of them. Once we have a MusicKey object, we can access it's single degrees using list index notation:
+
+```
+>>> from kord.keys import ChromaticScale
+>>> c = MusicNote('C')
+>>> c_chromatic_scale = ChromaticScale(*c)
+>>> c_chromatic_scale[2]
+C♯⁰
+>>> c_chromatic_scale[12]
+B⁰
+```
+
+### MusicKey.spell()
+
+Retrieving individual degrees is good, but it is perhaps more interesting to look at a more dynamic way of getting notes out of our MusicKey instances. The `spell()` method provides such an interface for generating MusicNote instances on the fly. Let's take a look at a couple of examples and the several arguments that we can use when calling this method:
+
+```
+>>> for note in c_chromatic_scale.spell():
+...     print(note, end=' ')
+...
+C⁰ C♯⁰ D⁰ D♯⁰ E⁰ F⁰ F♯⁰ G⁰ G♯⁰ A⁰ A♯⁰ B⁰ C¹ >>> 
+```
+
+As seen above the method will generate the first octave of degrees of the object when called without arguments.
+
+The `note_count` argument is an `int` and it allows us to set a specific amount of notes to retrieve:
+
+```
+>>> from kord.keys import MinorScale
+>>> a_minor_scale = MinorScale('A')
+>>> for note in a_minor_scale.spell(note_count=4):
+...     print(note, end=' ')
+...
+A⁰ B⁰ C¹ D¹ >>> 
+```
+
+Be careful, ask for too many notes and kord will throw and Exception when `oct` 9 has been exceeded.
+
+The `yield_all` argument is a `bool` that will make the method yield not just `MusicNote` instances, but also `None` objects for every non-diatonic semitone found:
+
+```
+>>> for note in a_minor_scale.spell(note_count=4, yield_all=True):
+...     print(note, end=' ')
+...
+A⁰ None B⁰ C¹ None D¹ >>> 
+```
+
+
+The `start_note` argument is a `MusicNote` object that can be used to start getting notes only after a specific note has been found. This can be done even if the note is not diatonic to the scale:
+
+```
+>>> Db1 = MusicNote('D', 'b', 1)
+>>> for note in a_minor_scale.spell(note_count=4, yield_all=True, start_note=Db1):
+...     print(note, end=' ')
+...
+None D¹ None E¹ F¹ None G¹ >>> 
+```
+
+
+
+## fretboard tool
+
+A sample application `fretboard.py` comes built-in with `kord` and gives some insight into the possibilities of the framework. It displays a representation of your instrument's fretboard, tuned to your liking along with note patterns for any given mode (scale/chord) for any given root note. 
+
+If you installed via pip (as opposed to cloning this repo) installation path will depend on your system, it's usually something like `/usr/local/fretboard` or `~/.local/fretboard`. You will also find a `tunings` directory with some pre-defined instrument tunings in the form of .json files. Feel free to modify them or add your own and they should immediately become available to the run-time.
+
+```
+$  python3 fretboard.py --help
+usage: fretboard.py [-h] [-d] [-s  | -c ] [-i] [-t] [-f] [-v] root
+
+<<< Fretboard visualizer sample tool for the kord music framework >>>
+
+positional arguments:
+  root                select key ROOT note
+
+optional arguments:
+  -h, --help          show this help message and exit
+  -d, --degrees       show degree numbers instead of note pitches
+  -s , --scale        major, minor, melodic_minor, harmonic_minor, major_pentatonic, minor_pentatonic,
+                      ionian, lydian, mixolydian, aeolian, dorian, phrygian, locrian, chromatic
+  -c , --chord        maj, min, aug, dim, maj7, min7, 7, dim7, min7dim5, maj9, min9, 9
+  -i , --instrument   banjo, guitar, pedal, bass, ukulele
+  -t , --tuning       check .json files for available options
+  -f , --frets        1, 2, .., 36
+  -v , --verbosity    0, 1, 2
+```
+
+The only required parameter is the `root` note. 
+
+The `--scale` and `--chord` options let you choose which note pattern to display for the selected root. They are mutually exclusive and the default value is `--chord maj` when left blank.
+
+The `--instrument` and `--tuning` options refer to the json files you will find in the tunings directory. Default values are `--instrument guitar   --tuning standard`.
+
+The `--frets` option let's you choose how many frets to visualize, maximum value is 36. Default value will fill your terminal screen.
+
+The `--verbosity` option let's you choose how much information to see on-screen from 0 to 2. Default value is 1.
+
+The `--degrees` option let's you display degree numbers instead of notes. Default value is false.
+
+
+## screenshots
+
+Here are a couple of pics to get you excited:
+
+### chords
+
+![](https://github.com/synestematic/kord/blob/master/resources/e7.png?raw=true)
+
+![](https://github.com/synestematic/kord/blob/master/resources/dim7.png?raw=true)
+
+### scales
+
+![](https://github.com/synestematic/kord/blob/master/resources/penta.png?raw=true)
+
+![](https://github.com/synestematic/kord/blob/master/resources/cs.png?raw=true)
+
+![](https://github.com/synestematic/kord/blob/master/resources/lydian.png?raw=true)
+
+
+Keep on rocking!
```

### Comparing `kord-3.5/README.md` & `kord-3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: kord
+Version: 3.6
+Summary: a framework for programming music applications
+Home-page: https://github.com/synestematic/kord
+Author: Federico Rizzo
+Author-email: synestem@ticATgmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # kord
 kord is a python framework that provides programmers with a simple api for the creation of music-based applications. While it's mainly intended for theoretical purposes, some of it's modules contain functionality specifically tailored for dealing with plucked-string instruments.
 
 ![](https://github.com/synestematic/kord/blob/master/resources/chrom.png?raw=true)
 
 ## installation
```

### Comparing `kord-3.5/app/fretboard.py` & `kord-3.6/app/fretboard.py`

 * *Files identical despite different names*

### Comparing `kord-3.5/app/tuner.py` & `kord-3.6/app/tuner.py`

 * *Files identical despite different names*

### Comparing `kord-3.5/app/tunings/guitar.json` & `kord-3.6/app/tunings/guitar.json`

 * *Files identical despite different names*

### Comparing `kord-3.5/kord/instruments.py` & `kord-3.6/kord/instruments.py`

 * *Files identical despite different names*

### Comparing `kord-3.5/kord/keys.py` & `kord-3.6/kord/keys.py`

 * *Files identical despite different names*

### Comparing `kord-3.5/kord/notes.py` & `kord-3.6/kord/notes.py`

 * *Files identical despite different names*

### Comparing `kord-3.5/kord/tests.py` & `kord-3.6/kord/tests.py`

 * *Files identical despite different names*

### Comparing `kord-3.5/setup.py` & `kord-3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kord",
-    version="3.5",
+    version="3.6",
     author="Federico Rizzo",
     author_email="synestem@ticATgmail.com",
     description='a framework for programming music applications',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/synestematic/kord",
     license="MIT",
```

