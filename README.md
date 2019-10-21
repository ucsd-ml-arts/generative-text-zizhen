# Project 1 Generative Text

Zizhen, ziw142@ucsd.edu

## Abstract

- This project I will work on one type of chinese fantasy novel such as swordsman stories. A lot of American people like Asian novel or fiction because these novels are different from American novels. My learning data is from a website which some volunteers transform the novel to English version. I want our module could learn some specific seeting or scenario and generate some chinese fantsy novel. My tranning data is a book called stellar-transformations which is very popular chinese fantasy novel in America. I plan to use RNN model to generate the text. My goal is the generating text would keep the same interesting narrative style.
![](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/pic.jpg)
- I started to use website scraped code to scrape the book from websites since the website does not provide download work. However, the website seperate each chapter to one url, so I need to collect them together through the for loop.
- Then I used RNN training model to train my novel. The varibles is Epoch number:3; Sequence legth is 100; Tempreture is 1; Number of characters to generate is 1000. The result is bad which means it can not form any readable word. Firstly, I wanted to increase the accuracy so I tried to increase epochs. But even I tried 100 epochs and spent a lot time due to large file, the result is still bad.
- Therefore, after I checked my text file is correct, I paid more attention on varibles for the trainning model.
- The first varible I changed is number of charactrer to generate, becasue I need more words to show a story which could achieve my goal.
- The second varible I changed is number of epochs. I tried 2, 30 , 100. I found the loss is not constantly decrease when the epochs increases, I recommend choose the epoch number when the loss is least. I used 20 epochs because I found the least loss at 20 epochs is about 0.7 but at 100 epochs, the loss went back to 1.3.
- The third varible I changed is temperature. I read some papers which how temperature affects RNN model. The explaination is for high temperatures, all actions have nearly the same probability and the lower the temperature, the more expected rewards affect the probability; for a low temperature, the probability of the action with the highest expected reward tends to 1. So I tried different temperature, when I decrease the tempreture to 0.3, the result showed a readable story. And the least loss at 20 peochs decrease 0.1 from the high temperature so I think it was useful.
- The last things I changed sequence length, I found the loss decreased again. When I increase the number epochs, I found 20 is not best number of epochs. The best number is about 130 when I did 200 epochs which means,  the sequence length will make loss decreasing more stable to show the accuracy increase.
- Finally, my varibles setting is :Epoch number is 20. Sequence legth is 200. Temperature is 0.3. Number of characters to generate is 10000.

## Model/Data


- trained models:RNN and website scraper
- training data: stellar-transformations :https://www.wuxiaworld.com/novel/stellar-transformations
## Code


- Both my training code and the generation code are inside the [Text_Generation_RNN.ipynb](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/Text_Generation_RNN.ipynb).
- My website scrape code is inside the [Webscraper.ipynb](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/Webscraper.ipynb).

## Results

- [results.txt](https://github.com/ucsd-ml-arts/generative-text-zizhen/blob/master/result.txt)

- The output have readable sentences, and it also have a lot of setting and scenario such as specific talking to show the narrative style. I think that was fit my goal to show a different vision for chinese fiction.
- Epoch number is 20.
- Sequence legth is 200.
- Temperature is 0.3.
- Number of characters to generate is 10000.

## Technical Notes


- Since the novel is very large book so when I train it, the running time is much longer. If you want to decrease the running time, you could choose part of text file, but the accuracy may decrease. And also, the loss is not constantly decrease when the epochs increases, I recommend choose the epoch number when the loss is least.
- I also choose the number of character to generate is 10000 since this is fiction. I want more words could show the whole narratvie style.
- The code requires TensorFlow, NumPy and IPython libraries. I also recommended to run the code on a platform/computer that has sufficient GPU power since the training phase occupy much computing power.

## Reference


- Papers
  - the fundamental concepts underlying RNNs : https://www.oreilly.com/library/view/neural-networks-and/9781492037354/ch04.html
  - Variable importance in RNN or LSTM: https://stats.stackexchange.com/questions/191855/variable-importance-in-rnn-or-lstm

