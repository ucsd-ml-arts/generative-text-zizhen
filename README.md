# Project 1 Generative Text

Zizhen, ziw142@ucsd.edu

## Abstract

This project I will work on one type of chinese fantasy novel such as swordsman stories. A lot of American people like Asian novel or fiction because these novels are different from American novels. My learning data is from a website which some volunteers transform the novel to English version. I want our module could learn some specific seeting or scenario and generate some chinese fantsy novel. My tranning data is a book called stellar-transformations which is very popular chinese fantasy novel in America. I plan to use RNN model to generate the text. My goal is the generating text would keep the same interesting narrative style.
![](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/pic.jpg)
## Model/Data


- trained models:RNN and website scraper
- training data: stellar-transformations :https://www.wuxiaworld.com/novel/stellar-transformations
## Code


- Both my training code and the generation code are inside the [Text_Generation_RNN.ipynb](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/Text_Generation_RNN.ipynb).
- My website scrape code is inside the [Webscraper.ipynb](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/Webscraper.ipynb).

## Results

- [results.txt](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/result.txt)

The output have readable sentences, and it also have a lot of setting and scenario such as specific talking to show the narrative style. I think that was fit my goal to show a different vision for chinese fiction.
I used epoch number is 20.
sequence legth is 200.
And tempreture is 0.3.

## Technical Notes


- Since the novel is very large book so when I train it, the running time is much longer. If you want to decrease the running time, you could choose part of text file, but the accuracy may decrease. And also, the loss is not constantly decrease when the epochs increases, I recommend choose the epoch number when the loss is least.
- The code requires TensorFlow, NumPy and IPython libraries. I also recommended to run the code on a platform/computer that has sufficient GPU power since the training phase occupy much computing power.

## Reference


- Papers
  - the fundamental concepts underlying RNNs : https://www.oreilly.com/library/view/neural-networks-and/9781492037354/ch04.html
  - Variable importance in RNN or LSTM: https://stats.stackexchange.com/questions/191855/variable-importance-in-rnn-or-lstm

