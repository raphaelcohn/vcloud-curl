vcloud-shell
===========
A shell, called vsh, based on curl, for mixing API calls to vCloud providers (such as Terremark and Skyscape) and general bash syntax.

Provides a script syntax (.vsh files) that can execute a sequence of commands.

Uses good ol'fashioned netrc files for managing credentials securely. Works properly with proxies, using curlrc files.


vCloud Curl Tools

* USE BASH_CMDS to replace the use of .path?
* consider integration with logger, so we can start doing some audit recording
* refactor metadata API calls for media into common code
* implement downloads_last
* exit / exitError / informationMessage FAIL
* capture versions and sessions in special download and captures?
* support CentOS and Debian paths
* support background downloading of OVF

* FIX METADATA format (eg org-metadata)
* FIX task formatting - seems broken for enableDownload?

##examples
demonstrate more functionality - especially all the possible formats for each api call
find a way to validate formats
refactor formats

## unrecorded downloads
vdc/vAppTemplate/ download and enableDownload
vdc/media/metadata/* (incl getValue, which could be cached, but might not be appropriate)

* records and queries
	* references / records / idrecords for EdgeGateways
	* ditto for /api/query