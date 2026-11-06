---
layout: post
title: "Day 1: Python basics with six complaints"
---
This project was about understanding what dictionary is, use python commands to get the data quickly analyzed and get an output that gives valuable insights.

One example below:
**Exercise 3.** Print the `id` and `issue` of every complaint that took more than 7 days.

```python
for c in complaints:
    if c["days_to_respond"] > 7:
        print(c["id"], c["issue"])
```

Output:
2 Payment trouble
4 Account closed
5 Incorrect info

   1. Explain a dictionary to a 12-year-old. Where did you get stuck? That's your gap.

Think of dictionary as a row holding information about a student with some labels like "Roll no., First name, Last Name, Grade, Div" and next to each label is the corresponding value (eg: {"Roll no.": 1,"First name":"Vijitkumar", "Last Name":"Kunhikandi","Grade":"10","Div":"B"})

I got stuck when executing a loop. I had to figure out how exactly the loop syntax works. When to use a variable before the for loop and when not to use it.

Solution: Create a variable before the loop when you need to carry something across all the rounds, like a running count (late = 0) or a total (total = 0). The loop adds to it each time, and you read the answer after the loop ends.
No variable is needed before the loop when each round is complete on its own, like printing each complaint.

2. Which complaint would worry you most as a support manager, and why?

The Credit Report issue reporting incorrect info took 21 days to respond. The customer may have some urgent need for that credit report. He may have to share it
with another organization for some purpose. It being incorrect is a major issue and taking 21 days to respond makes it worse.

3. One thing you want to find out when you see the real data.

Which products have the highest percentage of late replies. This will help to target those in a focused manner and bring the response time down to a lower number.

View: https://github.com/Vijit-k/complaint-intelligence/blob/main/notebooks/day01_python_basics.ipynb
Run in Colab: https://colab.research.google.com/github/Vijit-k/complaint-intelligence/blob/main/notebooks/day01_python_basics.ipynb
