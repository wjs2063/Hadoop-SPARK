# Hadoop vs Spark

HDFS (Hadoop Distributed File System) 
```
파일을 Hadoop 네이티브 형식으로 저장, 클러스터 전체에서 병렬화 
Map Reduce : block 을 원하는 결과로 결합하기위해 실제로 데이터 병렬로 처리 

Map : key,value 쌍으로 적절히 변형

Reduce : 집계 

```


          Hadoop                                Spark


Disk I/O 발생하므로 속도가 느림             반면 Spark 는 메모리에서 작업   
      일괄처리에 용이                     실시간 데이터 처리 용이    
      배치모드                          실시간 데이터처리가능   
      비용 저렴                         비용증가
      확장성 높음 (노드 + Disk)           RAM 에 의존 확장성 낮음
      
      
