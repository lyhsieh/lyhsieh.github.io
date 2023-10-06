---
layout: page
title: MeiChu Hackathon
description: 2020 梅竹黑客松
img: assets/img/proj_preview/meichu.jpg
importance: 1
category: Competition
giscus_comments: true
---

## Date
2020/10/24 (Sat.) - 2020/10/25 (Sun.)

## Topic
<a href="https://www.logitech.com/zh-tw" target="_blank">Logitech International</a>: <b>Ethical gaming world</b>

## Motivation
There are increasingly more online games in recent years. When playing, we don’t want to encounter cheating behaviors that will decrease our will to play. Thus, we want to develop a <b>cheating detection system</b> that can detect unethical actions in online games.

## Members

* Handsome Leo (Me)
* <a href="https://bwbwchen.github.io/" target="_blank">Bo-Wei Chen</a>
* <a href="https://github.com/Jack24658735" target="_blank">Jack Liu</a>
* <a href="https://github.com/bowen1248" target="_blank">Bowen Lee</a>
* <a href="https://github.com/HowardWang0915" target="_blank">Howard Wang</a>


## Ways of “Cheating”
* gaming hack
* AFK (away from keyboard)
* ask other people to play
* etc

## Solution: Machine Learning
We surveyed a [paper [1]](assets/img/meichu/paper.pdf) focusing on remote suspicious mouse intrusion, which gave us some inspiration. We believed that when a player cheats in a game, the mouse track must be different. So, we used <b>random forest</b> to train a <b>one-class classifier</b>, excepting the model after training could tell whether the input mouse track comes from the same person. By doing so, no matter the player installs gaming hack or asks his/her friends to play for him/her, our system could always tell us that the behavior was abnormal. Visit our [presentation file](assets/img/meichu/presentation.pdf) for detailed descriptions.

<img src="assets/img/meichu/flow.png">

## Data Collection and Preprocessing
* Game: CS-GO
* Type: First-person shooter (FPS) game
* Repository: Link
* Data recording: Python

<img src="assets/img/meichu/collect.png">

## Awards
Out of hundreds of people, We won the <b>FIRST place</b> of Logitech and the <b>FIRST place</b> in the second round competing with other champions from other enterprises including <a href="https://linecorp.com/zh-hant/" target="_blank">LINE</a> and <a href="https://tw.micron.com/" target="_blank">Micron Taiwan</a>. We were guaranteed to join the summer internship of Logitech and were reported in news.

<img src="assets/img/meichu/first_I.jpeg">
<img src="assets/img/meichu/first_II.jpeg">

## Certificates of Merit
<div style="margin:0 auto;">
  <img style="width:50%;height:auto;display:inline-block;margin-left:-4px;" src="assets/img/meichu/cert1.png">
  <img style="width:50%;height:auto;display:inline-block;margin-left:-4px;" src="assets/img/meichu/cert2.png">
</div>

## Related News
* <a href="https://dep-labor.hccg.gov.tw/ch/home.jsp?id=7&parentpath=0,1&mcustomize=municipalnews_view.jsp&toolsflag=Y&dataserno=202010250004&t=MunicipalNews&mserno=201601300117" target="_blank">HsinChu Goverment News</a>

* <a href="https://www.ettoday.net/news/20201026/1840005.htm" target="_blank">ETtoday News</a>

## Repository
* <a href="https://github.com/LeoTheBestCoder/Meichu2020_Team_726" target="_blank">Link</a>

## Reference
[1] M. Antal and E. Egyed-Zsigmond. Intrusion Detection Using Mouse Dynamics. 2018




