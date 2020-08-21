# hyperdimentions

make 4 folders
1. data
2. example_clips
3. model
4. output

data: will contain 2 sub folders a) safe for work  b) not safe for work 
example_clip will contain sample clip to test out model on
model: will contain saved location of model file
output: will contain inference

To train your code make this structure and run:
 python3 train.py --dataset data/ --model model/activity.model --label-bin model/lb.pickle --epoch 20


To test run:
python3 predict_video.py --model model/activity.model --label-bin model/lb.pickle --input example_clips/output.mp4 --output output/128fps.avi --size 128
