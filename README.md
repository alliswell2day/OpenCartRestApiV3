# OpenCartRestApiV3
GSS Opencart Rest API gateway for Opencart3.0

# README / INSTALLATION  #

This extension is provided on a as-is basis.

Installation is at your own risk.

The package may be updated from time to time, and these upgrades may break this particular version. You will be required to update.

###ENSURE YOU BACKUP YOUR SITE BEFORE INSTALLING THIS ###

### IT IS RECOMMENDED THAT YOUR GET YOUR WEBSITE ADMIN TO REVIEW THE FILES TO ENSURE IT DOES NOT CONFLICT WITH ANY EXISTING EXTENSIONS ###

Clone this repository and upload the files to your server.

You will notice that the folders are in the same structure as your Opencart installation.

1. Navigate to your opencart root folder using an FTP program
2. Upload the "catalog" & "admin" folder to your opencart installation folder
3. Go to your admin area in Extensions->Product Feeds and enable your GSS API extension
   You have to fill the security key field. We recommend you use a strong random password of at least 16 characters (eg. JRALdQMbrtx4cWr2y)
   This key is then required on GoSweetSpot configuration.

If you encounter an error while enabling the extension, you may need to apply the following permission changes:
```
(chmod 755 admin/controller/extension/feed/gss_api.php)

(chmod 755 admin/language/en-gb/extension/feed/gss_api.php)

(chmod 755 admin/view/template/extension/feed/gss_api.twig)

(chmod 755 catalog/controller/extension/feed/gss_api.php)

(chmod 755 catalog/model/account/gss_order.php)
```
