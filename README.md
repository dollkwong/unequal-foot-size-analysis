# unequal-foot-size-analysis

This is a project to discover the feasibility of creating a platform to match unequal-foot-sized people (unequal-foot-sizers) for better shoes comsumption experience. It is considered grouped/paired up if one have opposite size difference with another. (E.g `Left 38 + Right 37` is paired up with `Left 37 + Right 38`)
<br>
![Foot drawio (1)](https://github.com/user-attachments/assets/c2138865-afd7-4964-b628-ce9d874c3e3f)


Below dashboard shows the distribution of the interviewees. The interactive dashboard can be accessed [here](https://public.tableau.com/app/profile/doll.kwong/viz/unequal-foot-size/UnequalFootSizers)

![Unequal Foot Sizers (1)](https://github.com/user-attachments/assets/1d9ba037-a54c-4255-b6d2-e11bbb29c130)

## Data Source and Sample Size
Data is collected with a [Google form questionaire](https://forms.gle/8Hsn4z1X7qngCWYG8), with 900 responses from Hong Kong. An English version can be accessed [here](https://forms.gle/hdHtSkWmz9jsh54i6) 

## Data Cleaning
### 1. Translation
The original questionaire is in Chinese. I translated to English with my own language. I was planning to use the `translate` library but the result is not satisfying. 
### 2. Column Addition
In order to more easier to group/pair individuals, two columns are added: `estimated_left_foot_size` and `estimated_left_foot_size`. Two assumptions are made here:
<br>
1. Their usual shoe size is the size of the bigger foot
<br>
2. for feet size difference smaller than 0.5, difference is insignaficant and thus shoe exchange is unnecessary/unfeasible. 
<br>
The smaller foot size is thus calculated by subtracting the difference of two feet.

## Insights
- Among 900 interviewers, over 33% of them are suffering from unequal foot size, and the bigger foot is very evenly distributed between left and right feet. However, a majority of them only hold a difference of 0.25 size (less than 0.5), meaning only 150 interviewees falls within our attention. This takes up 16.7% (1 out of 6). This proportion, to me, is acceptable.
- The unequal-foot-sizers are grouped based on their foot sizes. In this study, non of the men can be paired up, but there are several groups among women. 

## Follow up Actions
As this platform is considered worth going on, the next phase is to understand the preferences of those target audience.
