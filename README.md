S3 compatible Object Storage Volume for Craft CMS
==============================================

This is a fork from [https://github.com/fortrabbit/craft-object-storage](https://github.com/fortrabbit/craft-object-storage). I had to make some changes to update dependencies and to work with other S3 service. 

## Requirements

This plugin requires Craft CMS 4.0 and PHP 8.0 or later. 


## Installation

To install the plugin, follow these instructions.


**1. Install the plugin via composer**

```
cd /path/to/project

composer require performing/craft-object-storage
```

**2. Update your local .env file** 
```
S3_BASE_URL=https://xxxxx.example.com/path
S3_ACCESS_KEY_ID=...
S3_SECRET_ACCESS_KEY=...
S3_ENDPOINT=https://xxxxx.example.com
S3_REGION=...
S3_BUCKET=...
```


**3. Install the plugin**
```
./craft plugin/install performing-object-storage
```

Or browse to  CP > Settings > Plugins to enable the plugin.


**4. Configure**

Configure volumes under: Settings > Assets > **[New Volume]**.  

Select `S3 Compatible Object Storage` as Volume Type and for the Base URL field use `$OBJECT_STORAGE_HOST` ENV variable. 
All other fields are pre-configured with ENV vars already. 


