# Korean-Counter-speech-TweetIDs

## Abstract
> This study argues for the necessity of a Korean counter-speech dataset for ethical and effective hate speech detection research. Counter-speech is a response to online hate in order to stop the spread of hate speech and is considered an alternative approach to deleting and blocking. However, since counter-speech often employs offensive language or linguistic structures similar to hate speech, even the state-of-the-art hate speech detection models usually classify it as hate speech. This false positive bias risks silencing the language of minorities and their allies. However, the evaluation of Korean hate speech detection models remains untouched due to the absence of a Korean counter-speech dataset. Thus, we introduce the first Korean counter-speech dataset with annotations about target groups. We then tested a Korean hate speech detection model with our dataset, revealing a significant drop in the model’s accuracy from 97.9% to 42.7%.

- 이 레포지터리에는 한국어로 작성된 대항표현 트윗ID 데이터셋과 데이터 구축에 사용된 소스 코드가 포함되어 있습니다. 혐오 표현에 대항하는 트윗을 모으기 위해 [Twint](https://github.com/twintproject/twint) 라이브러리를 사용하였고, 각 트윗에 대해 대상 그룹 정보 주석을 달았습니다. 트위터의 서비스 약관을 준수하기 위해 수집된 트윗의 트윗 ID만 공개하고 있습니다. 그러나 데이터는 비상업적인 연구용으로 공개되어 있습니다. 
- The repository contains a collection of tweets IDs associated with the counter-speech written in Korean. We used [Twint](https://github.com/twintproject/twint) library to gather Tweets countering against hate speech. We classified them and annotated target group information. To comply with Twitter’s [Terms of Service](https://developer.twitter.com/en/developer-terms/agreement-and-policy), we are only publicly releasing the Tweet IDs of the collected Tweets. The data is released for non-commercial research use. 

- 이 레포지터리는 [혐오와 대항: 혐오표현 탐지 모델 평가를 위한 대항표현 데이터셋 구축(Countering the hatred: The counter-speech dataset in Korean for evaluating hate speech detection models)](https://www.dbpia.co.kr/Journal/articleDetail?nodeId=NODE11063346)이라는 이름으로 출판이 완료되었습니다.
- The associated paper to this repository can be found here: [혐오와 대항: 혐오표현 탐지 모델 평가를 위한 대항표현 데이터셋 구축(Countering the hatred: The counter-speech dataset in Korean for evaluating hate speech detection models)](https://www.dbpia.co.kr/Journal/articleDetail?nodeId=NODE11063346)(**written in Korean**)

## Notes About the Data

* 트윗 ID를 이용해 원 트윗을 얻기 위해서는 [Hydrator](https://github.com/DocNow/hydrator)를 사용해야 합니다. Consider using tools such as the [Hydrator](https://github.com/DocNow/hydrator) and [Twarc](https://github.com/DocNow/twarc) to rehydrate the Tweet IDs.
* 하이드레이팅은 시간이 걸리며, 몇몇 트윗은 삭제되었을 수 있습니다. Hydrating may take a while, and *Tweets may have been deleted since our initial collection*. If that is the case, unfortunately you will not be able to get the deleted Tweets from querying Twitter's API. 

# Data Usage Agreement / How to Cite
This dataset is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)). By using this dataset, you agree to abide by the stipulations in the license, remain in compliance with Twitter’s [Terms of Service](https://developer.twitter.com/en/developer-terms/agreement-and-policy), and cite the following manuscript: 

```
박하율, 박현아, 송상헌.(2022).혐오와 대항: 혐오표현 탐지 모델 평가를 위한 대항표현 데이터셋 구축.담화와인지,29(2),1-23.
```
or

```
Park, Hayul, Park, HyunA, Song, Sanghoun.(2022).Countering the hatred: The counter-speech dataset in Korean for evaluating hate speech detection models.Discourse and Cognition,29(2),1-23.
```

BibTeX:
```bibtex
@article{edspia.NODE1106334620220531,
    Title = {혐오와 대항: 혐오표현 탐지 모델 평가를 위한 대항표현 데이터셋 구축.},
    Author = {박하율 (Park, Hayul) and 박현아 (Park, HyunA) and 송상헌 (Song, Sanghoun)},
    Journal = {담화와인지},
    Volume = {29},
    Number = {2},
    Pages = {1 - 23},
    Year = {2022}
}
```

# Inquiries

Please read through the README and the closed issues to see if your question has already been addressed first. 

If you have any questions about this dataset please contact Hayul Park at **hayul7805[at]korea[dot]ac[dot]kr**.

***
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="크리에이티브 커먼즈 라이선스" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />이 저작물은 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">크리에이티브 커먼즈 저작자표시-비영리-동일조건변경허락 4.0 국제 라이선스</a>에 따라 이용할 수 있습니다.
