# CS505


[Gender and Age](Twitter%20User%20Age%20and%20Gender.ipynb)

[Race](Twitter%20User%20Race.ipynb)

## Question

When I was using M3 inference, it outputs a json for each user like this:


 'output': {'age': {'19-29': 0.147,
                    '30-39': 0.8197,
                    '<=18': 0.0049,
                    '>=40': 0.0285},
            'gender': {'female': 0.0006, 'male': 0.9994},
            'org': {'is-org': 0.0, 'non-org': 1.0}}}

1. How can I determine the exact age when the age was given a range? 

To determine the exact age, you cannot use m3 inference. You must build your own classifier that is based on user tweets that I mentioned before in my previous email. 

2. Can we just say the above-given user is a male? 

yes, you can

3. the human label value(age, gender, etc..) in the given dataset has a lot of NULL values, how can we compare two values?

for NULL values, you cannot evaluate. So for evaluation, use only non-null values in that file for labeled age (to evaluate your age prediction), and labeled_gender (to evaluate your gender prediction)
