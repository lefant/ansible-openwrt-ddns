openwrt-ddns
============

dynamic dns config of your openwrt system.
compare: [http://wiki.openwrt.org/doc/howto/ddns.client]

Role Variables
--------------

there is a nested dict `ddns`. look at tasks and the page above to
understand usage.

you may want to consider `hash_behaviour=merge` in your ansible.cfg

Dependencies
------------

[lefant.openwrt-uci]

Example Playbook
----------------

[https://github.com/lefant/ansible-openwrt/blob/master/openwrt.yml]

Requirements
------------

must be kept minimal as this is supposed to run on openwrt embedded
systems. in particular we try get by with plain POSIX shell, using
neither python nor bash in any way. lua could be an option as that
seems to be the openwrt scripting language of choice.

License
-------

BSD

Author Information
------------------

Fabian Linzberger, [http://e.lefant.net/]



[http://wiki.openwrt.org/doc/howto/ddns.client]: http://wiki.openwrt.org/doc/howto/ddns.client
[lefant.openwrt-uci]: https://galaxy.ansible.com/list#/roles/1645
[https://github.com/lefant/ansible-openwrt/blob/master/openwrt.yml]: https://github.com/lefant/ansible-openwrt/blob/master/openwrt.yml
[http://e.lefant.net/]: http://e.lefant.net/
