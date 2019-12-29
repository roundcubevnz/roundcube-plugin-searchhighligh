# Roundcube Plugin: identiteam

Automatically creates new users' identities on first login, using LDAP fields.

This creates the user identities from a LDAP working server and not from the first login to roundcube's interface, 
**that automate all the user personal settings configuration on the identity**!

* Fully customizable HTML or text signatures.
* Automatically detect signatures types (HTML or text) when created.
* You can use custom signatures per domain.
* You can use custom signatures per user.
* Templates directory location is customisable, for instance '/etc/roundcube/templates'

**NOTE IMPORTANT**: roundcube has now the personal signature with html forms, that make almost same of this plugin.

## Requirements

Only tested this plugin with following environments. Other setup may work with luck.

- PHP: >= `5.4`
- Roundcube: `0.9`,`1.0.X`,`1.1`,`1.2.8`

# Bugs & Issues:

Only bug reports with solution, currently this are working for us: enter bug reports in https://github.com/roundcubevnz/roundcube-plugin-searchhighligh/issues

# Installation:

1. Copy this directory `identiteam` in `ROUNDCUBE_HOME/plugins` from this repository
2. Copy from the copied directory the file `config.inc.php.dist` to `config.inc.php`.
3. Edit `config.inc.php`, the settings have comments to help configuring the plugin.
4. Edit Roundcube's config file (`ROUNDCUBE_HOME/config/config.inc.php`, locate `$config['plugins']` and add `'identiteam',`.

Templates customisation on a global level:
* copy the 'default' directory into a directory representative of your company, for instance "SnakeOil"
* Modify 'folderName' in the config, and use 'SnakeOil' instead of default.

Templates customisation on per domain basis
* Modify 'folderName' in the config, and use '%d' instead of default.
* Create a directory for each domain name you hosts, and copy the file 'default.tmpl' into these directories
* Customise each signature.

## Donate

<a href="https://github.com/roundcubevnz/roundcube-plugin-searchhighligh/tags"><img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/roundcubevnz/roundcube-plugin-searchhighligh?style=flat-square&logo=github"></a>
<a href="https://github.com/roundcubevnz/roundcube-plugin-searchhighligh/blob/master/COPYING"><img alt="Project license" src="https://img.shields.io/github/license/roundcubevnz/roundcube-plugin-searchhighligh?style=flat-square&"></a>
<a href="https://www.paypal.me/mckaygerhared/5usd" title="Donate to this project using Paypal"><img src="https://img.shields.io/badge/paypal-donate-blue.svg?style=flat-square&logo=paypal" /></a>
