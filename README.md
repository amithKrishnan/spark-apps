spark-apps
==========

spark-apps contains several standalone Spark apps.

The project can be built by running

*./gradlew build*

from the project folder. The built jar will then be available in *spark-apps/build/libs/* folder

To run this jar locally run

YOUR_SPARK_HOME/bin/spark-submit --class JOB_CLASS_NAME --master local PATH_TO_BUILT_JAR ARGUMENTS_TO_JOB

*Example*

YOUR_SPARK_HOME/bin/spark-submit --class "SimpleApp" --master local  YOUR_PROJECTS_FOLDER/spark-apps/build/libs/spark-apps-0.1.jar PATH_TO_SAMPLE_FILE
