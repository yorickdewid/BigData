installeer krb5.conf in /etc/ (https://github.com/sara-nl/hathi-client)

download FireFox
browser setup (https://github.com/sara-nl/hathi-client)
test jobtracker http://head05.hathi.surfsara.nl/

ssh hhscyber@login.hathi.surfsara.nl
de login node is de gateway waarmee je toegang hebt tot het cluster

hdfs dfs -ls    # laat de inhoud op hdfs zien
hdfs dfs --help # hdfs commando's
hdfs dfs -get   # copieren van hdfs naar dfs
hdfs dfs -put   # copieren van dfs naar hdfs
hdfs dfs -cat   # een file tonen als platte text

yarn application -list      # jobs in de jobtracker
yarn application --help     # jobtracker commando's
yarn application -kill <id> # kill een job

yarn jar <jarfile> <class> <args>  # start de class in de jafile als een job, main ontvangt String[] args
yarn jar <jarfile> <class> -libjars jars/*.jar <args>  # start een job, libjars worden gecopieerd naar nodes

copy HuckleberryFinn.txt naar login
copy van login naar HDFS

wordcount example
http://hadoop.apache.org/docs/current/hadoop-mapreduce-client/hadoop-mapreduce-client-core/MapReduceTutorial.html#Example:_WordCount_v1.0

voer wordcount uit op HuckleberryFinn.txt


