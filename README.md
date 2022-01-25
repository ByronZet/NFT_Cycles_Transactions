Before running the scripts, you need to downoad the ethereum database and the sqlite jdbc jar.

1. Download the sqlite database

   pip3 install kaggle
   ~/.local/bin/kaggle datasets download simiotic/ethereum-nfts
   unzip ethereum-nfts.zip

2. Download the `sqlite-jdbc-3.36.0.3.jar`

   wget https://github.com/xerial/sqlite-jdbc/releases/download/3.36.0.3/sqlite-jdbc-3.36.0.3.jar
   
To run a script, the following command:

spark-submit --jars sqlite-jdbc-3.36.0.3.jar --driver-memory 4g --executor-memory 4g
