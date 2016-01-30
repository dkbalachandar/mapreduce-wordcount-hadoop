Basic example to run the Map reduce program[Word Count] in a single node cluster 

1. Install the Hadoop in respective operation system. 
2. Create a text file with some text in it
3. Login into Hadoop as hadoop user and go to Hadoop directory[/usr/local/hadoop] run the below command to copy the above files created
    bin/hadoop fs -copyFromLocal inputFile.txt /wordcount/input/inputFile.txt     
4. Copy the Jar into hadoop directory
5. Start the hadoop by going into sbin directory and run the below scripts
   start-dfs.sh
   start-yarn.sh
  6. Run the program as below 
  bin/hadoop jar wordcount-1.0-jar-with-dependencies.jar /wordcount/input /wordcount/output

NameNode - http://localhost:50070
DataNode -  http://localhost:50075
