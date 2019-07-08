# Blog3
## Nailed It! Contestant Analysis

This is the code I used behind my blog post, [Would I embarrass myself if I went on Netflix’s *Nailed It?*](https://medium.com/swlh/would-i-embarrass-myself-if-i-went-on-netflixs-nailed-it-9e3ae8ff6b5a)

The goal of this post was to create a classification model that could predict whether or not an individual (primarily myself) would embarrass themselves on the show. I manually compiled data from every episode of *Nailed It!*; however, because I was making quick guesses and judgements about strangers, I have decided NOT to share the data behind this model. 

I will, however, share the data dictionary for the relevant variables to my model : 
#### Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|embarrassed|int|df|My opinion on whether or not the contestant embarrassed himself or herself, 0 = did not embarrass, 1 = embarrassed a little or embarrassed a lot|
|baking_experience|int|df|Contestant's confidence in baking skills (High = 1, Low =0)| 
|decorating_experience|int|df|Contestant's confidence in decorating skills (High = 1, Low =0)| 
|goofy|int|df|Contestant acted goofy (Yes = 1, No =0)| 
|here_to_impress_someone|int|df|Contestant mentioned being here to impress someone (Yes = 1, No =0)|
|just_married|int|df|Contestant mentioned being a newlywed (Yes = 1, No =0)|
|risk_taker|int|df|Contestant's willingness to take risks (High = 1, Low =0)|
|familiar_with_show|int|df|Contestant was familiar with the show (Yes = 1, No =0)|
|here_for_the_money|int|df|Contestant mentioned being here for the money (Yes = 1, No =0)|
|slow|int|df|Contestant went through the challenges slowly (Yes = 1, No =0)|
|female|int|df|Contestant identifies as female (Yes = 1, No =0)|
|male|int|df|Contestant identifies as male (Yes = 1, No =0)|
|middle_aged|int|df|My guess at the contestant's age was 40-65 (Yes = 1, No =0)|
|older|int|df|My guess at the contestant's age was over 65 (Yes = 1, No =0)|
|young|int|df|My guess at the contestant's age was under 40 (Yes = 1, No =0)|
|arts|int|df|Contestant works in the arts (Yes = 1, No =0)|
|design|int|df|Contestant works in design (Yes = 1, No =0)|
|entertainment_&_tourism|int|df|Contestant works in entertainment or tourism (Yes = 1, No =0)|
|healthcare|int|df|Contestant works in healthcare (Yes = 1, No =0)|
|law_enforcement|int|df|Contestant works in law enforcement (Yes = 1, No =0)|
|military|int|df|Contestant works for the military (Yes = 1, No =0)|
|parent|int|df|Contestant is a full time parent (Yes = 1, No =0)|
|sales|int|df|Contestant works in sales (Yes = 1, No =0)|
|social_media|int|df|Contestant works in social media (Yes = 1, No =0)|
|student|int|df|Contestant is a dull time studennt (Yes = 1, No =0)|
|tech|int|df|Contestant works in tech (Yes = 1, No =0)|
|midwest|int|df|Contestant lives in the Midwest (Yes = 1, No =0)|
|northeast|int|df|Contestant lives in the Northeast (Yes = 1, No =0)|
|southeast|int|df|Contestant lives in the Southeast (Yes = 1, No =0)|
|southwest|int|df|Contestant lives in the Southwest (Yes = 1, No =0)|
|west|int|df|Contestant lives in the West (Yes = 1, No =0)|

I input the following variables to determine my own results: 
```
me = {'baking_experience' : 0, 
      'decorating_experience' : 1, 
      'goofy' : 1, 
      'here_to_impress_someone' : 1,
      'just_married' : 0, 
      'risk_taker' : 1,
      'familiar_with_show' : 1, 
      'here_for_the_money' : 0, 
      'slow' : 1, 
      'female' : 1, 
      'male' : 0,
      'middle_aged' : 0, 
      'older' : 0, 
      'young' : 1, 
      'arts' : 0, 
      'design' : 0,
      'entertainment_&_tourism' : 0, 
      'healthcare' : 0, 
      'law_enforcement' : 0, 
      'military' : 0,
      'parent' : 0, 
      'sales' : 0, 
      'social_media' : 0, 
      'student' : 0, 
      'tech' : 1, 
      'midwest' : 0,
      'northeast' : 0,
      'southeast' : 0, 
      'southwest' : 0, 
      'west': 1}
```
## Next Steps
- With more time, I would have loved to dig in to the ROC curve of my logistic regression model to look for ways to optimize for accuracy and sensitivty (as I would not want to get a false negative and be lulled into a sense of security by that.
- I would like to build a web app that can tell someone else whether or not they would embarrass themselves. 
- I would create models for whether or not a person is likely to win an episode. 
