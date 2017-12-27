# SSBM Fox Detector

## About

A [keras](https://keras.io/) FRCNN to detect Fox in Super Smash Bros Melee for the Nintendo Gamecube.  The FRCNN object detector was written by [yhenon](https://github.com/yhenon) and the orignal repo can be seen [here](https://github.com/yhenon/keras-frcnn).  The gameplay used to train and test the model is from VGBootcamp ([twitch](https://www.twitch.tv/vgbootcamp) & [youtube](https://www.youtube.com/channel/UCj1J3QuIftjOq9iv_rr7Egw)).  The model was trained on the [AMI provided by PyImageSearch](https://www.pyimagesearch.com/2017/09/20/pre-configured-amazon-aws-deep-learning-ami-with-python/).

[This google drive folder](https://drive.google.com/drive/folders/17QcuO9GQsiqO_4V86iV1gBGUCCfbPkUm) has the trained the model file, `model_frcnn.hdf5`.  The folder also has the training data, `data.zip`, which contains a folder of images in addition to bounding box annotations produced by [dlib's imglab](https://github.com/davisking/dlib/tree/master/tools/imglab) (these annotations were converted to `fox_frcnn_tags.txt` for compatibility with the frcnn scripts).  Lastly the folder has a .zip containing images with bounding boxes drawn by the trained model, `results_imgs.zip`.

## Output

This gif shows the output of the model.  The model works with still images 1 at time; a sample of these single frame outputs were then converted into the gif.

![](readme/kjh_plup_vgbc_tbh7_fox_detect2.gif)
