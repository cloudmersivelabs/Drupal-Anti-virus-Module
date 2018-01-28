About this module
-----------------

This module integrates with the anti-virus scanner Cloudmersive Antivirus.
Upload files are forwarded to the Cloudmersive Antivirus service and checked. Infected files
are blocked in the validation routine, so they cannot be saved.


Prerequisites
-------------

This module requires a Cloudmersive Antivirus service.

Sign up for a free API key at https://cloudmersive.com - free keys include 50,000 API calls/month.


Setup
-----

- Install a ClamAV service.
  For example: `sudo apt-get install clamav-daemon`

- Enable this module.

- Configure the module at /admin/config/media/clamav.
  The unix-socket daemon mode is quickest, but the ClamAV daemon must run on
  the same host as the web server. TCP/IP daemon mode may be best for a
  clustered web service. Executable mode is slowest but simplest.

