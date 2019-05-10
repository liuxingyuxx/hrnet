## DEMO
```
python pose_estimation/video.py
-o output_name
-i /path/to/video -o output_name
--display # 显示出来(display in screen)
--camera # 通过网络摄像头作为视频的输入(open web camera by video input)

python pose_estimation/demo.py (for image)
```

<br><br>
## UPDATE 2019-05-21
<br>
1. add high mAP mmdetection
`python pose_estimation/demo_mmd.py`
<br>
2. do RP accuracy  test
`cd tools && ./eval_coco.sh`
<br>
3. add simple tracking function 
`python pose_estimation/pose_track.py`
<br>

<br><br>
## imporove from origin code

```
# 通过flow net2来平滑视频(smooth pose joints by flownet2)
python pose_estimation/smooth_flownet.py

# 通过SGfilter, 最小二乘法和低次多项式平滑视频 (smooth pose joints by SG-filter)
python pose_estimation/smooth-sg.py

```
<br>
[todo]
 > 使用flownet2来实现视频姿态track(add tracking module by flownet2)


---


`original code`
clone from https://github.com/leoxiaobin/deep-high-resolution-net.pytorch
