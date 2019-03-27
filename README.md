//If you are using Spark 2.4.0

If you are using IntelliJ :
    
    Add the dependency : "org.apache.spark" %% "spark-avro" % "2.4.0"
    
    In the code section just use : val x = spark.read.format("avro").load("/path/of/dir")
    
    You are done.
    
    
If you are using CLI : 

    use the command : spark-shell --packages org.apache.spark:spark-avro_2.11:2.4.0
    
    In front of Scala console use : val x = spark.read.format("avro").load("/path/of/dir")
    
    You are done.
    

If you want to execute the jar :

    use the command : spark-submit --packages org.apache.spark:spark-avro_2.11:2.4.0 --class xyz --master local /xx/yy/your.jar
    
    You are done.
    
    
//If you are using versions < 2.4.0

If you are using IntelliJ :

    Add the dependency : "com.databricks" %% "spark-avro" % "4.0.0"
    
    In the code section just use : val x = spark.read.format("com.databricks.spark.avro").load("/path/of/dir")
    
    You are done.
    
    
If you are using CLI : 

    use the command : spark-shell  --packages com.databricks:spark-avro_2.11:4.0.0
    
    In front of Scala console use : val x = spark.read.format("com.databricks.spark.avro").load("/path/of/dir")
    
    You are done.
    
    
 If you want to execute the jar :

    use the command : spark-submit  --packages com.databricks:spark-avro_2.11:4.0.0 --class xyz --master local /xx/yy/your.jar
    
    Note : In jar don't forget to mention : ("com.databricks.spark.avro")
    
    You are done.
    
    

    

    
