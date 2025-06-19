# Shakespeare-Bot

The objective of this project is to train a generative language model capable of producing original text in the poetic style of Shakespeare. The models take a prompt as an input and return a sentence in the aforementioned style. To achieve this, we will implement and compare two types of models: a recurrent neural network (LSTM RNN) and a transformer-based (GPT-2) model. 

The RNN serves as a baseline due to its simplicity, while the transformer offers a modern, attention-based approach known for superior performance in capturing long-range dependencies in text. This comparison allows us to evaluate the trade-offs between model complexity, training efficiency, and generation quality in the context of text generation.

The trained LSTM model is saved in the github repo with other documents from the project. If you want to use the model, you dont need to retrain unless you want to try different hyperparamters or design.

The GPT2-transformer model is a pr-trained model from [huggingface Open AI community ](https://huggingface.co/openai-community/gpt2). The model was tuned (transfer learning) by the [Shakespeare plays](https://www.kaggle.com/datasets/kingburrito666/shakespeare-plays) dataset from kaggle, containing over 100,000 lines of dialogue attributed to individual characters across various works. Each line is accompanied by metadata including the play title, act and scene identifiers, and speaker information. 

The tuned GPT-2 model was stored in my [huggingface model repo](https://huggingface.co/Bilal1jk/Shakespeare-Bot). This gives any user access to the tuned model using huggingface API. This eliminated the need for re-trainning which can be costly.

GPUs from Kaggle and google colab were utilized to train both the LSTM RNN and GPT-2 transformer models.

Measuring accuracy in generative models can be tricky. Althoug discriminators can help tune, improve and compare the models but due to the limited time and GPU resources, that was not utilized. We instead relied on the common qualitative approach of evaluating the generated samples. Since all models are pre-trained, feel free to use your own words and compare the two models in your local.

[Github Repo](https://github.com/Bilal1k/Shakespeare_Bot)
