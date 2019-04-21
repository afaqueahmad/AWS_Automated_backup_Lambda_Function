Backup solution required as the part of the BCDR strategy.
Backup helps in recovering the partial or complete environment during failure scenarios.
With an automated backup and Restore solution the downtime can be reduced.
This solution ensures to increase the availability and redundancy of data, which is the most valuable asset.
In order to achieve the desired solution, we designed and developed a functionality using AWS Lambda function (coded in python).

EBS_Snapshot_Solution_Backup.py 
This Lmbda function is executed by the CloudWatch event, It fetches all the server for backup based on the TAGs,creates the snapshot of all the servers and add the retention TAG so that another Lmabda function remove the snapshot based on retension TAGs.

This describes how this solution works:

![iam](https://github.com/afaqueahmad/AWS_Automated_backup_Lambda_Function/blob/master/bkp1.png)

Below Diagram describes the strategy for backup based on backup tags:

![iam](https://github.com/afaqueahmad/AWS_Automated_backup_Lambda_Function/blob/master/bkp2.PNG)
