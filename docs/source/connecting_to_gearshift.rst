connecting to Gearshift
=======================

.. _connecting_to_gearshift:

After setting up rsync and ssh, you can set up everything to connect to the cluster.

I assume you have an ssh key called id_rsa (default) in your .ssh folder already, if not, create one using the git bash window

.. code-block:: console

   ssh-keygen -t rsa -f ~/.ssh/id_rsa -C your_username -b 2048


make sure you have an ssh key, and add that to the ssh agent, in a git bash window.

.. code-block:: console

   eval $(ssh-agent -s)
   ssh-add ~/.ssh/id_rsa


now copy the config file from the zip you extracted, to where your .ssh is (on UMCG laptops, you need to make that folder on the H drive)
and modify the username to be yours instead of the one that is currently in the config file (search and replace in notepad++ does wonders here)

next create a directory called ‘tmp’ in the same directory that houses the .ssh one (not ín the .ssh one)

exit the git bash window using exit, and then open it again

if you created a new SSH key, be sure to send the helpdesk the public key, so you can get access to the cluster

after the key has been added, or if the key was already added before, you can access the cluster just like a Mac or Linux user would

.. code-block:: console
  
  ssh airlock+gearshift
  
  
and rsync just like a Mac or Linux user would

.. code-block:: console
  
  rsync -a airlock+gearshift:/where/the/the/files/are/ /where/you/want/them/locally/


.. autosummary::
   :toctree: generated
