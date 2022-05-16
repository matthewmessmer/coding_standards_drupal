# Drupal Code Standards

A fork of nilswloewen/drupal_code_standards - see https://blog.acromedia.com/making-drupal-code-standards-work-for-you-with-phpstorm-phpcs-phpcbf for the initial thinking of this.

## Quick Setup

### Install

```bash
git clone git@github.com:matthewmessmer/drupal_code_standards.git
cd drupal_code_standards
composer install
```

### Set PATH

```
export PATH=$PATH:~/PATH/TO/drupal_code_standards/vendor/bin
```

### Configure PhpStorm inspections

**Must be done on a per-project basis!**

#### Register phpcs and phpcbf as PHP Quality Tools. 

Settings | PHP | Quality Tools | PHP_CodeSniffer

Click the ellipses to set the path to `~/PATH/TO/drupal_code_standards/vendor/bin` for the Local configuration.

#### Enable the inspection.

Settings | Editor | Inspection | PHP | Quality Tools

* Set the extension list to: `php,module,inc,install,test,profile,theme,css,info,yml`

* DO NOT set the "Installed standard paths"

* Choose "Drupal" Coding Standard. Close and reopen preferences window if it does not appear in the dropdown list.

* Click OK and code inspections should be working!