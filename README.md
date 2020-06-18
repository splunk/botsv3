# Boss of the SOC (BOTS) Dataset Version 3
A sample security dataset and CTF platform for information security professionals, researchers, students, and enthusiasts. This page hosts information regarding the version 3 *dataset*. If you would like access to the scoreboard software, please visit [the CTF Scoreboard Github repository](https://github.com/splunk/SA-ctf_scoreboard). If you are looking for the BOTS version 2 dataset, it can be found [here](https://github.com/splunk/botsv2). If you are looking for the BOTS version 1 dataset, it can be found [here](https://github.com/splunk/botsv1).

## Download

| Dataset          | Description | Size | Format | MD5 |
| ---------------- | ----------- | ---- | ------ | --- |
| [BOTS V3 Dataset](https://botsdataset.s3.amazonaws.com/botsv3/botsv3_data_set.tgz) |  BOTSv3 dataset. | 320.1MB | Pre-indexed Splunk | d7ccca99a01cff070dff3c139cdc10eb |


## Installation
1. Download the dataset file indicated above and check the MD5 hash to ensure integrity.
2. Install Splunk Enterprise and the apps/add-ons listed in the *Required Software* section below. It is important to match the specific version of each app and add-on.
3. Unzip/untar the downloaded file into $SPLUNK_HOME/etc/apps
4. Restart Splunk
5. The BOTS v3 data will be available by searching:
```
index=botsv3 earliest=0
```
6. Note that because the data is distributed in a pre-indexed format, there are no volume-based licensing limits to be concerned with.

## Data Sourcetypes included
* access_combined
* alternatives
* amazon-ssm-agent
* amazon-ssm-agent-too_small
* apache_error
* aws:cloudtrail
* aws:cloudwatch
* aws:cloudwatch:guardduty
* aws:cloudwatchlogs
* aws:cloudwatchlogs:vpcflow
* aws:config:rule
* aws:description
* aws:elb:accesslogs
* aws:rds:audit
* aws:rds:error
* aws:s3:accesslogs
* bandwidth
* bash_history
* bootstrap
* cisco:asa
* cloud-init
* cloud-init-output
* code42:api
* code42:computer
* code42:org
* code42:security
* code42:user
* config_file
* cpu
* cron-too_small
* df
* dmesg
* dpkg
* error-too_small
* errors
* errors-too_small
* ess_content_importer
* hardware
* history-2
* interfaces
* iostat
* lastlog
* linux_audit
* linux_secure
* localhost-5
* lsof
* maillog-too_small
* ms:aad:audit
* ms:aad:signin
* ms:o365:management
* ms:o365:reporting:messagetrace
* netstat
* o365:management:activity
* openports
* osquery:info
* osquery:results
* osquery:warning
* out-3
* package
* perfmonmk:process
* protocol
* ps
* script:getendpointinfo
* script:installedapps
* script:listeningports
* stream:arp
* stream:dhcp
* stream:dns
* stream:http
* stream:icmp
* stream:igmp
* stream:ip
* stream:mysql
* stream:smb
* stream:smtp
* stream:tcp
* stream:udp
* symantec:ep:agent:file
* symantec:ep:agt_system:file
* symantec:ep:behavior:file
* symantec:ep:packet:file
* symantec:ep:risk:file
* symantec:ep:scm_system:file
* symantec:ep:security:file
* symantec:ep:traffic:file
* syslog
* time
* top
* unix:listeningports
* unix:service
* unix:sshdconfig
* unix:update
* unix:uptime
* unix:useraccounts
* unix:version
* userswithloginprivs
* vmstat
* who
* wineventlog
* winhostmon
* xmlwineventlog:microsoft-windows-sysmon/operational
* yum-too_small


## Required Software
The dataset requires the following software which is distributed and licensed separately
and should be installed before using the dataset. The versions listed are
those that were used to create the dataset. Different versions of the software
may or may not work properly. If you are new to Splunk, follow [these instructions](http://docs.splunk.com/Documentation/Splunk/latest/Installation/Whatsinthismanual) to install the free Splunk Enterprise trial and [these instructions](https://docs.splunk.com/Documentation/AddOns/released/Overview/Singleserverinstall) to install apps and add-ons.


|	App / Add-on	|	Version	|	Download
| ----------- | ------- | -------- |
| Splunk Enterprise                               | 7.1.7 | http://www.splunk.com
|	Aws_guardduty	                                  |	1.0.4	|	https://splunkbase.splunk.com/app/3790/
|	CiscoNVM	                                      |	1.0.346	|	https://splunkbase.splunk.com/app/2992/
|	Code42 App For Splunk	                          |	3.0.6	|	https://splunkbase.splunk.com/app/3736/
|	Code42ForSplunk Technology Add-On	              |	3.0.4	|	https://splunkbase.splunk.com/app/3746/
|	Splunk Add-on for Cisco ASA	                    |	3.3.0	|	https://splunkbase.splunk.com/app/1620/
|	Splunk Add-on for Microsoft Cloud Services	    |	2.1.0	|	https://splunkbase.splunk.com/app/3110/
|	Splunk Add-on for Microsoft Office 365	        |	1.0.0	|	https://splunkbase.splunk.com/app/4055/
|	Splunk Add-on for Microsoft Windows	            |	4.8.4	|	https://splunkbase.splunk.com/app/742/
|	Splunk Add-on for Symantec Endpoint Protection	|	2.3.0	|	https://splunkbase.splunk.com/app/2772/
|	Splunk Add-on for Tenable	                      |	5.1.3	|	https://splunkbase.splunk.com/app/1710/
|	Splunk Add-on for Unix and Linux	              |	5.2.4	|	https://splunkbase.splunk.com/app/833/
|	Splunk Common Information Model	                |	4.11.0	|	https://splunkbase.splunk.com/app/1621/
|	Splunk Security Essentials	                    |	2.2.0	|	https://splunkbase.splunk.com/app/3435/
|	Splunk Stream Add-on	                          |	7.1.2	|	https://splunkbase.splunk.com/app/1809/
|	TA-VirusTotalActions	                          |	0.2.0	|	https://splunkbase.splunk.com/app/3446/
|	URL Toolbox	                                    |	1.6	  |	https://splunkbase.splunk.com/app/2734/
|	DecryptCommands	                                |	2	|	https://splunkbase.splunk.com/app/2655/
|	Microsoft Azure Active Directory Reporting Add-on for Splunk	|	1.0.1	|	https://splunkbase.splunk.com/app/3757/
|	Microsoft Cloud App for Splunk	                |	1.0.1	|	https://splunkbase.splunk.com/app/3786/
|	Microsoft Office 365 Reporting Add-on for Splunk  |	1.0.1	|	https://splunkbase.splunk.com/app/3720/
|	Microsoft Sysmon Add-on	                        |	8.0.0	|	https://splunkbase.splunk.com/app/1914/
|	OSquery App for Splunk	                        |	0.6.0	|	https://splunkbase.splunk.com/app/3902/
|	Splunk Add-on for AWS	                          |	4.5.0	|	https://splunkbase.splunk.com/app/1876/
|	ES Content Updates	                            |	1.0.25	|	https://splunkbase.splunk.com/app/3449/
|	SA-cim_vladiator	                              |	1.2	|	https://splunkbase.splunk.com/app/2968/


## Warning
**Please be advised that this dataset may contain profanity, slang, vulgar expressions, and/or generally offensive terminology. Please use with discretion.**

This dataset contains evidence captured during actual computer security incidents, or from realistic lab recreations of security incidents. As such, the dataset **may** contain profanity, slang, vulgar expressions, and/or generally offensive terminology. The authors believe that the educational benefits of preserving the realism of the dataset outweigh the risk of offending some users. If the possibility of encountering this type of offensive material is a concern to you or to any audience with whom you plan to share the dataset, please stop now and do not continue.

## Authors
Written in 2018 by Ryan Kovar, David Herrald, James Brodsky, John Stoner, Jim Apger, David Veuve, Lily Lee, and Matt Valites

## Copyright and License
To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to this software to the public domain worldwide. This software is distributed
without any warranty. You should have received a copy of the CC0 Public Domain Dedication along with this software. If not, see http://creativecommons.org/publicdomain/zero/1.0/.

