# groovy-script
Generate JPA POJOs under IDEA intelliJ

# How to Use:
1.Put this file under :
C:\Users\Administrator\.IntelliJIdea2017.1\config\extensions\com.intellij.database\schema\ <br/>
This path can be found by following steps:<br/>
a. Open IDEA, right pannel,choose DataBase<br/>
b. Connect to currrent DB.<br/>
c. choose  one table, Right click (on Windows),choose the "Scripted Extentions" -> "Go to Script Directory"<br/>
d. Open this directory in Explore. Back up the origional "Generate POJOs.groovy". Replace it with your downloaded file.<br/>
2. Use it just like it's the origional one!  <br/>
  Choose a DATATABLE, Right Click ," Scripted Extentions" -> Generate POJOs.groovy!<br/>
  
# 3.Caution:<br/>
 a. The DB column which name is "id"(ignore the case) is recognized as Primary KEY ,annotated BY @Id<br/>
 b. You Should OPEN this file , modify its VARIABLE according to your MODULE/PROJECT ,such as:<br/>
   packageName,<br/>
   beanName,<br/>
   author, etc.<br/>
 c. When comes to DB column type mapping to POJO, you should always perform a double CHECK!<br/>
    This file is modified according to ORCALE DB SYSTEM.<br/>
    About this, you should refer to :<br/>
    http://blog.csdn.net/high2011/article/details/47701455<br/>
