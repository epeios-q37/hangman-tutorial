# Modern exercises for programming tutorials, based on the [Hangman game](https://q37.info/s/gtdtk4hp).

[![Hangman](https://q37.info/s/pnmjfw39)](https://q37.info/s/jtdqjsx7)

- **The purpose of this repository is (currently) to serve as proof of concept**.
- **It is under development (contributions welcome)**.
- **Some exercises may need to be switched and will probably be switched in the final version**.
- **It is however fully functional.**

This project shows a new type of exercises for programming tutorials. It only contains the exercises, not (yet?) a complete tutorial.

Each exercise consists to program a feature of the [Hangman game](https://q37.info/s/gtdtk4hp). With the last exercise, the game will be fully operational. The finished game can be see at this address: <https://q37.info/s/jtdqjsx7>.

Nowadays, almost all young people have a smartphone, so they are used to graphical interfaces. They rarely, if ever, had to deal with a text console. Writing programs with a textual interface may be (falsely) considered outdated. This is why all the exercises provided by this project have a web interface, unlike the exercises usually provided with programming tutorials, which almost always have only a text-based interface. 

When one of the exercises of this project is launched, a web browser will automatically be opened to give access to its interface, which you can see in the above picture. To make testing easier, there will also be a text box that displays the word to guess, and in which you can also enter the word to guess. Of course, this text box will not be available in the final version of the game.

The application for a given exercise can also be opened on any device connected to the Internet, by using the URL used by the browser. This is facilitated by the [QR code](https://q37.info/s/3pktvrj7) displayed in the web browser, which can be scanned by a smartphone.

The `en` folder contains the English version of the exercises, and the `fr`, the French one. To adapt the exercises to another language, create a sub-folder in the `workshop` folder, like the `en` or `fr` folder, retrieve the content of one of this folder, and adapt this content to the desired language.

The content of the `en` or `fr` folder located in the root folder should **not** be provided to the students, as they contain an example of the solution of the exercises, and are intended to help the teachers to give to their students all the information they need to complete the exercises. Only the `workshop` folder should be provided, along with both ZIP files.

To begin, the students will create a file with following content:

English version:

```python
# coding: utf-8

import sys
sys.path.append(".")
from workshop.en.a import *

def isLetterInWord(letter,word):

go(globals())

```

French version (note the `fr` in the `from workshop.fr.a import *` line):

```python
# coding: utf-8

import sys
sys.path.append(".")
from workshop.fr.a import *

def lettreEstDansMot(lettre,mot):

go(globals())
```

The first exercise consists in implementing the `isLetterInWord(…)` (*fr*: `lettreEstDansMot(…)`) function. As mentioned above, the teacher will use the content of the (`en`/`fr`)`/a.py` file to give to the students all the instructions they need to complete the exercise.

Once this first exercise is completed, the students will be instructed to replace the `a` in `from workshop.en.a import *` (*fr*: `from workshop.fr.a import *`) with a `b` to obtain `from workshop.en.b import *` (*fr*: `from workshop.fr.b import *`), and also to add following function declaration:

English:

```python
def getMask(word,guesses)
```

French:

```python
def obtenirMasque(mot,pioches)
```

This is how the modified file looks like:

English:

```python
# coding: utf-8

import sys
sys.path.append(".")
from workshop.en.b import *

def isLetterInWord(word,guesses):
# Whatever the student wrote for the previous exercise.

def getMask(word,guesses):

go(globals())
```

French:

```python
# coding: utf-8

import sys
sys.path.append(".")
from workshop.fr.b import *

def lettreEstDansMot(mot,pioches):
# Whatever the student wrote for the previous exercise.

def obtenirMasque(mot,pioches):

go(globals())
```

To tell the students what to do, the teachers will also look at the (`en`/`fr`)`/b.py` file.

And so on for the *c*, *d*, *e*… exercises (when available).

Once an exercise is completed, the teachers will probably have to introduce the concepts that will be relevant for the next exercise. For this purpose, another set of exercises is being developed and can be find here: <https://q37.info/s/tpkx4cfk>.
