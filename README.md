# Couchbase Cartridge

This is just an example OpenShift v2 Couchbase Cartridge Example. It allows you the following:

## Features

* Install Script
  * Download Couchbase Server 3.0.2 and the OpenSSL dependencies to your Application
  * Perform a single node non-root installation of Couchbase Server 3.0.2 to your application root directory
  * Start Couchbase Sever

* Post Install Script
  * Set server node name
  * Set the default index path
  * Set the default data path
  * Set the admin user name to a default value
  * Set the admin password to a default value
  * Set the admin port to a default value
  * Set the memory quota to a defualt value
  * Keep the 'default' bucket

* Control Script
  * Start the single Couchbase Server instance
  * Stop the single Couchbase Server instance
  * Restart the single Couchbase Server instance
  * Get the status of the Couchbase Server Installation

## How to install this Cartridge to your Application

* E.G. Create a sample application based on Node.js
```
rhc app create $app_name nodejs-0.10
```

* Install the cartridge

For OpenShift Online:

```
rhc add-cartridge https://raw.githubusercontent.com/dmaier-couchbase/cb-cartridge/master/metadata/manifest.yml -a $app_name
```

For OpenShift Enterprise follow the following article: https://access.redhat.com/documentation/en-US/OpenShift_Enterprise/2/html/Administration_Guide/Installing_and_Removing_Custom_and_Community_Cartridges.html
