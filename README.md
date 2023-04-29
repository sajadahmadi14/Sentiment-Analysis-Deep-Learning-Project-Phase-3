# Sentiment-Analysis-Deep-Learning-Project-Phase-3
In the final phase of the deep learning project, you will focus on combining image and text modalities to improve emotion recognition. The first step is to concatenate the representation vectors obtained from the image and text data and use them to train a network for emotion recognition.

The second step involves using pre-trained Transformer models as backbones to fine-tune an emotion recognition model. You can refer to articles on this topic or use two examples of multi-modal transformers with trained weights available.

In the second part of this phase, you will work on supervised weakly learning using a multimodality dataset. Suppose you have a large but unlabeled dataset of image-text pairs along with your labeled MSCTD dataset. Your goal is to achieve an image-based emotion recognition model for the unlabeled dataset.

You will take two steps to achieve this goal. First, you will consider an image-based model and a text-based model, and update their FC layers using labeled datasets. Then, you will use the output of the text-based model as a pseudo label to update the weights of the FC layers of the image-based model to match its output.

This approach can improve the performance of the image-based model because linguistic models are generally better at recognizing emotions than faces, and they can create better representations of input text. By involving these good representations in the training process of photo-based emotion recognition, the final model's performance can be improved.

In the second stage, you will freeze the text-based model's weights and use its output as a label to teach the image-based model using weak supervision. This process involves using creative methods to produce noisy and imprecise labels to train and improve the performance of a model on a large set of unlabeled data.

The weakly supervised learning approach allows you to adapt your model to the domain of your unlabeled dataset, even if it is not from the same domain as your labeled dataset. To demonstrate this, you can choose an unlabeled dataset of your choice (e.g., a TV series with subtitles) and compare the performance of your image-based model trained via domain adaptation learning supervised weakly to the case where it is only trained from the image itself and its corresponding label.
