Technology Stack
Apache Spark 3.2.1
Scala SDK 2.12.11
Oracle OpenJDK 1.8.0_341


Installation
Environment Setup: Follow the specific instructions for setting up Apache Spark on Ubuntu or Windows. Ensure Scala SDK and Java JDK are properly installed.
IDE Setup: The project development was carried out using IntelliJ IDEA with the Scala plugin. Ensure the IDE is set up with the correct Scala version and Spark library dependencies.
Building the Project: Use SBT and Assembly plugins to compile and package the Scala project into a .jar file.
Usage
Step 1: Set up your Hadoop and Apache Spark test environment.
Step 2: Complete the programming assignments for both Hot Zone Analysis and Hot Cell Analysis by submitting the source code as a .jar file.
Step 3: Write and submit a detailed project report of your work.

Dataset :- yellow_tripdata_2009-01_point.csv

Project Descriptions
Hot Zone Analysis
Objective: Perform a range join operation between rectangle datasets and point datasets to calculate the "hotness" of all rectangles based on the number of points each rectangle contains.
Input: Point data representing NYC taxi pickup locations and rectangle datasets containing zone coordinates.
Output: A sorted list of all zones with their point count, indicating the level of activity or hotness.

Hot Cell Analysis
Objective: Apply spatial statistics to identify statistically significant spatial hot spots using the Getis-Ord statistic on NYC Taxi Trip datasets.
Input: Monthly taxi trip dataset from 2009 - 2012. Each cell's unit size is 0.01 * 0.01 degrees, with 1 day as the Time Step size.
Output: Coordinates of the top 50 hottest cells sorted by their significance without the actual G-score values.
Coding Template Specifications
Input Parameters: Includes output path, task name ("hotzoneanalysis" or "hotcellanalysis"), and task parameters (nyc taxi data path, zone path for hot zone analysis; nyc taxi data path for hot cell analysis).
Data Format: Point data format for pickup locations and zone data format for hot zone analysis.
Expected Output: For hot zone analysis, all zones with their count, sorted ascendingly by rectangle string. For hot cell analysis, the coordinates of the top 50 hottest cells sorted by their significance.


Lessons Learned
This project offered invaluable experience in spatial analysis and big data processing with Apache Spark. Key learnings include:

Implementation of spatial operations and understanding of spatial relationships.
Optimization of Spark SQL for efficient data transformations.
Application of geospatial libraries like GeoSpark for spatial analysis tasks.
Integration of technologies (Spark, Scala, Hadoop) and system handling across different platforms (Windows).


Results
The project yielded insightful results into the spatial distribution of taxi pickups in NYC, identifying key hotspots and patterns of activity. These findings have practical implications for urban planning, traffic management, and targeted marketing strategies.
