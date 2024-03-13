Scripts and Jupyter notebooks to download and analyse unanswered Parliamentary written questions (PWQs) from [TheyWorkForYou](theyworkforyou.com).

**Project set-up**

```
git clone git@github.com:centreforpublicdata/written-answers.git
cd written-answers
conda create -n written-answers python=3.10
conda activate written-answers
pip install -r requirements.txt
``` 

**How to collect data**

First collect the URLs of written answers from TheyWorkForYou:

    cd scripts
    python3 get_answer_urls.py --year 2023

Then scrape the raw data:

    python3 scrape_urls.py --year 2023
    
**How to run the analysis**

Use [the notebook](https://github.com/centreforpublicdata/written-answers/blob/main/Analyse%20unanswered%20written%20questions%20in%20the%20House%20of%20Commons.ipynb) with your own data stored locally.

**How to cite**

This repo is published under a CC-BY-SA licence, meaning that you may use the code and findings freely in your own research (including commercially) as long as you cite the authors clearly. 

Please cite the repo as follows: _Powell-Smith A., Centre for Public Data, Analysis of Unanswered Questions in the UK Parliament (2022), GitHub repository, https://github.com/centreforpublicdata/written-answers_.

Also, if you remix, adapt, or build upon the material, you must license your modified material under a CC-BY-SA licence.
