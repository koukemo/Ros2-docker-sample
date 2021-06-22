# Ros2-docker-sample

DockerにてUbuntu20.04上のROS2 foxyを構築する <br>

## 実行方法

以下コマンドを初回のみ実行 <br>

```
docker build --rm -t ros2:foxy .
```

実行時には時間がかかるので注意 <br>


### 動作確認

端末を2つ開き、それぞれで以下を実行 <br>

```
docker run --rm -it ros2:foxy

# 端末1
ros2 run demo_nodes_cpp listener

# 端末2
ros2 run demo_nodes_cpp talker
```