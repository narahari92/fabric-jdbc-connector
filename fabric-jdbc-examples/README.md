Running Instruction
===============

### Asset Transfer example
To run the fabric jdbc asset transfer example, execute following command:
```
mvn exec:java -Dexec.mainClass="com.impetus.fabric.example.App" -DconfigPath=<configPathDirectory> -Dchannel=<channelName> -Dexec.classpathScope="compile" -Dexec.cleanupDaemonThreads=false
```

The Asset IDs that exist are *1000*, *1001*, *1002*, *1003*, *1004* and the participant IDs that exist are *2000*, *2001*, *2002*.

### Fabric spark example

To run the fabric spark example, execute following commands.

```
mvn clean install -Pspark
spark-submit --class com.impetus.fabric.spark.example.App --master local[*] --conf spark.fabric.configpath=<configPathDirectory> --conf spark.fabric.username=admin --conf spark.fabric.password=adminpw target/fabric-jdbc-examples-1.1.0-SNAPSHOT.jar
```



### Flight Delay Insurance example

To run flight delay insurance example, execute below command

```
mvn exec:java -Dexec.mainClass="com.impetus.fabric.flightdelayinsuranceexample.InsuranceApp" -DconfigPath=<configPathDirectory> -Dchannel=<channelName> -Dexec.classpathScope="compile" -Dexec.cleanupDaemonThreads=false

```
