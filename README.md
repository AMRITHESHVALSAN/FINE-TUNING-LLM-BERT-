# FINE TUNING LLM USING LoRA and PEFT
We will use the Hugging Face ecosystem to fine-tune a Large Language Model to classify text as ‘positive’ or ‘negative’. Here, we fine-tune distilbert-base-uncased, a ~70M parameter model based on BERT. Since this base model was trained to do language modeling and not classification, we employ transfer learning to replace the base model head with a classification head. Additionally, we use **LoRA and PEFT** to fine-tune the model efficiently enough that it can run on my system(HP intel core i5) in a reasonable amount of time (~20 min).

We use a dataset of movie reviews and train the LLM to classify the  reviews as Positiveor negative


While fine-tuning an existing model requires more computational resources and technical expertise than using one out-of-the-box, (smaller) fine-tuned models can outperform (larger) pre-trained base models for a particular use case, even when employing clever prompt engineering strategies.
