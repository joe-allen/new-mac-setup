# New Mac Setup

Now that a lot more of folks are working from home, chances are, upgrading to a new computer is liekly in your future. I just took the plunge and purchased a new Macbook Pro (2019) and wanted to document what I did to get it up and running for a modern web development work station.

I would recommend putting a list like this together for your exact setup. This way you're able to get started more quickly next time you need to start fresh.

## code
[x] - Install VSCode

[x] - Install Hyper (port ~/.hyper config from old comp or [read](https://tjay.dev/howto-my-terminal-shell-setup-hyper-js-zsh-starship/))

[x] - Install ZSH (port ~/.zshrc config from old comp or [read](https://github.com/ohmyzsh/ohmyzsh))

[x] - Install Brew

[x] - Install Git

[x] - Install Github Desktop

[x] - Install Node

[] - Install Composer

[] - Install Laravel Valet
  [x] - Install wp-cl

[] - Install [wp-cl + valet](https://github.com/aaemnnosttv/wp-cli-valet-command)
  - If you get a "WP-CLI ran out of memory" error, update the file _/usr/local/etc/php/7.4/conf.d/php-memory-limits.ini_ to be `memory_limit = 1024M` instead of `memory_limit = 512M`
  [] - If mysql is not in you path, you may get an error like _Error: env: mysql: No such file or directory_. Make sure add `export PATH="$PATH:$HOME/.composer/vendor/bin:/usr/local/Cellar/mysql@5.7/5.7.29/bin/"` to you .zshrc or .bashrc file. I would `cd` into `/usr/local/Cellar/` to make sure you have directories _mysql@5.7_ and _5.7.29_ as you might have different versions. (The above export is also putting **Composer** in your path).

[x] - Install MySQL Pro

[] - Install CLI Netlify (`sudo npm install netlify-cli -g`)

[] - Install CLI Maizzle

[] - Install CLI Ionic
  [] - Capicitor requieres install for android studio and Xcode Command Line tools / cocoapods for iOS.

[] - Install CLI Puppeteer

### wordpress / php

[] - `brew install mailhog`

[] - install phpcs
  [] - `curl -OL https://squizlabs.github.io/PHP_CodeSniffer/phpcs.phar`
  [] - `curl -OL https://squizlabs.github.io/PHP_CodeSniffer/phpcbf.phar`
  [] - `composer global require --dev 10up/phpcs-composer:dev-master`
  [] - Install vscode plugin phpcs by Ioannis Kappas
  [] - In _.eslinstrc.json_ extend 10up `{"extends": "@10up/eslint-config"}`
  [] - check installed correctly w/ `phpcs -i` (should see something like: `The installed coding standards are PEAR, Zend, PSR2, MySource, Squiz, PSR1, PSR12, 10up-Default, PHPCompatibility, PHPCompatibilityParagonieRandomCompat, PHPCompatibilityParagonieSodiumCompat, PHPCompatibilityWP, WordPress, WordPress-Extra, WordPress-Docs and WordPress-Core`)

### vscode

[] - Use sublime text shortcuts

[] - Use [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync)


## design

[x] - Install Adobe Creative Cloud

[] - install figma

## productivity

[x] - Install Spotify

[x] - Install Slack

[x] - Install Zoom

[x] - Install Alfred

[x] - Install Magnet

[x] - Install Annotate

[x] - Install Vanilla

## misc

[x] - Install Brave

[x] - Install Chrome (sign in)

[x] - Install Firefox Develeporer Edition

[] - Good workflow [article](https://dev.to/oryanmoshe/i-spend-one-hour-a-week-optimizing-my-development-environment-l9a)

## system settings

[] - Remove uneeded apps in doc

[] - Set up hotcorners [tl: desktop, tr: mission control, br: launchpad, bl: sleep]

[] - Add bluetooth icon to toolbar

