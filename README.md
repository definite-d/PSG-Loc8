# PSG-Loc8
A PySimpleGUI extension module that gets the ideal locations for your windows to be.

With this module, doing this:...
```
# I'm using Python 3 here.
import PySimpleGUi as sg
from PSG-Loc8 import Locator
loc8or = Locator(my_reference_window)

some_other_windows_layout = [[sg.Text('Hello World')]]
some_other_window = sg.Window('Some Window', some_other_windows_layout, location=loc8or.get_ideal_location(some_other_windows_layout, 'UC', 'UC'))
```
...will make "some_other_window" appear as though you dragged the center of its titlebar to align with that of "my_reference_window".

Your windows don't have to appear at the center of the screen or at the top left corner of some other window, neither should you waste time with coordinates and vectors.

For a 'real-world', working example, check out LookyFeely:
https://github.com/definite-d/PSG-LookyFeely/
