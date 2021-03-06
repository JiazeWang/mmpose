# Changelog

## v0.9.0 (30/11/2020)

**Highlights**

1. Support more human pose estimation methods.
  - [MSPN](https://arxiv.org/abs/1901.00148)
  - [RSN](https://arxiv.org/abs/2003.04030)
1. Support video pose estimation datasets.
  - [sub-JHMDB](http://jhmdb.is.tue.mpg.de/dataset)
1. Support Onnx model conversion.

**New Features**

- Support MSPN ([\#278](https://github.com/open-mmlab/mmpose/pull/278))
- Support RSN ([\#221](https://github.com/open-mmlab/mmpose/pull/221), [\#318](https://github.com/open-mmlab/mmpose/pull/318))
- Support new post-processing method for MSPN & RSN ([\#288](https://github.com/open-mmlab/mmpose/pull/288))
- Support sub-JHMDB dataset ([\#292](https://github.com/open-mmlab/mmpose/pull/292))
- Support urls for pre-trained models in config files ([\#232](https://github.com/open-mmlab/mmpose/pull/232))
- Support Onnx ([\#305](https://github.com/open-mmlab/mmpose/pull/305))

**Bug Fixes**

- Fix model download links in README ([\#255](https://github.com/open-mmlab/mmpose/pull/255), [\#315](https://github.com/open-mmlab/mmpose/pull/315))

**Breaking Changes**

- `post_process=True|False` and `unbiased_decoding=True|False` are deprecated, use `post_process=None|default|unbiased` etc. instead ([\#288](https://github.com/open-mmlab/mmpose/pull/288))

**Improvements**

- Enrich the model zoo ([\#256](https://github.com/open-mmlab/mmpose/pull/256), [\#320](https://github.com/open-mmlab/mmpose/pull/320))
- Set the default map_location as 'cpu' to reduce gpu memory cost ([\#227](https://github.com/open-mmlab/mmpose/pull/227))
- Support return heatmaps and backbone features for bottom-up models ([\#229](https://github.com/open-mmlab/mmpose/pull/229))
- Upgrade mmcv maximum & minimum version ([\#269](https://github.com/open-mmlab/mmpose/pull/269), [\#313](https://github.com/open-mmlab/mmpose/pull/313))
- Automatically add modelzoo statistics to readthedocs ([\#252](https://github.com/open-mmlab/mmpose/pull/252))
- Fix Pylint issues ([\#258](https://github.com/open-mmlab/mmpose/pull/258), [\#259](https://github.com/open-mmlab/mmpose/pull/259), [\#260](https://github.com/open-mmlab/mmpose/pull/260), [\#262](https://github.com/open-mmlab/mmpose/pull/262), [\#265](https://github.com/open-mmlab/mmpose/pull/265), [\#267](https://github.com/open-mmlab/mmpose/pull/267), [\#268](https://github.com/open-mmlab/mmpose/pull/268), [\#270](https://github.com/open-mmlab/mmpose/pull/270), [\#271](https://github.com/open-mmlab/mmpose/pull/271), [\#272](https://github.com/open-mmlab/mmpose/pull/272), [\#273](https://github.com/open-mmlab/mmpose/pull/273), [\#275](https://github.com/open-mmlab/mmpose/pull/275), [\#276](https://github.com/open-mmlab/mmpose/pull/276), [\#283](https://github.com/open-mmlab/mmpose/pull/283), [\#285](https://github.com/open-mmlab/mmpose/pull/285), [\#293](https://github.com/open-mmlab/mmpose/pull/293), [\#294](https://github.com/open-mmlab/mmpose/pull/294), [\#295](https://github.com/open-mmlab/mmpose/pull/295))
- Improve README ([\#226](https://github.com/open-mmlab/mmpose/pull/226), [\#257](https://github.com/open-mmlab/mmpose/pull/257), [\#264](https://github.com/open-mmlab/mmpose/pull/264), [\#280](https://github.com/open-mmlab/mmpose/pull/280), [\#296](https://github.com/open-mmlab/mmpose/pull/296))
- Support PyTorch 1.7 in CI ([\#274](https://github.com/open-mmlab/mmpose/pull/274))
- Add docs/tutorials for running demos ([\#263](https://github.com/open-mmlab/mmpose/pull/263))

## v0.8.0 (31/10/2020)

**Highlights**

1. Support more human pose estimation datasets.
  - [CrowdPose](https://github.com/Jeff-sjtu/CrowdPose)
  - [PoseTrack18](https://posetrack.net/)
1. Support more 2D hand keypoint estimation datasets.
  - [InterHand2.6](https://github.com/facebookresearch/InterHand2.6M)
1. Support adversarial training for 3D human shape recovery.
1. Support multi-stage losses.
1. Support mpii demo.

**New Features**

- Support [CrowdPose](https://github.com/Jeff-sjtu/CrowdPose) dataset ([\#195](https://github.com/open-mmlab/mmpose/pull/195))
- Support [PoseTrack18](https://posetrack.net/) dataset ([\#220](https://github.com/open-mmlab/mmpose/pull/220))
- Support [InterHand2.6](https://github.com/facebookresearch/InterHand2.6M) dataset ([\#202](https://github.com/open-mmlab/mmpose/pull/202))
- Support adversarial training for 3D human shape recovery ([\#192](https://github.com/open-mmlab/mmpose/pull/192))
- Support multi-stage losses ([\#204](https://github.com/open-mmlab/mmpose/pull/204))

**Bug Fixes**

- Fix config files ([\#190](https://github.com/open-mmlab/mmpose/pull/190))

**Improvements**

- Add mpii demo ([\#216](https://github.com/open-mmlab/mmpose/pull/216))
- Improve README ([\#181](https://github.com/open-mmlab/mmpose/pull/181), [\#183](https://github.com/open-mmlab/mmpose/pull/183), [\#208](https://github.com/open-mmlab/mmpose/pull/208))
- Support return heatmaps and backbone features ([\#196](https://github.com/open-mmlab/mmpose/pull/196), [\#212](https://github.com/open-mmlab/mmpose/pull/212))
- Support different return formats of mmdetection models ([\#217](https://github.com/open-mmlab/mmpose/pull/217))

## v0.7.0 (30/9/2020)

**Highlights**

1. Support HMR for 3D human shape recovery.
1. Support WholeBody human pose estimation.
  - [COCO-WholeBody](https://github.com/jin-s13/COCO-WholeBody)
1. Support more 2D hand keypoint estimation datasets.
  - [Frei-hand](https://lmb.informatik.uni-freiburg.de/projects/freihand/)
  - [CMU Panoptic HandDB](http://domedb.perception.cs.cmu.edu/handdb.html)
1. Add more popular backbones & enrich the [modelzoo](https://mmpose.readthedocs.io/en/latest/model_zoo.html)
  - ShuffleNetv2
1. Support hand demo and whole-body demo.

**New Features**

- Support HMR for 3D human shape recovery ([\#157](https://github.com/open-mmlab/mmpose/pull/157), [\#160](https://github.com/open-mmlab/mmpose/pull/160), [\#161](https://github.com/open-mmlab/mmpose/pull/161), [\#162](https://github.com/open-mmlab/mmpose/pull/162))
- Support [COCO-WholeBody](https://github.com/jin-s13/COCO-WholeBody) dataset ([\#133](https://github.com/open-mmlab/mmpose/pull/133))
- Support [Frei-hand](https://lmb.informatik.uni-freiburg.de/projects/freihand/) dataset ([\#125](https://github.com/open-mmlab/mmpose/pull/125))
- Support [CMU Panoptic HandDB](http://domedb.perception.cs.cmu.edu/handdb.html) dataset ([\#144](https://github.com/open-mmlab/mmpose/pull/144))
- Support H36M dataset ([\#159](https://github.com/open-mmlab/mmpose/pull/159))
- Support ShuffleNetv2 ([\#139](https://github.com/open-mmlab/mmpose/pull/139))
- Support saving best models based on key indicator ([\#127](https://github.com/open-mmlab/mmpose/pull/127))

**Bug Fixes**

- Fix typos in docs ([\#121](https://github.com/open-mmlab/mmpose/pull/121))
- Fix assertion ([\#142](https://github.com/open-mmlab/mmpose/pull/142))

**Improvements**

- Add tools to transform .mat format to .json format ([\#126](https://github.com/open-mmlab/mmpose/pull/126))
- Add hand demo ([\#115](https://github.com/open-mmlab/mmpose/pull/115))
- Add whole-body demo ([\#163](https://github.com/open-mmlab/mmpose/pull/163))
- Reuse mmcv utility function and update version files ([\#135](https://github.com/open-mmlab/mmpose/pull/135), [\#137](https://github.com/open-mmlab/mmpose/pull/137))
- Enrich the modelzoo ([\#147](https://github.com/open-mmlab/mmpose/pull/147), [\#169](https://github.com/open-mmlab/mmpose/pull/169))
- Improve docs ([\#174](https://github.com/open-mmlab/mmpose/pull/174), [\#175](https://github.com/open-mmlab/mmpose/pull/175), [\#178](https://github.com/open-mmlab/mmpose/pull/178))
- Improve README ([\#176](https://github.com/open-mmlab/mmpose/pull/176))
- Improve version.py ([\#173](https://github.com/open-mmlab/mmpose/pull/173))

## v0.6.0 (31/8/2020)

**Highlights**

1. Add more popular backbones & enrich the [modelzoo](https://mmpose.readthedocs.io/en/latest/model_zoo.html)
  - ResNext
  - SEResNet
  - ResNetV1D
  - MobileNetv2
  - ShuffleNetv1
  - CPM (Convolutional Pose Machine)
1. Add more popular datasets:
  - [AIChallenger](https://arxiv.org/abs/1711.06475?context=cs.CV)
  - [MPII](http://human-pose.mpi-inf.mpg.de/)
  - [MPII-TRB](https://github.com/kennymckormick/Triplet-Representation-of-human-Body)
  - [OCHuman](http://www.liruilong.cn/projects/pose2seg/index.html)
1. Support 2d hand keypoint estimation.
  - [OneHand10K](https://www.yangangwang.com/papers/WANG-MCC-2018-10.html)
1. Support bottom-up inference.

**New Features**

- Support [OneHand10K](https://www.yangangwang.com/papers/WANG-MCC-2018-10.html) dataset ([\#52](https://github.com/open-mmlab/mmpose/pull/52))
- Support [MPII](http://human-pose.mpi-inf.mpg.de/) dataset ([\#55](https://github.com/open-mmlab/mmpose/pull/55))
- Support [MPII-TRB](https://github.com/kennymckormick/Triplet-Representation-of-human-Body) dataset ([\#19](https://github.com/open-mmlab/mmpose/pull/19), [\#47](https://github.com/open-mmlab/mmpose/pull/47), [\#48](https://github.com/open-mmlab/mmpose/pull/48))
- Support [OCHuman](http://www.liruilong.cn/projects/pose2seg/index.html) dataset ([\#70](https://github.com/open-mmlab/mmpose/pull/70))
- Support [AIChallenger](https://arxiv.org/abs/1711.06475?context=cs.CV) dataset ([\#87](https://github.com/open-mmlab/mmpose/pull/87))
- Support multiple backbones ([\#26](https://github.com/open-mmlab/mmpose/pull/26))
- Support CPM model ([\#56](https://github.com/open-mmlab/mmpose/pull/56))

**Bug Fixes**

- Fix configs for MPII & MPII-TRB datasets ([\#93](https://github.com/open-mmlab/mmpose/pull/93))
- Fix the bug of missing `test_pipeline` in configs ([\#14](https://github.com/open-mmlab/mmpose/pull/14))
- Fix typos ([\#27](https://github.com/open-mmlab/mmpose/pull/27), [\#28](https://github.com/open-mmlab/mmpose/pull/28), [\#50](https://github.com/open-mmlab/mmpose/pull/50), [\#53](https://github.com/open-mmlab/mmpose/pull/53), [\#63](https://github.com/open-mmlab/mmpose/pull/63))

**Improvements**

- Update benchmark ([\#93](https://github.com/open-mmlab/mmpose/pull/93))
- Add Dockerfile ([\#44](https://github.com/open-mmlab/mmpose/pull/44))
- Improve unittest coverage and minor fix ([\#18](https://github.com/open-mmlab/mmpose/pull/18))
- Support CPUs for train/val/demo ([\#34](https://github.com/open-mmlab/mmpose/pull/34))
- Support bottom-up demo ([\#69](https://github.com/open-mmlab/mmpose/pull/69))
- Add tools to publish model ([\#62](https://github.com/open-mmlab/mmpose/pull/62))
- Enrich the modelzoo ([\#64](https://github.com/open-mmlab/mmpose/pull/64), [\#68](https://github.com/open-mmlab/mmpose/pull/68), [\#82](https://github.com/open-mmlab/mmpose/pull/82))

## v0.5.0 (21/7/2020)

**Highlights**

- MMPose is released.

**Main Features**

- Support both top-down and bottom-up pose estimation approaches.
- Achieve higher training efficiency and higher accuracy than other popular codebases (e.g. AlphaPose, HRNet)
- Support various backbone models: ResNet, HRNet, SCNet, Houglass and HigherHRNet.
