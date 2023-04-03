# EAD_LAB_3
## Created a Helm Pipeline for Lab 3 (Helm)
Steps are

###  Deploy Helm on Azure agent Nodes

Deploy MYSQL and DB Creation Script file Chart */helm/eadlab3/Charts.yaml*
<br>
This Creates:

 - MySql Server Deployment
 - A Secret by name of *ead-lab3-mysql*
 - A configMap to store the db-script file by name of  *db-scripts-configmap*
 <br>
 <img title="Job : Deployment of MySql Server" alt="Alt text" src="screencap/Capture1.PNG">
  
  ### Created a Job to connect to MySql Database
Created a Job  which uses mysql secrets *ead-lab3-mysql* ,  and database script file *db-scripts-configmap* to connect to MySql DB and create a Database
 <br>
 <img title="Job : Creation and Execution of JOB" alt="Alt text" src="screencap/Capture2.PNG">

### Finally
Finally run a shell script to call kubectl and execute to validate and read data from database
  
 <br>
 <img title="Query to database" alt="Alt text" src="screencap/Capture3.PNG">
