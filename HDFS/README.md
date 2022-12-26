
putty 로 sandbox 에 접속 

```
hadoop fs -mkdir m1-100k

hadoop fs -ls

wget http://media.sundog-soft.com/hadoop/ml-100k/u.data

hadoop fs -copyFromLocal u.data ml-100k/u.data  

hadoop fs -ls ml-100k
```


### MRJOB INSTALL 

```
su root

password 입력

yum-config-manager --save --setopt=HDP-SOLR-2.6-100.skip_if_unavailable=True

yum install https://repo.ius.io/ius-release-el7.rpm https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm 

yum install python-pip

pip install mrjob==0.7.4

yun install nano

wget http://media.sundog-soft.com/hadoop/ml-100k/u.data

wget http://media.sundog-soft.com/hadoop/RatingsBreakdown.py

```


## LOCAL 

```
python RatingsBreakdown.py -r hadoop --hadoop-streaming-jar /usr/hdp/current/hadoop-mapreduce-client/hadoop-streaming.jar u.data


```
