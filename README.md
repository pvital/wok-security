# wok-security
Wok rules and artifacts to configure firewall and SELinux.

What is Wok?
============

Wok is a cherrypy-based web framework with HTML5 support originated from Kimchi.
It can be extended by plugins which expose functionality through REST APIs.

Examples of such plugins are [Kimchi](https://github.com/kimchi-project/kimchi/)
(Virtualization Management); [Ginger Base](https://github.com/kimchi-project/gingerbase/)
(Basic host management) and; [Ginger](https://github.com/kimchi-project/ginger/)
(System Administration).

Wok runs through wokd daemon.

Why this project is necessary?
==============================

Wok and its plugins are exposed by HTTP and HTTPS, and some firewall and
SELinux rules are necessary to allow the correct ports and contexts maintaining
the security of the server.

This project offers rules and artifacts to be used or installed by System
Administrator to allow/set the correct rules to provide Wok service to users.
