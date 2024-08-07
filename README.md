Photo Application - Dash Python on webview by Enzo
===========
My goal was to find a solution to make an app with Dash(Without a browser).

1) In this code, you will find a way to make an app Dash (Without a browser) with pywebview
2) Make a Stream video App with open-cv and Dash inside a Flask server
3) How to make a .exe from a dash app / flask app
4) Correct a bug from some module after the .exe method => dash_ag_grid

##### To make an .exe #####
# I used autopytoexe.exe after install pyinstaller in my .venv
# I build an onefile .exe
# I didn't find how to use style.css in an external file (In assets...)
# I had to integrate style in my dash components in the code but it works

# I used autopytoexe.exe directly in .venv/Scripts/autopytoexe.exe
# I also got an error with some modules like dash_ag_grid when i opened my .exe after the first compile in an another program
# I got an error with dash_ag_grid, Dash_ag_grid has no hooks.py but it's possible to build without that.
# You just should add in "collect_data" in Advanced Module in autopytoexe.exe=> "dash_ag_grid"

"""
The error was
Traceback (most recent call last):
  File "main.py", line 7, in <module>
  File "<frozen importlib._bootstrap>", line 1360, in _find_and_load
  File "<frozen importlib._bootstrap>", line 1331, in _find_and_load_unlocked
  File "<frozen importlib._bootstrap>", line 935, in _load_unlocked
  File "PyInstaller\loader\pyimod02_importers.py", line 419, in exec_module
  File "dash_ag_grid\__init__.py", line 21, in <module>
FileNotFoundError: [Errno 2] No such file or directory: 'C:\\Users\\Enzo\\AppData\\Local\\Temp\\_MEI212162\\dash_ag_grid\\package-info.json'
"""
