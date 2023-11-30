<h1>DDoS Tools: CLDAP</h1>

As the availability of sourced tools for threat actors continues to increase, we can expect to see an increase in attack performance volume in the coming years.

In perspective:
In 2018, <a href="https://github.blog/2018-03-01-ddos-incident-report">GitHub’s publicly disclosed large scale DDoS attack</a> measured at 1.35 Tbps. 

In 2020, <a href="https://aws-shield-tlr.s3.amazonaws.com/2020-Q1_AWS_Shield_TLR.pdf">AWS’s publicly disclosed DDoS attack</a> measured at 2.3 Tbps, a 70 percent increase compared to the 2018 Github attack.
<br>

<h3>What tool was used in the AWS DDoS attack?</h3>
<a href="https://www.rfc-archive.org/getrfc.php?rfc=3352#gsc.tab=0">Connection-less Lightweight Directory Access Protocol (CLDAP)</a>  was used as a reflector to amplify the volume of this DDoS attack.

<br>

<h3>What is CLDAP and what is it normally used for?</h3> 
CLDAP is used to reduce the overhead of completing small directory lookups by avoiding the overhead from establishing/closing connections, and works via UDP. It is inherently designed with security vulnerabilities in order to reduce connection overhead. Although uncommon in comparison to other DDoS weapons, there are a notable number of instances where CLDAP is used as a reflector during DDoS attacks.

<br>

<h3>What are the ​benefits to threat actors of amplification attacks? </h3>
1. Amplification of the attacker’s payload<Br>
2. Ability to spoof the attacker’s tracks

<br>

<h3>How common of a threat are CLDAP DDoS attacks? </h3>
CLDAP attacks are notable, but are not as common as other potential DDoS weapons. <a href="https://www.a10networks.com/resources/reports/2022-ddos-threat-report/">A10’s DDoS Weapons Report</a> shows that CLDAP is a mere fraction of the top 5 DDoS weapons, which include <a href="https://www.securityweek.com/rpc-portmapper-abused-ddos-attack-reflection-amplification/#:~:text=Malicious%20actors%20can%20use%20Portmapper,larger%20response%20to%20the%20victim.">Portmap</a>, 
<a href="https://www.techtarget.com/searchnetworking/definition/SNMP">SNMP</a>,
<a href="https://www.akamai.com/glossary/what-is-an-ssdp-ddos-attack">SSDP</a>, 
<a href="https://www.cloudflare.com/learning/ddos/dns-amplification-ddos-attack/">DNS Resolver</a>, 
and <a href="https://www.incibe.es/en/incibe-cert/blog/drdos-cyberattacks-based-tftp-protocol">TFTP</a>.
<br>
The list’s number 5, TFTP is listed as 1,054,330 DDoS weapons currently available while CLDAP is listed as having only 15,651 DDoS weapons available. While this number is not insignificant, in the larger context of DDoS threat tools, the likelihood of a threat actor utilizing one or more of the previously mentioned tools is significantly higher than the likelihood of a threat actor utilizing CLDAP alone for a DDoS attack.

<br>

<h3>How can enterprises protect themselves from CLDAP DDoS attacks?</h3>
1. Blocking or rate-limiting CLDAP’s UDP port 389<br>
2. Establish traffic baselines and monitor carefully for any unusual traffic spikes
