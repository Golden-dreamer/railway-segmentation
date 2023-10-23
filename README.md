# railway-segmentation
Neural network for detecting rails.
NNs shows good result in semantic segmantation tasks.
# additional actions
- labeling dataset (89 images total) for NN to learn
- GPU was set up for speed up
- data agmentation for generating more data and improve model score
- used pretrained U-NET model from segmentation-models. It will help to converge faster.
# Metric and loss
Appropriate metric for this type of problem is IoU (intersection over Union),  
since I care about matching pixel with rails.
Loss function is Jaccard index (it is the same as IoU, perfect function for this problem).

# Reults
IoU score is about 0.80. Without any augmentation (used augmentation for more lighter model, but score was lower), and openCV tricks( more discussed about them in summary in notebook).
![ScreenShot](images/model_learning.gif)
