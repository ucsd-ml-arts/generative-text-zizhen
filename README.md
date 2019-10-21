# Project 1 Generative Text

Zizhen Wang, ziw142@ucsd.edu



## Abstract

This project I will work on one type of chinese fantasy novel such as swordsman stories. A lot of American people like Asian novel or fiction because these novels are different from American novels. My learning data is from a website which some volunteers transform the novel to English version. I want our module could learn some specific seeting or scenario and generate some chinese fantsy novel. My tranning data is a book called Steller Transformations which is very popular chinese fantasy novel in America. I plan to use RNN model to generate the text. My goal is the generating text would keep the same interesting narrative style.

## Model/Data


- trained models: RNN, website scarper
- training data ：Stellar Transformations: https://www.wuxiaworld.com/novel/stellar-transformations
## Code

My web scrape code is webscraper.ipynb
Both my training code and the generation code are inside the Text_Generation_RNN.ipynb.


## Results

- Documentation of your generative text in an effective form. A file with your generated text (.pdf, .doc, .txt). 

## Technical Notes

- When I used the whole book which the text file would be very large, and then the running time would be very long.
It could choose some part of the book which will increase the running time.
- The code requires TensorFlow, NumPy and IPython libraries. It is recommended to run the code on a platform/computer that has sufficient GPU power since the training phase will occupy much computing power.

## Reference

- Papers
  - the fundamental concepts underlying RNNs: https://www.oreilly.com/library/view/neural-networks-and/9781492037354/ch04.html
  - Variable importance in RNN or LSTM: https://stats.stackexchange.com/questions/191855/variable-importance-in-rnn-or-lstm https://stats.stackexchange.com/questions/191855/variable-importance-in-rnn-or-lstm
