# Fine-Tuning-of-XLSR-Wav2Vec2-on-Moroccan-Dialect-Darija

This project is about speech to text using moroccan dialect darija. In fact, MSA dataset and Moroccan speech corpus are not that different from each other. This no stark differnece between them help stand us in good stead.

The model was pretrained using Arabic classic speech corpus of common voice that is about 12 hours of speech, and then fine-tuning it using just 8 min of moroccan darija.
The model was not that performant because of the lack of data using to fine tuning the model, so that is why we tried to increase its performance by increasing the dataset used for the fine-tuning. To do so, we used the application follow to make the task much fast  :

https://github.com/igmim-yassine/speech-training-recorder

![alt text](https://i.ibb.co/tPrSfrF/c92ec977-721c-4991-a64b-b6f3cef50bd7.jpg)

<p align="center">
  <img src="https://i.ibb.co/tPrSfrF/c92ec977-721c-4991-a64b-b6f3cef50bd7.jpg" />
</p>


# Useful Links:

https://huggingface.co/anas/wav2vec2-large-xlsr-arabic
https://commonvoice.mozilla.org/en/datasets
https://discuss.huggingface.co/t/open-to-the-community-xlsr-wav2vec2-fine-tuning-week-for-low-resource-languages/4467
https://github.com/huggingface/transformers/blob/master/examples/research_projects/wav2vec2/FINE_TUNE_XLSR_WAV2VEC2.md
https://github.com/saobou/arabic-text-preprocessing/blob/master/Preprocess.ipynb
