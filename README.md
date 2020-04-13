# German Macedonian Dictionary

This repo contains a ready-to-install Apple Dict for MacOS to be used with the built-in Dictionary app. 

The Apple Dict is contained in `data/Deutsch - Mazedonisch.dictionary`.

Alternatively, you can generate the Apple Dict from the source data (`data/Deutsch - Mazedonisch.csv`). To do so, follow these steps:
* Install (pyglossary)[https://github.com/ilius/pyglossary]
  * Clone the repo
  * Install necessary libraries, i.e. run `sudo pip3 install lxml beautifulsoup4 html5lib`
* Run:
    ```
    python3 ~/<PATH_TO_PYGLOSSARY>/main.py --write-format=AppleDict Deutsch\ -\ Mazedonisch.csv Deutsch\ -\ Mazedonisch
    cd Deutsch\ -\ Mazedonisch
    make
    make install
    ```
    This will install the dictionary in `~\Library\Dictionaries`
