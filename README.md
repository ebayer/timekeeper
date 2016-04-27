timekeeper
==========

Automated Time Tracker for Linux

The objective of this project will be to track the active window in order to apply some automated rules to determine the personal usage profiling on desktop applications. This will allow a person to see how much time he/she spends using each program.

There are some other projects like this:
* [Arbtt][1]
* [Window-title][2]
* [Wakoopa][3]
* [RescueTime][4]

All projects on this subject fall short on the following:
* There are two approaches that can be used: Sampling (Polling) and event-driven information gathering. Event-driven approach is better because sampling does not produce very accurate results.
* There is no support for cryptography. Personal information is not protected properly.
* There is no support for cloud storage. All of the mentioned software uses either local files or their own infrastructure to store the information.
* In order to properly deduce some useful information on usage statistics, we have to present the results in most useful graphical representation. Dumping all information onto a terminal screen is not very user-friendly.

This project will use an event-driven approach to properly log the active window usage into a file, with the option of encryption and storing the information on personal cloud storage systems like dropbox, google-drive, spideroak. It will then use the collected information to present the usage statistics on a graph using charts, bars, etc.

In order to develop this application, one will need to have beginner level understanding on the following subjects:
* Python
* X Window system python bindings (xpyb and [xpybutil][5])
* Using cryptography in python
* Using external APIs

[1]: http://hackage.haskell.org/package/arbtt
[2]: https://github.com/abyrd/window-title
[3]: http://wakoopa.com/
[4]: https://www.rescuetime.com/
[5]: https://github.com/BurntSushi/xpybutil
