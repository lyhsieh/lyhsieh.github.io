---
layout: page
title: MeiChu Hackathon
description: 2020 梅竹黑客松
img: assets/img/proj_preview/meichu.jpg
importance: 1
category: 
giscus_comments: false
related_publications: antal2018intrusion
---

## Date
2020/10/24 (Sat.) - 2020/10/25 (Sun.)

## Topic
<a href="https://www.logitech.com/zh-tw" target="_blank">Logitech International</a>: <b>Ethical gaming world</b>

## Motivation
There are increasingly more online games in recent years. When playing, we don’t want to encounter cheating behaviors that will decrease our will to play. Thus, we want to develop a <b>cheating detection system</b> that can detect unethical actions in online games.

## Members

* Leo (Me)
* <a href="https://bwbwchen.github.io/" target="_blank">Bo-Wei Chen</a>
* <a href="https://jack24658735.github.io/" target="_blank">Jack Liu</a>
* <a href="https://github.com/bowen1248" target="_blank">Bowen Lee</a>
* <a href="https://github.com/HowardWang0915" target="_blank">Howard Wang</a>


## Ways of “Cheating”
* gaming hack
* AFK (away from keyboard)
* ask other people to play
* etc

## Solution: Machine Learning
We surveyed a [paper](../../assets/img/meichu/paper.pdf) focusing on remote suspicious mouse intrusion, which gave us some inspiration. We believed that when a player cheats in a game, the mouse track must be different. So, we used <b>random forest</b> to train a <b>one-class classifier</b>, excepting the model after training could tell whether the input mouse track comes from the same person. By doing so, no matter the player installs gaming hack or asks his/her friends to play for him/her, our system could always tell us that the behavior was abnormal. Visit our [presentation file](../../assets/img/meichu/presentation.pdf) for detailed descriptions.

<center>
{% include figure.html path="assets/img/meichu/flow.png" title="flow" class="img-fluid rounded z-depth-1" %}
</center>

## Data Collection and Preprocessing
* Game: CS-GO
* Type: First-person shooter (FPS) game
* Data recording: Python

<center>
{% include figure.html path="assets/img/meichu/collect.png" width="70%" title="collect" class="img-fluid rounded z-depth-1" %}
</center>


## Awards
Out of hundreds of people, We won the <b>FIRST place</b> of Logitech and the <b>FIRST place</b> in the second round competing with other champions from other enterprises including <a href="https://linecorp.com/zh-hant/" target="_blank">LINE</a> and <a href="https://tw.micron.com/" target="_blank">Micron Taiwan</a>. We were guaranteed to join the summer internship of Logitech and were reported in news.


<center>
{% include figure.html path="assets/img/meichu/first_I.jpeg" width="70%" title="first place" class="img-fluid rounded z-depth-1" %}
{% include figure.html path="assets/img/meichu/first_II.jpeg" width="70%" title="first place" class="img-fluid rounded z-depth-1" %}
</center>


## Certificates of Merit
<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/meichu/cert1.png" title="certificate of merit" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/meichu/cert2.png" title="certificate of merit" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Related News
* <a href="https://dep-labor.hccg.gov.tw/ch/home.jsp?id=7&parentpath=0,1&mcustomize=municipalnews_view.jsp&toolsflag=Y&dataserno=202010250004&t=MunicipalNews&mserno=201601300117" target="_blank">HsinChu Goverment News</a>

* <a href="https://www.ettoday.net/news/20201026/1840005.htm" target="_blank">ETtoday News</a>

## Repository
{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo.html repository="lyhsieh/Meichu2020_Team_726" %}
</div>
{% endif %}


<!-- ## Reference
[1] M. Antal and E. Egyed-Zsigmond. Intrusion Detection Using Mouse Dynamics. 2018 -->




