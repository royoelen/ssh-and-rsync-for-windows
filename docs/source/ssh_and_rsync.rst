SSH and rsync setup
===================

.. _ssh_and_rsync_setup:

install git for windows
https://github.com/git-for-windows/git/releases/tag/v2.37.2.windows.2

download the zip file containing the libraries and executables
https://drive.google.com/file/d/1knjsRweAcUXCPFJMFnxCbH1ilDL0MpAZ/view?usp=sharing

unzip the files

Then, for all three folders, copy the usr folder in each of the three folders, to C:\Program Files\Git\, or any other place that git for windows was installed. (This might be in appdata for UMCG laptops)

From this point on, you can use 'git bash' program to open a terminal, which supports the use of the ssh and rsync commands, and this terminal will in that regard act the same as the terminal would on Linux or Mac OSX

Next, we can try to connect to the gearshift cluster :doc:`connecting_to_gearshift`

.. autosummary::
   :toctree: generated

