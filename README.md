# NBA Data ETL Project
# Pre-requisites
Apache Spark installed
Scala installed
sbt installed
# Getting Started
1. Clone the repository and Change the Directory using **cd scala_project**
2. Update the API URLs: Open Extract.scala and replace the placeholder URLs with the actual API endpoints.
    val urlMatches = "https://api.example.com/games?season=2021-2022&team="
    val urlStats = "https://api.example.com/stats?season=2021-2022&team="
3. Build the project using **sbt package**
4. Run the extraction using **spark-submit --class Extract target/scala-2.12/NBADataETL_2.12-1.0.jar
**
5. Run the transformation using **spark-submit --class Transform target/scala-2.12/NBADataETL_2.12-1.0.jar
** This will transform the data and save the final DataFrame as a CSV file.

6. Check the results: The final CSV file will be saved in the project directory as **final_output.csv**
