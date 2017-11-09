![Darknet Logo](http://pjreddie.com/media/files/darknet-black-small.png)

# whos_he
- Originally forked by darknet
- link is here : https://pjreddie.com/darknet/yolo/
- github of yolo : https://github.com/pjreddie/darknet
- OpenCV : 2.4.9
- CUDA : 8.0
- cuDNN : 5.1
- You need to complile with CUDA & OpenCV (doesn't matter about cuDNN)
- trained by coco and https://mega.nz/#F!GRV1XKbJ!v8BCsFO8iJVNppiGXY4qMw

This program detects face and pedestrian. if it found face, mosaic this area.

check this video : https://youtu.be/VwBazA7Ykv4?t=6m46s

# how to install
- $ cat backup.tar.gz* | tar xzvf -
- $ make (if you don't have cuDNN, change Makefile cuDNN = 1 to 0)
- $ ./darknet detector demo cfg/coco.data cfg/yolo.cfg backup/yolo_9200.weights
- You can also run it on a video file.
- $ ./darknet detector demo cfg/coco.data cfg/yolo.cfg backup/yolo_9200.weights <video file>
- You can change threshold value.
- $ ./darknet detector demo cfg/coco.data cfg/yolo.cfg backup/yolo_9200.weights -thresh <num>
