Digital Ocean Dynamic DNS-Updater
=================================

Purpose:
--------
Allows the dynamic updating of an 'A' or 'AAAA' record that is managed by Digital Ocean's DNS servers.

Usage:
------
Provide your API key, the domain you want to update and the 'Record' for that domain and schedule the script to run however
often you want (using, for example, the Windows Scheduler or a cron job).


Example Usage:
--------------
The PHP script has been designed to be called as a command line tool. Config is passed into it in the form of CLI parameters, for example:

    php updater.php accessToken domain record recordtype

    python updater.py accessToken domain record recordtype

where 'accessToken' is your ['Personal Access Token'](https://cloud.digitalocean.com/settings/applications), 'domain' is the domain name you want to update
(e.g: example.com), 'record' is the value of the record you want to update (e.g: home), and 'recordtype' is either A or AAAA.

