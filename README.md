##SERVER SETUP

This is ansible for easier set-up of my server if something bad happens.

Server contains:

1. Small tools for testing and other stuff.
2. Factorio server with service file.
3. Minecraft server with service and socket file.
   Minecraft server is runned by accessing to socket.

##HOW TO

To use this you must do these steps:

1. Replace all *\<user\>* in ``packetseekers-playbook.yml`` with username of
   the administrator account on a server.
2. Add ``minecraft`` and ``factorio-server`` folders from backup to
   ``./srv/games/`` folder.
3. Install ansible and create hosts group home-server in ``/etc/ansible/hosts``
   file.
4. Run ``ansible-playbook -K packetseekers-playbook.yml`` (you can use ``-C``
   for dry-run first).

