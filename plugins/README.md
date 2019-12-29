
# Roundcube Plugin: SearchHighlight, and IdentiTeam

<a href="https://github.com/roundcubevnz/roundcube-plugin-searchhighligh/tags"><img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/roundcubevnz/roundcube-plugin-searchhighligh?style=flat-square&logo=github"></a>
<a href="https://github.com/roundcubevnz/roundcube-plugin-searchhighligh/blob/master/COPYING"><img alt="Project license" src="https://img.shields.io/github/license/roundcubevnz/roundcube-plugin-searchhighligh?style=flat-square&"></a>
<a href="https://www.paypal.me/mckaygerhared/5usd" title="Donate to this project using Paypal"><img src="https://img.shields.io/badge/paypal-donate-blue.svg?style=flat-square&logo=paypal" /></a>

Specially search highlight, some useful plugins for roundcube.

* [SearchHighlight](search_highlight): Very simple plugin to highlight the words searched in the messages displayed.
* [IdentiTeam](identiteam): Create new users' identities and fancy signatures, using data from an LDAP server and complex HTML or text templates.

The search_highlight are configless plugin, rest will need setup and customizations.

## Requirements

Only tested this plugin with following environments. Other setup may work with luck.

- PHP: >= `5.4`
- Roundcube: `0.9`,`1.1`,`1.2.8`,`1.3.0`
- Supported skins: `Classic`, `Larry`, `Elastic`


## How to install this plugin in Roundcube


1. Create folder `<pluginname>` in `ROUNDCUBE_HOME/plugins` if it does not exist. Each individual are in [plugin](../plugin) directory in this repository
2. Copy all plugin `<pluginname>` files there.
3. If you want to do plugin configuration, copy `config.inc.php.dist` to `config.inc.php` and then edit `config.inc.php`.
4. Edit your Roundcube's config file (`ROUNDCUBE_HOME/config/config.inc.php` or maybe `/etc/roundcube/config.inc.php`), locate `$config['plugins']` and add `'<pluginname>',`.
5. For detailed info check each [plugin](../plugin) directory in this repository.
