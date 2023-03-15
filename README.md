# task5
Create Data Vis and Pyspark Tutorial Installation
In this task will be seperated into two parts
1. Data Vis (url: https://lookerstudio.google.com/reporting/6e46a6aa-8e36-4fdb-ab67-296376cb69c1)
![Task Taxi Trip](https://user-images.githubusercontent.com/74971584/225286254-b26e77ee-619e-4801-9ce2-559453534c0b.png)

In this Data Visualization i made 5 Visualization based on : Trip Fare, Passenger Count, Payment Type, PU Location ID, and DO Location ID
We can see that Trip fare and Passenger Count have smiliar pattern, it can be concluded that Trip Fare and Passenger Count are directly proportional
In Pie Diagram We can see that Passenger likely to use Payment Type 1 with 64,9% passengers using this type. 
PU Location that has highset passenger to pickup at ID 273, and Dropoff at ID 236



2. Pyspark Installation

# install dependencies
sudo apt install default-jdk scala git -y

# verify dependencies
java -version; javac -version; scala -version; git --version

# download Spark
wget https://downloads.apache.org/spark/spark-3.3.1/spark-3.3.1-bin-hadoop3-scala2.13.tgz

# extrct files
tar xvf spark-*

# move Spark to /opt/spark
sudo mv spark-3.3.1-bin-hadoop3-scala2.13 /opt/spark

# configure environmental variables (in editor)
source ~/.bashrc
add on editor and save
export SPARK_HOME=/opt/spark
export PATH=$PATH:$SPARK_HOME/bin:$SPARK_HOME/sbin
export PYSPARK_PYTHON=/usr/bin/python3

# load profile
source ~/.profile

# start master server

cd SPARK_HOME
source sbin/start-worker.sh spark://ubuntu1:7077

# start spark
spark-shell

# Spark Version
![image](https://user-images.githubusercontent.com/74971584/225287927-2603a073-6ec8-4791-aab7-3320456b0189.png)


