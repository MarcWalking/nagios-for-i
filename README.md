# nagios-for-i
## Description
Nagios provides enterprise-class Open Source IT monitoring, network monitoring, server and applications monitoring.<br>
We provide several customized plugin for monitoring IBM i systems.<br>
You could refer to the [this link](https://www.ibm.com/support/pages/node/1274296/ ) for more details.
<br><br>
The nagios plugin for i has two methods. 
* You can run the plugin with a daemon server to handle and dispatch the request to worker thread.<br>
You could start the daemon server by script server_start.sh.
* You can also run the plugin without the server. Then every request will be handled by seperate processes. It would be more simple but consumes more resources.
<br>
The plugins suport to mornitor following martix<br>
<br>
<pre>
  <b>plugin            martix</b><br>
  CPU               Retrieve the CPU utilization for the entire system<br>
  SpecificJobCPU    Retrieve the CPU usage for a specific job<br>
  DiskUsage         Retrieve the disk usage status<br>
  DiskConfig        Retrieve the disk health status<br>
  ASPUsage          Retrieve the ASP usage percentage of the entire system<br>
  ActiveJobs        Retrieve the number of active jobs on the system<br>
  BasicInfo         Retrieve the basic information of an IBM i system<br>
  CurSignOnUsers    Retrieve the number of users that currently log on to the system<br>
  LongRunSQL        Retrieve the longest running SQL<br>
  Message           Retrieve the messages from a specific message queue<br>
  SpecificMessage   Retrieve the status whether a specific message ID is found in a specific message queue<br>
  PageFaults        Retrieve the page faults<br>
  SubsystemJobs     Retrieve job information in a specific subsystem<br>
  CustomSQL         The user could leverage SQL services to create self-defined matrix<br>
  TempStorageJobs   Retrieve top N jobs that have the most temp storage usage<br>
  DaemonServer      Retrieve the daemon server status<br>
</pre>

## Installation and upgrade
<p>For the version of Nagios Core, you could install the latest plugins by service pack in directory <b><i>service pack</i></b>.<br>
You could take <i>Nagios Plugin for IBM i Install and Configure Guidelines.txt</i> for detail steps.
</p>
<br>
<p>For the version of Nagios XI, the plugin for IBM i has already been integrated in XI. You could update the plugins by install the latest wizard file in <b><i>Wizard for NagiosXI/ibmiservice.zip</i></b>.</p>
<br>
