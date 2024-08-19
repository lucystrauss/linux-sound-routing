Python --> JACK --> REAPER

Resources:
https://jackclient-python.readthedocs.io/en/0.5.4/

This code uses the following example as a starting point:
https://jackclient-python.readthedocs.io/en/0.5.4/examples.html#pass-through-client

*Steps to run client-test-just-jack.ipynb:
1) open jackctl, choose sound device settings, click start/play
3) open client-test-just-jack.ipynb
4) run cells up until and including "# STREAM!" block
5) open REAPER**
6) go back to jackctl and route outputs from Python to inputs to REAPER (channel numbers as you wish)
7) in REAPER, set appropriate input and output channels

*To do: automate routing. For now, there are many steps and they must be done in order.

**Before running, make sure you select JACK as audio device in REAPER and that you set enough input and output channels. After doing so, you will need to save your REAPER project, then close REAPER and only open it at the appropriate moment as stated above.

NB sample rates must match in Python, REAPER and any external soundcard thath you may be using.
