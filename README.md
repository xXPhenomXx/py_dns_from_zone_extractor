py_dns_from_zone_extractor
==========================

Python script to extract DNS entries from zone files

Language: Python
Date Created: 10-31-12
Dependencies: dnspython & easyzone

Description:
This script will iterate through a directory full of zone files, extract all of the DNS entries
and write those DNS records into a CSV file for analysis.

Use Case:
We host 6,000 plus sites and store our DNS entries for each site in a database.
At some point our database became corrupt and we lost some data, the DNS records in the table where no longer reliable. This
became an issue when we had to move to another Registrar and they requested all of the DNS records in a CSV so they could
import on their end.

The only reliable source of info was the actual zone files itself. This script will open each zone file and extract the DNS records
in the zone file and write to the CSV.

This is open-source and free for any use or modification you see fit.

Any questions, comments, or bugs feel free to drop me a line.
jassen.michaels@gmail.com