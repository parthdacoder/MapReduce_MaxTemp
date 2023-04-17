<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
    <h1>MapReduce_MaxTemp</h1>
    <p>This repository contains a Java program that uses MapReduce to find the maximum temperature from a given dataset. The program takes a text file containing temperature data in the form of key-value pairs, where the key is the location and the value is the temperature recorded at that location.</p>
    <h2>Prerequisites</h2>
    <ul>
      <li>Java Development Kit (JDK) 1.8 or higher</li>
      <li>Apache Hadoop 2.x or higher</li>
    </ul>
    <h2>How to Run</h2>
    <ol>
      <li>Clone the repository: <code>git clone https://github.com/&lt;your_username&gt;/MapReduce_MaxTemp.git</code></li>
      <li>Navigate to the project directory: <code>cd MapReduce_MaxTemp</code></li>
      <li>Compile the Java program: <code>javac -classpath $(hadoop classpath) -d classes/ MaxTemp.java</code></li>
      <li>Create an input directory and upload the temperature data file: <code>hadoop fs -mkdir input &amp;&amp; hadoop fs -put &lt;path_to_input_file&gt; input/</code></li>
      <li>Run the MapReduce job: <code>hadoop jar &lt;path_to_hadoop_jar_file&gt; MaxTemp input/ output/</code></li>
      <li>View the output: <code>hadoop fs -cat output/*</code></li>
    </ol>
    <p>The output will contain the maximum temperature for each location in the input dataset.</p>
    <h2>How it Works</h2>
    <p>MapReduce is a programming model used for processing large amounts of data in a distributed and parallel manner. The MapReduce algorithm consists of two phases: the Map phase and the Reduce phase.</p>
    <p>In the Map phase, the input data is split into smaller chunks and each chunk is processed by a mapper function. The mapper function takes the input data and emits key-value pairs. In this program, the key is the location and the value is the temperature recorded at that location.</p>
    <p>In the Reduce phase, the key-value pairs emitted by the mapper functions are grouped by key and processed by a reducer function. In this program, the reducer function finds the maximum temperature for each location by iterating over the values associated with each key.</p>
    <p>The MapReduce framework handles the distribution and parallel execution of the mapper and reducer functions across multiple nodes in a Hadoop cluster, making it a scalable and efficient way to process large datasets.</p>
  </body>
</html>
