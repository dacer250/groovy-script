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

    ##简介
在SOA开发过程中,使用intelliJ IDEA 开发 JPA.需要根据table生成POJO,而且是带JPA
注解的POJO,例如@Entity @Column @Builder 之类.
目前的已有的generate POJO 工具只能生成bean.无法满足JPA POJO的需求.问题在于:
1.bean的属性需要配合项目,使用Camel Name法则
2.无JPA特性的注解
3.无继承Serializable接口和生成defaultSerialID

由于以上原因,可以看到通过网络搜索到的脚本没办法直接使用.因此自己修改生成了一个groovy脚本.能够生成满足自己使用.

##环境
windows下 IDEA IntelliJ. Mac下需要运行groovy脚本,对应的步骤需要修改.


