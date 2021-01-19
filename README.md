# dokku-php-newrelic
Inject Newrelic dpkg in container.

dokku-php-newrelic is a plugin for [dokku][dokku] that installs PHP Newrelic in your dokku environment.

## Installation
On your dokku server:

### dokku >= 0.4.0
```sh
sudo dokku plugin:install https://github.com/CreativeGS/dokku-php-newrelic
```

## Usage
When you deploy your project, the dokku-php-newrelic plugin will install Newrelic, provided you have set needed config.

## Configuration
Installer uses environmental variables to set Newrelic license and app name.

```
NEW_RELIC_ENABLED="true" # must be set for plugin to even attempt installation
NEW_RELIC_LICENSE_KEY="Your Newrelic license" # something like "8ae8e02b0d25abce858301dx14f6946fe6d87ba1f"
NEW_RELIC_APP_NAME="You App Name" # something like "Basecamp"
```

[dokku]: https://github.com/progrium/dokku
