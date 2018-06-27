# YelpDataSet-Analysis-Visualisation

Analysis and Visualisation of Yelp Dataset using Apache Spark | ELK Stack ( Elastic Search, Logstash, Kibana)

</br>

## Introduction

Most businesses seek to get reviews on their goods and services one way or another. It is a most basic way for the business to improve their efficiency and subsequently their bottom-line. Get the review is not only the issue, ability to extract and visualize analytics from review data is critical to business success.

In Apache Spark Project, we will use the yelp review dataset to analyze businesses and reviews over a period of time. Perhaps we will spot potential gaps in service delivery or see how business thrive in different scenarios.

Beyond processing this data, we will ingest the final output of our data processing in Elasticsearch and use the visualization tool in the ELK stack to visualize various kinds of ad-hoc reports from the data.


</br>

## Goal

The goal of this Spark project is to analyze business reviews from Yelp dataset and ingest the final output of data processing in Elastic Search.Also, use the visualisation tool in the ELK stack to visualize various kinds of ad-hoc reports from the data.

</br>

## Architecture

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/Uarch.png)

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/ar.png)


• Import data from yelp dataset into relational database(MySQL)
   
    please go through file(get_yelp_in_mysql_databaset.txt) for more information 

• Ingesting data from relational database (MySQL) using Sqoop into Hadoop HDFS

    please go through file(yelp_mysql_sqoop_commands.txt) for more information 

• Ingesting data from relational database directly into Spark

•  Processing relational data in Spark

•  Ingesting processed data into Elasticsearch

•  Visualizing review analytics using Kibana


## Technology stack

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/tec.png)

</br>    


<table>
<thead>
<tr>
<th>Area</th>
<th>Technology</th>
</tr>
</thead>
<tbody>
    <tr>
        <td>DataSet </td>
        <td> Yelp </td>
    </tr>
    <tr>
        <td>Relational Database</td>
        <td>MySQL</td>
    </tr>
    <tr>
        <td>Big Data Ingestion Tool</td>
        <td>Hadoop (Sqoop) </td>
    </tr>
    <tr>
        <td>Distributed File System</td>
        <td> Hadoop (HDFS) </td>
    </tr>
    <tr>
        <td>Cluster Computing Framework</td>
        <td>Apache Spark (Scala) </td>
    </tr>
    <tr>
        <td>Search and Analytics Engine </td>
        <td>Elasticsearch</td>
    </tr>  
</tbody>
</table>

</br>   

## Yelp schema

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/schema.png)

Out of all attributes we will focus on some shown below 

Business

category

hours

Review

</br>

## Use Cases considered for Visualisation

</br>


   Top 10 Business Categories

   Yelp Business Map

   Business distribution by state

   Average rating of business over time

   Top rated businesses 

   User sign up trend




</br>

## Configuring Environment

</br>

Installation of Cloudera quickstart VM

Installation of Elk stack

Later Configuring Scala Runtime to Cloudera QuickStart VM

Watch the below video for more information 

https://www.youtube.com/watch?v=SFJsuo2XISs

</br>

## Execution Instructions
 
   Launch the Spark Shell

   spark-shell --packages org.elasticsearch:elasticsearch-spark-13_2.10:6.1.1 --conf spark.es.index.auto.create=true --conf spark.es.nodes= Ipaddress:port(Elastic search)

</br>

## Visualisation Screen shots

After Ingesting processed data into Elasticsearch

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/1.png)

Yelp User sign up trend

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/2.png)


![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/3.png)


Business distribution by state

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/5.png)


Yelp review

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/review.png)

Top 10 Business Categories

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/cat.png)

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/catdes.png)

Dashboard 

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/dash.png)





