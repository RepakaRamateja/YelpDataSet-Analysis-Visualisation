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

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/arch.png)

![alt text](https://github.com/RepakaRamateja/YelpDataSet-Analysis-Visualisation/blob/master/images/arc.png)


• Import data from yelp dataset into relational database(MySQL)
   
    please go through file(get_yelp_in_mysql_databaset.txt) for more information 

• Ingesting data from relational database (MySQL) using Sqoop into Hadoop HDFS

    please go through file(yelp_mysql_sqoop_commands.txt) for more information 

• Ingesting data from relational database directly into Spark

•  Processing relational data in Spark

•  Ingesting processed data into Elasticsearch

•  Visualizing review analytics using Kibana


## Technology stack



