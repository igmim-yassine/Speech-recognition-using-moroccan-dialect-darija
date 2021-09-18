# Fine-Tuning-of-XLSR-Wav2Vec2-on-Moroccan-Dialect-Darija

This project is about speech to text using moroccan dialect darija. In fact, MSA dataset and Moroccan speech corpus are not that different from each other. There is no a stark differnece between them, thig that help stand us in good stead to well thackle the issue in question.

The model was pretrained using Arabic classic speech corpus of [common voice](https://commonvoice.mozilla.org/ar) which is about 12 hours of speech, and then fine-tuning it using just 8 min of moroccan darija.

The model was not that performant because of the lack of data used to fine tuning the model, so that is why we tried to improve its performance by increasing the dataset used for the fine-tuning. To do so, we used this application to make the task much faster :

[Applciation desktop for labelisation](https://github.com/igmim-yassine/speech-training-recorder)

<p align="center">
  <img src="https://i.ibb.co/tPrSfrF/c92ec977-721c-4991-a64b-b6f3cef50bd7.jpg" />
</p>

This model uses wav2vec2.0 to do speech2text. The problem was that using the custom dataset gives nothing.

As a resolution of the project, we will use the dataset of dvoice.ma that well be realesed soon and then the model will be pretrained by moroccan darija and also fine-tuning with it as well. But now all what we did is try to transcript audios of darija using pretrained wav2vec-large-53 fine-tuned with 12 hourse of MSA.

# Useful Links:

https://huggingface.co/anas/wav2vec2-large-xlsr-arabic
https://commonvoice.mozilla.org/en/datasets
https://discuss.huggingface.co/t/open-to-the-community-xlsr-wav2vec2-fine-tuning-week-for-low-resource-languages/4467
https://github.com/huggingface/transformers/blob/master/examples/research_projects/wav2vec2/FINE_TUNE_XLSR_WAV2VEC2.md
https://github.com/saobou/arabic-text-preprocessing/blob/master/Preprocess.ipynb
