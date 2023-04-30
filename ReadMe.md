### 오프라인에서 도커 이미지 다운받는 방법

1. 도커 이미지를 온라인환경에서 다운로드 한다.
```
 $ docker pull confluentinc/cp-kafka
 $ docker pull confluentinc/cp-zookeeper
 $ docker pull provectuslabs/kafka-ui
```

2. 도커 이미지를 오프라인 환경으로 복사한다.
```
 - docker save -o kafka.tar confluentinc/cp-kafka
 - docker save -o zookeeper.tar confluentinc/cp-zookeeper
 - docker save -o kafka-ui.tar provectuslabs/kafka-ui
```

3. 오프라인 환경에서 도커 이미지를 불러옵니다.
```
 - docker load -i kafka.tar
 - docker load -i zookeeper.tar
 - docker load -i kafka-ui.tar
```

