
### Instructions:
Each of the 4 questions below, simulate an IDA ticket first response.
All the questions below can be solved by the provided information - without the need to ask the customer for more information / files.
Your answers to these questions must be in a format of an email to the customer.
You must explain the solution, like you would explain it to a customer.

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




