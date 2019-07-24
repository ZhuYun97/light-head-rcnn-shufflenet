# **Under development!!!**
# light-head-rcnn
Developed based on pytorch, backbone replaced with shufflenet v2.<br>
The codes are based on [faster-rcnn](https://github.com/jwyang/faster-rcnn.pytorch). <br>
I think it's better to understand the codes of [faster-rcnn](https://github.com/jwyang/faster-rcnn.pytorch), if you want to modify the codes(e.g. adding new network)
## How to understand the codes
#### [How to generate anchors, Chinese edition](https://blog.csdn.net/williamyi96/article/details/77996526)

## light backbone
I add a state-of-the-art network which is called [ShuffleNet v2](https://github.com/ZhuYun97/ShuffleNet-v2-Pytorch), because I want to run this detector on mobile phone. If you find some newer and better network, you can add to the project following steps bellow.
### How to add new backbone?
1. In the `/lib/model/faster_rcnn/` folder, you can add your network(e.g. EfficientNet, MobileNetv3). You can refer to `mobilenet.py` to code your own network.
2. In the `/cfgs/` folder, you shoud add a `yml` file corresponding to your network. Also, you can refer to `mobilenet.yml`.

