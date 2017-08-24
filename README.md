# groovy-script
Generate JPA POJOs under IDEA intelliJ

How to User:
1.Put this file under :
C:\Users\Administrator\.IntelliJIdea2017.1\config\extensions\com.intellij.database\schema\
This path can be found by following steps:
a. Open IDEA, right pannel,choose DataBase
b. Connect to currrent DB.
c. choose  one table, Right click (on Windows),choose the "Scripted Extentions" -> "Go to Script Directory"
d. Open this directory in Explore. Back up the origional "Generate POJOs.groovy". Replace it with your downloaded file.
2. Use it just like it's the origional one!  
  Choose a DATATABLE, Right Click ," Scripted Extentions" -> Generate POJOs.groovy!
  
3.Caution:
 a. The DB column which name is "id"(ignore the case) is recognized as Primary KEY ,annotated BY @Id
 b. You Should OPEN this file , modify its VARIABLE according to your MODULE/PROJECT ,such as:
   packageName,
   beanName,
   author, etc.
 c. When comes to DB column type mapping to POJO, you should always perform a double CHECK!
    This file is modified according to ORCALE DB SYSTEM.
    About this, you should refer to :
    http://blog.csdn.net/high2011/article/details/47701455
