CES Process

I.	Receive the call from PagerDuty
a.	Choose the acknowledge option in the response and you will be assigned a ticket with the details of the failure
II.	Log into Control-M
a.	Place the job on hold  
b.	Go to the alerts window and look for the job in the list, write in the comments window that you are looking into the failure and click save
c.	Mark the alert as Reviewed  
III.	Open the CES Production Schedule and look for the job in the spreadsheet
a.	Verify the Job type to gather more information
i.	If the job is an SAP Program
1.	Log into SAP PM1
2.	Enter transaction SM37 in the search bar
3.	Search for the job name, change the username to (*), add the current date and then click execute
4.	Once job comes up check the log by selecting the canceled run and then click on the Job Log button
5.	Gather the information on the failure and take note of what the issue is.
6.	Check if column AJ has any notes, if something exists check the Recovery Instructions tab in how to handle the jobs
a.	Contact the second/third line of contact (columns AH/AI) to give them the failure and request how to address it. Should you not receive a response then reach out to the Module lead (column AO)
i.	The Module Lead appears in the Module Contacts tab
b.	The Functional team will inform how to address the failure.
ii.	If the job is an AFT
1.	Check the type of failure, ex. Connection, Missing File
2.	If the failure appears to be a connection problem, try to rerun the job to see if it works.
a.	If the rerun fails, reach out the Second Line of Contact
3.	If the failure is a missing file reach out to the Third Line of Contact to find out what happened to the file.
iii.	If the job is Unix Script/Sleep/Windows Bat/Resource, reach out to the Second Line of Contact to investigate the problem
iv.	If the job is a Filewatcher
1.	Check column T to see the file path
2.	Log into SAP
3.	Enter transaction AL11 in the search bar
4.	Dig down into the file path from column T to verify if the file is there
5.	If the file exists rerun the job
6.	If the file is missing
a.	Reach out to the First/Second/Third line of contacts to find information on where the missing file is and when it will be sent
i.	If the file comes from the Gateway (filepath includes gwx) then a ticket must be created for them to send the file over (link in page 3) (Steps to create the ticket page 7).
b.	Once the file received rerun the job.
c.	If the file will not be available on the same day, contact the Module Lead to inform them. They will advise on what to do.
