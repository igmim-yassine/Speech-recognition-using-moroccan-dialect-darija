# Fine-Tuning-of-XLSR-Wav2Vec2-on-Moroccan-Dialect-Darija

This project is about speech to text using moroccan dialect darija. In fact, MSA dataset and Moroccan speech corpus are not that different from each other. There is not a stark differnece between them, thig that help stand us in good stead to well tackle the issue of recognition.

* The model was pretrained using 53 languanges :


The XLSR model uses the following datasets for multilingual pretraining:

* MLS: Multilingual LibriSpeech (8 languages, 50.7k hours): Dutch, English, French, German, Italian, Polish, Portuguese, Spanish

* CommonVoice (36 languages, 3.6k hours): Arabic, Basque, Breton, Chinese (CN), Chinese (HK), Chinese (TW), Chuvash, Dhivehi, Dutch, English, Esperanto, Estonian, French, German, Hakh-Chin, Indonesian, Interlingua, Irish, Italian, Japanese, Kabyle, Kinyarwanda, Kyrgyz, Latvian, Mongolian, Persian, Portuguese, Russian, Sakha, Slovenian, Spanish, Swedish, Tamil, Tatar, Turkish, Welsh (see also finetuning splits from this paper).

* Babel (17 languages, 1.7k hours): Assamese, Bengali, Cantonese, Cebuano, Georgian, Haitian, Kazakh, Kurmanji, Lao, Pashto, Swahili, Tagalog, Tamil, Tok, Turkish, Vietnamese, Zulu




and fine-tuned using Arabic classic speech corpus of [common voice](https://commonvoice.mozilla.org/ar) that is about 12 hours of speech.

The model was not that performant because of the lack of data used to fine tuning the model with the moroccan dialect darija, so that is why we tried to improve its performance by increasing the dataset used for the fine-tuning. To do so, we used this application to make the task much faster :

[Applciation desktop for labelisation](https://github.com/igmim-yassine/speech-training-recorder)


<p align="center">
  <img src="https://i.ibb.co/tPrSfrF/c92ec977-721c-4991-a64b-b6f3cef50bd7.jpg" />
</p>


Finally, we end up building the model, that uses wav2vec2.0 to do speech2text. The problem was that using the custom dataset gives nothing.

As a resolution of the project, we will use the dataset of dvoice.ma that well be released soon and then the model will be fine-tuned by moroccan darija. But now all what we did is try to transcript audios of darija using pretrained wav2vec-large-53 fine-tuned with 12 hourse of MSA.

# Useful Links:

https://github.com/pytorch/fairseq/tree/master/examples/wav2vec#wav2vec-20
https://huggingface.co/anas/wav2vec2-large-xlsr-arabic
https://commonvoice.mozilla.org/en/datasets
https://discuss.huggingface.co/t/open-to-the-community-xlsr-wav2vec2-fine-tuning-week-for-low-resource-languages/4467
https://github.com/huggingface/transformers/blob/master/examples/research_projects/wav2vec2/FINE_TUNE_XLSR_WAV2VEC2.md
https://github.com/saobou/arabic-text-preprocessing/blob/master/Preprocess.ipynb
