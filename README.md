# Project 1 Generative Text

Zizhen, ziw142@ucsd.edu

## Abstract

This project I will work on one type of chinese fantasy novel such as swordsman stories. A lot of American people like Asian novel or fiction because these novels are different from American novels. My learning data is from a website which some volunteers transform the novel to English version. I want our module could learn some specific seeting or scenario and generate some chinese fantsy novel. My tranning data is a book called stellar-transformations which is very popular chinese fantasy novel in America. I plan to use RNN model to generate the text. My goal is the generating text would keep the same interesting narrative style.
## Model/Data


- trained models:RNN and website scraper
- training data: stellar-transformations :https://www.wuxiaworld.com/novel/stellar-transformations
## Code


- Both my training code and the generation code are inside the Text_Generation_RNN.ipynb.
- My website scrape code is inside the Webscraper.ipynb

## Results

- Documentation of your generative text in an effective form. A file with your generated text (.pdf, .doc, .txt). 

## Technical Notes


- Since the novel is very large book so when I train it, the running time is much longer. If you want to decrease the running time, you could choose part of text file, but the accuracy may decrease. And also, the loss is not constantly decrease when the epochs increases, I recommend choose the epoch number when the loss is least.
- The code requires TensorFlow, NumPy and IPython libraries. I also recommended to run the code on a platform/computer that has sufficient GPU power since the training phase occupy much computing power.

## Reference

References to any papers, techniques, repositories you used:
- Papers
  - [This is a paper](this_is_the_link.pdf)
- Repositories
- Blog posts
