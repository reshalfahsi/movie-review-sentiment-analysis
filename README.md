# Movie Review Sentiment Analysis Using CNN and MLP


 <p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/cnn-mlp-white.png" alt="CNN-MLP" > A diagram of the CNN-MLP model. </p>


Audiences' reactions to the movie they have watched can be presented in a text format called reviews. These reviews can be polarized into two clusters: positive responses and negative responses. Using CNN and MLP, one can perform sentiment analysis on movie reviews to automatically recognize the viewer's tendency toward a particular movie. CNN is used for extracting the latent information within the text format. MLP leverages the extracted information of CNN and carries out the classification task. The CNN-MLP model is evaluated with Standford's IMBD Movie Review dataset. On the test set, the model achieves ``85.6%`` accuracy.


## Experiment

To run the experiment, [click here](https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/Movie_Review_Sentiment_Analysis_Using_CNN_and_MLP.ipynb).


## Result

### Quantitative Result
The model's performance is measured by the accuracy and loss value. These values are computed regarding the sentiment analysis of the model on the dataset. The loss value is calculated based on the loss function employed in the training process which is the cross-entropy loss.

Dataset Split | Accuracy | Loss
------------ | ------------- | -------------
Train | 94.1% | 0.347 
Validation | **96.5%** | **0.331**
Test | 85.6% | 0.454


### Accuracy and Loss Curve

 <p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/accuracy_curve.png" alt="acc_curve" > <br /> Accuracy curve on the train set and the validation set. </p>
 
  <p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/loss_curve.png" alt="loss_curve" > <br /> Loss curve on the train set and the validation set. </p>

### CNN Visualization

To understand what CNN sees in deciding whether it is a positive or negative opinion, the GradCAM and TAHV visualization techniques are employed.

#### Positive Review

<p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/pos_CNN0.png" alt="pos_CNN0" > Visualization of the first layer of CNN on the positive review. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/pos_CNN1.png" alt="pos_CNN1" > Visualization of the second layer of CNN on the positive review. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/pos_CNN2.png" alt="pos_CNN2" > Visualization of the third layer of CNN on the positive review. </p>

#### Negative Review

<p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/neg_CNN0.png" alt="neg_CNN0" > Visualization of the first layer of CNN on the negative review. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/neg_CNN1.png" alt="neg_CNN1" > Visualization of the second layer of CNN on the negative review. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/movie-review-sentiment-analysis/blob/master/assets/neg_CNN2.png" alt="neg_CNN2" > Visualization of the third layer of CNN on the negative review. </p>

## Credit

- [Text Classification from Scratch](https://keras.io/examples/nlp/text_classification_from_scratch)
- [Standford's IMBD Movie Review](https://ai.stanford.edu/~amaas/data/sentiment/)
- [VLC University of Southampton GradCAM](https://colab.research.google.com/github/ecs-vlc/fmix/blob/master/notebooks/grad_cam.ipynb)
- [University of Toronto GradCAM](https://colab.research.google.com/github/csc413-uoft/2021/blob/master/assets/tutorials/tut04_cnn.ipynb)
- [TAHV：Text Attention Heatmap Visualization](https://github.com/jiesutd/Text-Attention-Heatmap-Visualization)
