# DBA-lab1
1) 
     - unlock hr user    
     ![Screenshot (890)](https://user-images.githubusercontent.com/93229250/231505661-7af0a823-540e-4a08-b6a3-16ba4bbbafc1.png)

     - connect as HR user
     ![Screenshot (891)](https://user-images.githubusercontent.com/93229250/231506070-f1bf71dd-2ff4-4250-afce-605da2ec088d.png)

     - create table t1 with two columns , column 1 number , column2 varchar2
     ![Screenshot (892)](https://user-images.githubusercontent.com/93229250/231506387-ab72aa16-c543-455f-84af-f6ae1adf00df.png)

     - insert 3 rows in this table
     ![Screenshot (894)](https://user-images.githubusercontent.com/93229250/231509207-df70ae35-a51e-4ada-8e30-c7ef81415466.png)

     - find information related to this table, and in which tablespace it saved. 
     ![Screenshot (895)](https://user-images.githubusercontent.com/93229250/231509471-8e133e20-9d16-4d51-982d-1d0835146397.png)

2)
     - find the indexes for table hr.departments
     ![Screenshot (896)](https://user-images.githubusercontent.com/93229250/231509685-eaaa5864-b30a-4b17-af47-67544041eb7a.png)

     - find all objects related to HR schema
     ![Screenshot (898)](https://user-images.githubusercontent.com/93229250/231510235-4c9444f2-113a-4510-acaf-a1451f133c6a.png)
     ![Screenshot (899)](https://user-images.githubusercontent.com/93229250/231510281-0727066c-dd6d-4124-9000-51386909018d.png)
     or getting its count directly 
     ![Screenshot (897)](https://user-images.githubusercontent.com/93229250/231510521-266199b3-c2c8-40d9-b6e4-58891f85e894.png)

     - rebuild one of this indexes  "DEPT_ID_PK" 
     ![Screenshot (900)](https://user-images.githubusercontent.com/93229250/231510947-04928b5d-b061-4797-b8af-d2f9f5ddfb1c.png)


3)
     - change parameter audit_trail from none to DB.
     ![Screenshot (909)](https://user-images.githubusercontent.com/93229250/231517808-c17df6e8-ef62-4dd6-b20e-dc4de2ed974b.png)

     - restart the database to find the changes
     ![Screenshot (904)](https://user-images.githubusercontent.com/93229250/231513318-5df64e5b-3c34-4c38-b28c-620971d1355d.png)

     - create pfile from the spfile and find the change you made on it.
     I created it before!
     BY: create pfile from spfile;
     so I check changes directly  
     ![Screenshot (906)](https://user-images.githubusercontent.com/93229250/231515465-727655aa-42a6-4f62-9328-be5ba549b42d.png)

     - edit the pfile and make the audit_sys_operations=true 
     ![Screenshot (911)](https://user-images.githubusercontent.com/93229250/231519135-c2b2f9ea-45c4-4034-b703-ea4d9434b977.png)

     - start the database using this pfile.
     ![Screenshot (913)](https://user-images.githubusercontent.com/93229250/231520750-fab5c495-1568-4589-a658-6238931412e3.png)

     - create spfile from the pfile.
     ![Screenshot (915)](https://user-images.githubusercontent.com/93229250/231526960-dd918196-5222-4ed2-b2ed-c076d0184c52.png)

4)
     - show the version of your database using the view "v$version"
     ![Screenshot (917)](https://user-images.githubusercontent.com/93229250/231527334-c88cfb7b-2eaa-4be2-842d-bc80464c3c9f.png)

     - show hostname, instance name, status, open mode and startup_time using the views "v$instance" and "v$database"
     ![Screenshot (919)](https://user-images.githubusercontent.com/93229250/231528967-0111b4bd-426a-46fe-ac0c-7145081cde73.png)

     - show the name and type of parameter "db_create_file_dest" using view "v$parameter"
     ![Screenshot (921)](https://user-images.githubusercontent.com/93229250/231529496-33376bfd-5d1a-46cf-9298-8bac07256111.png)

     - show your archiving status then enable the archiving mode if not enabled and show your archiving status again.
     ![Screenshot (923)](https://user-images.githubusercontent.com/93229250/231530140-d33ecd21-61ff-4baa-95fd-a41e2b5dbb71.png)
     ![Screenshot (925)](https://user-images.githubusercontent.com/93229250/231530789-603ae743-5a9c-43d6-ab6d-245b1001ba5a.png)

     - Identify the location of the alert log file.
     ![Screenshot (930)](https://user-images.githubusercontent.com/93229250/231534034-bd4a2ceb-07f2-4bbe-9f83-87a65c6fcd9b.png)

     - shutdown your database with the most safe and fast method and watch your alert log while doing this (use "tail -f" command).
     ![Screenshot (934)](https://user-images.githubusercontent.com/93229250/231534915-c34c0b1a-13d1-49ac-8e3e-e8d2769da37f.png)
     ![Screenshot (932)](https://user-images.githubusercontent.com/93229250/231534950-e2d6ba58-d588-433a-9b4c-0998667a4e32.png)

     - Start up your database step by step and watch your alert log while doing this (use "tail -f" command).
     ![Screenshot (937)](https://user-images.githubusercontent.com/93229250/231535600-0d7a678e-5df2-443b-908f-9212d0f38020.png)
     ![Screenshot (939)](https://user-images.githubusercontent.com/93229250/231536011-f45d8168-cf2b-477d-b299-39d89de4e896.png)
