# Changelog

## 0.1.13 - 2020-07-31

### Add
- Add hints for database tables (table exists, column exists)
### Change
- Fix typo in banner.  ( close #6 )
- updated tests


## 0.1.12 - 2020-07-25

### Add
- When a check is not working properly, some hints are now displayed.
- Add hints for database connection
- Add hints for HTTP connections

## 0.1.11 - 2020-07-12

### Add

### Change
- Improved list of languages;
- Update readme

## 0.1.10 - 2020-06-25

### Add
New function for check files.
- check .env file
- check language storage
- list languages available

## 0.1.9 - 2020-06-18

### Add

New runtime config about some paths:

* "langPath" =>"Path to the language files",
* "publicPath" =>" Path to the public / web directory",
* "storagePath" => "Storage directory",
* "resourcePath" =>"Resources directory",
* "getCachedServicesPath" => "Path to the cached services.php",
* "getCachedPackagesPath" => "Path to the cached packages.php",
* "getCachedConfigPath" => "Path to the configuration cache",
* "getCachedRoutesPath" => "Path to the routes cache",
* "getCachedEventsPath" => "Path to the events cache file",
* "getNamespace" => "Application namespace"

## 0.1.8 - 2020-06-18

### Add

:nail_care: Style output table via --style option. You can choose one of these styles (box-double is the default used by LaraLens):
* default
* borderless
* compact
* symfony-style-guide
* box
* box-double

:eyeglasses: Runtime config:
* environmentPath
* environmentFile
* environmentFilePath

### Change

* Refactor for App::"function"()
* update tests
* update readme
* update help (-h)

## 0.1.7 - 2020-06-16

### Add

Database connection:
* connection name
* getQueryGrammar
* getDriverName
* getDatabaseName
* getTablePrefix
* database server version

Runtime configuration:
* Laravel version
* PHP version

## 0.1.6 - 2020-06-01

### Add

* Add show option --show (all|config|runtime|connection|database|migration)

## 0.1.5 - 2020-05-29

### Improve

* managing a better output
* extracting long message from tables
* settings width for columns tables


## 0.1.4 - 2020-05-28

### Fix

* Catch HTTP connection exception

## 0.1.3 - 2020-05-27

### Add

* detect DB connection type
* get tables for mysql
* get tables for sqlite
* count and retrieve last row from a table. Table and column name are as input parameters
* test database diagnostics
* update readme for documentation


## 0.1.2 - 2020-05-22

### Add

* Add new argument as input (it is optional):
    - overview: you can see configuration, http connection, db connection etc
    - allconfigs: you can see verbose configuration from Laravel application. Try to use 'php artisan laralens:diagnostic allconfigs' in your laravel application. You will see the dump of all configuration parameters in json format

## 0.1.1 - 2020-05-22

### Add

* Add runtime config:
    * App::getLocale()
    * App::environment())
    * Generated url via asset() and url() helpers
* Invoke migrate:status

## 0.1.0 - 2020-05-21

* :tada: initial release
* Add laralens:diagnostic artisan command (Laraval)
* Check config parameter like app.url, app.locale, app.url and database.*
* Check the http connection with app.url defined in base configuration
* Check the connection with DB and counts the row for a specific table (users by default)
