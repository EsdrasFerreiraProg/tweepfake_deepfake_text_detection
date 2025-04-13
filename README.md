This repository contains the scripts used to perform experimentation described in https://arxiv.org/abs/2008.00036 :

**Title**: "TweepFake: about Detecting Deepfake Tweets"

**Authors**: Tiziano Fagni, Fabrizio Falchi, Margherita Gambini, Antonio Martella, Maurizio Tesconi

**Abstract**: The threat of deepfakes, synthetic, or manipulated media, is becoming increasingly alarming, especially for social media platforms that have already been accused of manipulating public opinion. Even the cheapest text generation techniques (e.g. the search-and-replace method) can deceive humans, as the Net Neutrality scandal proved in 2017. Meanwhile, more powerful generative models have been released, from RNN-based methods to the GPT-2 language model. State-of-the-art language models, transformer-based in particular, can generate synthetic text in response to the model being primed with arbitrary input. Thus, Therefore, it is crucial to develop tools that help to detect media authenticity. 
To help the research in this field, we collected a dataset of real Deepfake tweets. It is real in the sense that each deepfake tweet was actually posted on Twitter. We collected tweets from a total of 23 bots, imitating 17 human accounts. The bots are based on various generation techniques, i.e., Markov Chains, RNN, RNN+Markov, LSTM, GPT-2. We also randomly selected tweets from the humans imitated by the bots to have an overall balanced dataset of 25,836 tweets (half human and half bots generated). The dataset is publicly available on Kaggle. 
In order to create a solid baseline for detection techniques on the proposed dataset we tested 13 detection methods based on various state-of-the-art approaches. The detection results reported as a baseline using 13 detection methods, confirm that the newest and more sophisticated generative methods based on transformer architecture (e.g., GPT-2) can produce high-quality short texts, difficult to detect.


*NOTE*: All the experiments have been performed using Google Colaboratory platform and Google Drive integration, if you want to run the scripts under different conditions you need to change the code accordingly.

**Added by @EsdrasFerreiraProg

1. Install Python 3.6.8 - https://www.python.org/downloads/release/python-368/
2. Create a virtual environment with Python 3.6.8 - python.exe -m venv venv // maybe other commands will be necessary
3. Activate the venv - .\venv\Scripts\activate
4. Verify if pip is installed - pip --version
4.1 - If it is not, do 
python -m ensurepip --upgrade
python -m pip install --upgrade pip
5. Install the requirements file called requirements-char-cnn.txt
6. Run this command, it will fix some compatibilities problems: pip install notebook==6.4.0 jinja2==2.11.3 nbclient==0.5.9 nbconvert==6.0.7
7. Now install jupyter - jupyter notebook