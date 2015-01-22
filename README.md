# PwAuth authentification plugin for MediaWiki

This plugin will provide authentification against both MediaWiki users and system users using PwAuth.

Two sources authentication works because of MediaWiki's default fallback behaviour. If a user doesn't exist in /etc/passwd, it automatically tries to 
authenticate against its own users. This is accomplished by returning false on ->strict().

Dependency: PwAuth (binary located in /usr/local/sbin/pwauth with setuid root flag, Version 2.3.10)
