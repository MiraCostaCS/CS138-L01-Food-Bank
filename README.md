Food Bank Distribution Calculator
=================================

_Learning objective: demonstrate proficiency in creating and executing functions._

Introduction:
-------------

Each year a significant number of college students experience food insecurity at some point, meaning that they have limited or uncertain access to adequate food. In 2018-2019, about 39% of students who applied for financial aid reported experiencing food insecurity. This number has continued to grow and in more recent years it was reported that 66% of college students reported food insecurity. [(source)](https://www.csac.ca.gov/sites/default/files/file-attachments/food_and_housing_basic_needs_survey_2023.pdf ) This is a serious issue and can make it difficult for students to succeed in their courses. 

Luckily, there are resources for people struggling with food security. Two government funded resources for individuals to turn to include CalFresh and CalWorks. CalFresh is a program that assists low income households by providing EBT cards that can be used to help pay for groceries. CalWorks is another program, similar to CalFresh but is specifically dedicated to helping low income families with children access safe and nutritious foods. Both options are great resources to turn to for support. In addition, if students find themselves needing meals or groceries while on the San Elijo Campus, Community Learning Center, or the Oceanside campus they can find a food pantry on each campus that provides small snacks and quick meals for students. 

Below are links to resources for students facing food insecurity: 

*   Resource page on the MiraCosta website: [https://www.miracosta.edu/student-services/care/resources-for-students.html](https://www.miracosta.edu/student-services/care/resources-for-students.html) 
*   CalFresh: [Application](https://www.getcalfresh.org/?source=g2&utm_term=calfresh%20application&utm_campaign=Statewide+EN&utm_source=adwords&utm_medium=ppc&hsa_acc=3022312842&hsa_cam=13530638856&hsa_grp=120972711982&hsa_ad=538519139184&hsa_src=g&hsa_tgt=kwd-301897372977&hsa_kw=calfresh%20application&hsa_mt=b&hsa_net=adwords&hsa_ver=3&gad_source=1&gclid=Cj0KCQiAo5u6BhDJARIsAAVoDWtBxGpRyNPSTbkXa8zSIU6X-XHZcJt3EyNMSOYLYuPrlSTcGNN_VhgaAnonEALw_wcB), [Information](https://feedingsandiego.org/calfresh/?gad_source=1&gclid=Cj0KCQiAo5u6BhDJARIsAAVoDWu2KgEB9mfsJYJKru2rGBss6QEi16hdg2gxY1KvSdbnbXm5n029-KoaAhrgEALw_wcB)
*   CalWorks Application: [Application](https://benefitscal.com/), [Information](https://www.cdss.ca.gov/calworks)

In today's lab we will be creating a food bank simulation which calculates how many resources each household will be given based on the number of members within the household as well taking into consideration whether or not the family has infants to provide for. 

Step 1: `calc_family_items`
---------------------------

Write a function called `calc_family_items` that takes a parameter for the number of family members and returns how many loaves of bread and how many canned goods the family should receive. This function should not print to the console.

*   The amount of bread will be half the number of family members, rounded up to the nearest whole number. For example, a family of 3 would receive 2 loaves of bread. A family of 2 would receive 1 loaf of bread. I suggest using the `ceil(x)` function in the [math module](https://docs.python.org/3/library/math.html) to accomplish the rounding up part.
*   The amount of canned items will be 2 per family member.

Step 2: `calc_baby_items`
-------------------------

Write a function called `calc_baby_items` that takes a parameter for the number of infants in the family and returns how many packs of diapers and cans of formula the family should receive. This function should not print to the console.

*   The amount of diapers will be 3 packs per infant
*   The amount of formula will be 2 cans per infant

Step 3: `main`
------------

Write your `main` function which implements the following algorithm.

1.  Get console input for number of family members
2.  Get console input for number of infants
3.  Calculate bread and canned goods by calling method
4.  Calculate diapers and formula by calling method
5.  Output to console the results, formatted as shown below

```
Enter the number of family members (excluding infants): 3
Enter the number of infants: 2
Family will receive:
        2 loaves of bread
        6 canned goods
Infant items family will receive:
        6 diaper packs
        4 formula cans
```

Submit
------