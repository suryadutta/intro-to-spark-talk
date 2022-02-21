## Outline for Spark Dev Talk

1. What is Big Data
    * Ask for answers in chat box
    * 4 V's - Volume, Velocity, Variety, Veracity
    * Big data platforms can definitely handle volume, but good platforms like Spark are set up to handle all of these scenarios. We'll see how.

3. What is Spark?

    * Platform

    * Why do we need it?
        * limits of processing datasets on one machine
            * not enough disk / memory to hold the data
            * some analysis requires computation over all data 
                * simple ex: sorting
        * vertical vs horizontal scaling costs
            * Moore's Law is Dead

    * What we need to distribute compute:
        * Parallelism
        * Fault-Tolerance
        * Compatibility

    * Different ways to use spark (PySpark, Scala, Java)

3. Evolution of Spark APIs
    * Pre-Spark: Hadoop & MapReduce 
    * RDDs
    * DataFrame and Datasets
    * Spark SQL
    * How it all fits together

4. PySpark Commands
    * Importing Data
        * sc.parallelize
        * read csv 
        * other data formats (json, parquet, db connectors)
    * Basic commands
        * select / selectExpr 
        * adding / renaming / dropping columns
        * literal values
        * change a column type
        * filtering rows (filter, where)
        * sort
        * limit
    * Working with types
        * number functions
        * string functions
        * datetime functions
    * User defined functions
    * Aggregations
        * count / countdistinct 
        * sum/avg
        * groupby aggregation
    * Joins

5. Let's code some stuff:
    * DataBricks Wikipedia Clickstream example

