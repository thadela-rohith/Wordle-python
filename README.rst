Wordle-Python
=============

A terminal-based clone of the popular Wordle game, built in Python.  
This version has been customized, republished, and enhanced for educational and portfolio purposes by Rohith Vamsi Thadela.

Overview
--------

This project brings the familiar Wordle experience to the command line. It supports multiple game modes, a solver that plays on your behalf, and a helper that provides intelligent word suggestions.

Whether you're looking to sharpen your logic or explore how algorithms can narrow down a word puzzle, this tool demonstrates how Python can deliver engaging interactive applications through a simple CLI.

Features
--------

* Interactive Wordle game playable in the terminal
* Smart solver that auto-plays and demonstrates logic-based guessing
* Helper mode to assist with solving external Wordles
* Random and seeded gameplay for reproducible runs
* Cleanly structured Python code, easy to follow and extend

How to Run
----------

Clone this repository and run the game using Python 3:

.. code-block:: console

    $ git clone https://github.com/thadela-rohith/Wordle-python.git
    $ cd Wordle-python
    $ python wordle.py

Requirements
------------

No external dependencies required. Works with Python 3.6+.

Game Modes
----------

**Default Mode**  
Play a daily Wordle using a fixed word set.

**Random Mode**  
Use the ``--random`` option to play any random word.

**Solver Mode**  
Let the built-in algorithm solve the word for you using ``--solve``.

**Helper Mode**  
Use ``--helper`` to get guided suggestions for solving third-party Wordles (like on NYT).

Example
-------

.. code-block:: console

    $ python wordle.py --helper

    Attempt 1
    =========
    Suggestions: [('raise', 94.3)]
    Chosen word: raise
    Result: 01201

    Attempt 2
    =========
    Suggestions: [('plush', 78.2)]
    Chosen word: plush
    Result: 22222

    Congratulations!

Terminology
-----------

* **Known Letters**: Letters known to be in the word based on feedback
* **Coverage**: Percent of possible solutions a word could eliminate
* **Result String**: Feedback like 20100 → Green, Grey, Yellow, Grey, Grey

Planned Improvements
--------------------

* Colored terminal feedback for better UX
* GUI version using Tkinter or PyGame
* Word frequency–based hint system
* Win streak tracking and player stats

License
-------

This project is distributed under the GNU General Public License v3.0.

Acknowledgements
----------------

Inspired by the original project: `python-wordle by @hrishikeshrt <https://github.com/hrishikeshrt/python-wordle>`_

