# Couchbase Cartridge Example

This is just an example OpenShift v2 Couchbase Cartridge Example. It allows you the following:

## Features

* Install Script
** Download Couchbase Server 3.0.2 and the OpenSSL dependencies to your Application
** Perfrom a non-root installation of Couchbase Server 3.0.2 to your Application Root directory
** Start Couchbase Sever

* Post Install Script
** Set Server Node Name
** Set the default index path
** Set the default data path
** Set the Admin user name to a default value
** Set the Admin password to a default value
** Set the Admin port to a default value
** Set the Memory Quota to a defualt value
** Keep the 'default' bucket

* Control Script
** Start Couchbase Server
** Stop Couchbase Server
** Restart Couchbase Server
** Get the status of the Couchbase Server Installation

## How to install this Cartridge to your Application

rhc add-cartridge https://raw.githubusercontent.com/dmaier-couchbase/cb-cartridge/master/metadata/manifest.yml -a $app_name


