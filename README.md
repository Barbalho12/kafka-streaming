## Dependencies

* docker
* docker-compose
* python3
* pip3

**Python libs:**

* kafka-python (lib)
* opencv-python (lib)
* Flask (lib)

**Install libs**

```bash
pip3 install -r requirements.txt
```

## Running


**Terminal 1** Inicialize `Zookeeper` and `Kafka` on Docker
```bash
docker-compose up
```

**Terminal 2** Execute consumer script, for receive data frames and show on browser 
```bash
python consumer.py
```

**Terminal 3** Execute producer passing video sample `dummy.mp4` or `0` for camera streaming (if connected)
```bash
python producer.py dummy.mp4
```

Open http://localhost:5000 in Browser 

## References

* [Python code](https://github.com/akmamun/kafka-python-camera-stream)
* [kafka](https://hub.docker.com/r/wurstmeister/kafka/)
* [zookeeper](https://github.com/bitnami/bitnami-docker-zookeeper)
* [Video Streaming with Python and Kafka](https://medium.com/@kevin.michael.horan/distributed-video-streaming-with-python-and-kafka-551de69fe1dd)
