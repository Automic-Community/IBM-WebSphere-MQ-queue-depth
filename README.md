*IBM WebSphere MQ queue depth*
=============


The Agent monitors the local queues of an IBM WebSphere MQ.
http://github.com/Automic-Community/IBM-WebSphere-MQ-queue-depth

<!-- List of attached files -->
Contents of Solution Package:

						
								*WebSphereMQ_Agent.zip
								
								*30-image1.jpg
								
						


Documenation and Instructions
---

<p>The Agent monitors the local queues of an IBM WebSphere MQ.</p>
<div class="ipsType_textblock ipsPad_half description_content">It can be installed on each Websphere MQ server having the Perl interpreter.<br /><br />The Agent supports the following versions of IBM WebSphere MQ.
<ul class="bbc">
<li>7.0.x</li>
</ul>
The Agent collects :
<ul class="bbc">
<li>The minimum queue depth.</li>
<li>The maximum queue depth.</li>
<li>The average queue depth.</li>
<li>The cumulate queue depth.</li>
</ul>
<p>&nbsp;</p>
<p><strong class="title">Prerequisites:</strong></p>
<p>- Sysload SP Studio 1.20a<br /> - 1 OPENAGENT Token Available<br /> - Perl interpreter <br /> - WebSphere MQ</p>
<p>&nbsp;</p>
<p><strong class="title">Implementation:</strong></p>
<p>1) Import into your SP Studio.<br /> 2) Generate Agent setup from there (refer to Sysload SP Studio User Manual).<br /> 3) Install Agent.<br /> 4) Update your Console (Files .DES).<br /> 5) Enjoy it<br /> <br /> The agent will run the Perl script "mq.pl" located in the resource file attached.<br /> You have to update the `runmqsc` command parameter located in this script line 6 in order to match the name of your target queue manager.<br /> --&gt; $query="echo \'dis ql(QL*) curdepth \' | runmqsc REPLACE |grep -Ev \"AMQ8409|5724-H72|Starting|dis|One|No|All\""; )</p>
</div>

Copyright and License
---

Broadcom does not support, maintain or warrant Solutions, Templates, Actions and any other content published on the Community and is subject to Broadcom Community [Terms and Conditions](https://community.broadcom.com/termsandconditions)



Questions or Need Help? 
---
Join the [Automic Community Integrations](https://community.broadcom.com/communities/community-home?CommunityKey=83e49dd4-b93e-464a-a343-2bb1e51c13ec) to discuss this integration.
