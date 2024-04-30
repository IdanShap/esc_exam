
### Instructions:
Each of the  questions below, simulate a ticket first response.
All the questions below can be solved by the provided information - without the need to ask the customer for more information / files.
Your answers to these questions must be in a format of an email to the customer.
You must explain the solution, like you would explain it to a customer.


# IDA section:
#### **Question 1:** 
A customer opened the following ticket - What is the MOST likely cause for the issue? (configuration wise) - you must provide a solution in your first email.

Hello Support,
We have configured Identity Broker according to the Admin guide between 2 of our GWs.
The GWs are managed by different Management servers.
On the publisher GW, the user matches Identity based rules, but on the subscriber GW the user does not match Identity based rules.
Below you will found the broker config from our publisher and subscriber:

The publisher:
```
(
  :sharing_id (k3124gb234k234khbkj22jkjkhg3)
  :identity_subscribers (
    : (
      :Name (SubscriberGW)
      :sharing_id (k2gb2345jkgbjk235gbjk235gjk)
      :ipaddr (192.168.20.1)
      :certificate_subject ("<for the question purpose, this field is correct>")
    )
  )
)
```

The subscriber:
```
(
  :sharing_id (k2gb2345jkgbjk235gbjk235gjk)
  :identity_publishers (
    : (
      :Name (PublisherGW)
      :sharing_id (k3124gb234k234khbkj22jkjkhg3)
      :ipaddr (IP_ADDRESS_OF_INTERFACE_ON_PUBLISHER_GATEWAY_1)
    )
  )
)
```



#### **Question 2:** 
A customer opened the following ticket - What is the MOST likely cause for the issue ?(configuration wise) - you must provide a solution in your first email.

Hello Support,
We are trying to move from RC4 encryption to AES256 encryption in Kerberos.
We followed sk111945 in order to enable it, but now the Identity Agents are not able to connect automatically, and they display the user & password window.
If we switch back to RC4 encryption it works again.
What may cause this issue? please assist us.


#### **Question 3:** 
A customer have opened the following ticket, assist him to achieve his goal - you must provide a solution in your first email.

Hello Support,
We are using Cisco VPN, but we do not have Cisco ISE.
From looking at checkmates, we have seen that it is possible to configure Cisco VPN to send Syslog messages to the Identity Collector, and create a parser for Login, and Logout events.
We are unsure how to configure the parser - we tried several times, and it didn't work.
We need you assistance.

Below are examples of Login and Logout syslog messages:
```
Mar  5 12:32:22 WIN-6UKNDHK4QEV SyslogGen %ASA-7-746012: user-identity: Delete IP-User mapping 10.10.10.1 - LOCAL\lsge\angela.lopez Succeeded - VPN user
```
```
Mar  5 12:32:07 WIN-6UKNDHK4QEV SyslogGen %ASA-7-746012: user-identity: Add IP-User mapping 10.10.10.3 - LOCAL\lsge\christina.baker Succeeded - VPN user
```


#### **Question 4:** 
A customer opened the following ticket - What is the MOST likely cause for the issue? (configuration wise) - you must provide a solution in your first email.

Hello Support,
We have a MUHv2 agent installed on Windows Server 2019.
When we add a windows firewall rule, to allow traffic of specific AD group to our Microsoft-SQL server, the users are not getting access.
But when we uninstall the MUHv2 agent, the users get access to the server, without any change being made to the windows firewall rule.
Why is this happening?


# TP section:



# DLP section:

#### Question 1:
A customer opened the following ticket - in your response, take in consideration known issues (03/2024)

Hello support,
We have identified that some of our workers uploading C++ source code to Google Drive.
We can block downloads completely to Google Drive using content awareness, however this is not our desired goal.
We only want to restrict uploads of source code to Google Drive, but allow anything else.
How can it be performed.


#### Question 2:
A customer have opened the following ticket, assist him to achieve his goal - you must provide a solution in your first email.

Hello Support,
We want to create a DLP rule that will be applied to all files transfers from inside to outside of our organization.
The rule's purpose is to block files of the following types .pdg/.docx./.pptx/.clx/.txt/.js/.py/.xml/.jason
But only if they contain sensitive information.
How can we do that? and how can we define our own patterns?


# Content Awareness section:

#### Question 1:
A customer have opened the following ticket, assist him to achieve his goal - you must provide a solution in your first email.

Hello Support,
We have created the following rule, but it is not working.
![caw-image](https://github.com/IdanShap/esc_exam/assets/112121953/430e66bd-b887-40e2-b9c3-4ff10320ce3e)

Why is not working?

#### Question 2:
A customer have opened the following ticket, assist him to achieve his goal - you must provide a solution in your first email.

Hello support,
We have identified that a Microsoft service is trying to download a .cab file in order to update our Office Suite on client machines.
This is currently blocked by our rule-base.
We would like to allow downloads of ONLY .cab files , and ONLY  from the specific destination https://some-microsoft-service
How can we do it with content awareness?
# Maestro section:
#### Question 1:
Hello Support,

I have a Maestro Security Group with 2 SGMs.
We have the following enabled_blades: fw SSLinsp urlf av ab ips
When running "asg monitor" we see that the second SGM's state is down
The PNOTE in "cphaprob state" says only AMW
When we run "asg_policy verify_amw -a" we can see:
- On SGM 1 - the TP policy name and hash - and status installed
- On SGM 2 - "Disabled"
  
No matter how many times we install the policy, it is not fixed.

When doing fetchlocal, we see the following errors:
```
Installing Threat Prevention policy from local
boolean_cpt malware_tp_conf_reload(const char*, char*, int): Reload(/opt/CPsuite-R81.20/fw1/state/local/AMW) failed ()
127.0.0.1:12872/global_policy/is_ab_installed rc=4
malware_tps_get_active_blades: tpConfClient->GetGlobalPolicySetting() failed
malware_tps_reload: malware_tps_get_active_blades() failed
boolean_cpt malware_tp_conf_reload(const char*, char*, int): malware_tps_reload() failed
malware_load: malware_tp_conf_reload( dir=/opt/CPsuite-R81.20/fw1/state/local/AMW ) failed
```

When we look at the policies folder on SGM 2 we see this:
```
ls -lah /opt/CPsuite-R81.20/fw1/state/__tmp/
lrwxrwxrwx 1 admin root 51 Apr 18 05:26 AMW -> /mnt/fcd/var/opt/CPsuite-R81.20/fw1/state/local/AMW
lrwxrwxrwx 1 admin root 39 Apr 18 05:44 FW1 -> /opt/CPsuite-R81.20/fw1/state/local/FW1
```

Please help us to resolve the PNOTE so the member will be able to become Active and not Down


# Performance section:

#### Question 1:
A customer have opened the following ticket, assist him to achieve his goal - you must provide a solution in your first email.

Hello support,
We are facing High CPU utilization by the RAD process on our cluster.
Several times in a day, we see this high CPU happening, and then it decreases over time.
During the issue, we can see some errors/warnings in logs of Anti-Virus regarding RAD unresponsiveness.
What can be the cause for that? How can we mitigate it? 



# QoS section:



# PTC section:





