---
layout: default
title: Similarity Part 
description: 
htmlwidgets: TRUE
---

Please write here 

### Introduction
Now let's look at each individual event. To determine if an event has had an impact on the movie industry, we'll again use the similarity score to classify a movie as _similar_ to an event. We'll quantify this be asking the question: Is the fraction of similar movies larger in the dataset after than before the event?

How can we examine this? Regression! We'll use the the **fraction of similar movies per year** (_F_ ) as response variable and use **year** (_Y_ ) and an indicator variable **is after** (_A_ ) as covaraiates. This yields the formula:

<img src="https://latex.codecogs.com/svg.image?F&space;=&space;\alpha&space;&plus;&space;\beta_{1}Y&space;&plus;&space;\beta_{2}A&space;&plus;&space;\epsilon&space;" title="https://latex.codecogs.com/svg.image?F = \alpha + \beta_{1}Y + \beta_{2}A + \epsilon " />

where alpha is a constant and epsilon is random noise. So why do we use the fraction of similar movies per year rather to the, perhaps more intuitive quanity, _similar movies per year_? We saw earlier that movie-making is much more popular today compared to earlier year. This means we have to work with fractions instead of absolute quantities to capture this effect. The results from these regression models are found in the table below.


| **Event**                                         | &alpha; | &beta;<sub>1</sub>              | &beta;<sub>2</sub>            | **Significant coefficients**                   |
|---------------------------------------------------|---------|---------------------------------|-------------------------------|------------------------------------------------|
| Pearl Harbour                                     | 0.1986  | -0.0001                         | 0.0078                        | &alpha;, &beta;<sub>1</sub>, &beta;<sub>2</sub> |
| Apollo 11                                         | -0.2270 | 0.0001                          | -0.0034                       | &alpha;, &beta;<sub>1</sub>, &beta;<sub>2</sub> |
| John Hinckley Jr Attempts To Assassinate Reagan   | -0.0524 | 2.886&middot;10<sup>-5</sup>    | 0.0027                        | &beta;<sub>2</sub>                             |
| Cold War                                          | -0.1623 | 8.567&middot;10<sup>-5</sup>    | -0.0005                       | &alpha;, &beta;<sub>1</sub>                   |
| Brown v. Board of Education of Topeka             | -0.0040 | 4.096&middot;10 <sup>-6</sup>   | -0.0015                       | &beta;<sub>2</sub>                             |
| The Berlin Wall Falls                             | 0.0146  | -5.343&middot;10<sup>-6</sup>   | 0.0026                        | &beta;<sub>2</sub>                             |
| The Hungarian Revolution Starts                   | 0.0626  | -2.991&middot;10<sup>-5</sup>   | 0.0030                        | &beta;<sub>2</sub>                             |
| The War In The Falkland Islands Begins            | -0.0870 | 4.75&middot;10<sup>-5</sup>     | -0.0011                       | &alpha;, &beta;<sub>1</sub>                   |
| The Iranian Revolution Happens                    | -0.1286 | 6.846&middot;10<sup>-5</sup>    | 0.0001                        | &alpha;, &beta;<sub>1</sub>                   |
| Apartheid Ends                                    | -0.0773 | 4.133&middot;10<sup>-5</sup>    | 0.0012                        | None                                           |
| Nelson Mandela Is Released From Prison            | -0.0264 | 1.554&middot;10<sup>-5</sup>    | 0.0006                        | None                                           |
| Stanislav Petrov Saves The World By Doing Nothing | -0.0799 | 4.333&middot;10<sup>-5</sup>    | -0.0005                       | None                                           |
| Apollo 13                                         | -0.1088 | 5.895&middot;10 <sup>-5</sup>   | -0.0015                       | None                                           |
| Winston Churchill Dies                            | 0.0034  | 2.146&middot;10 <sup>-7</sup>   | -0.0009                       | None                                           |
| Civil Rights Act Is Passed                        | -0.0252 | 1.479&middot;10<sup>-5</sup>    | -0.0007                       | None                                           |
| President Kennedy Is Assassinated                 | -0.0751 | 4.145&middot;10<sup>-5</sup>    | 0.0011                        | None                                           |
| Construction Begins On The Berlin Wall            | -0.0436 | 2.543&middot;10<sup>-5</sup>    | -0.0019                       | None                                           |
| The Vietnam War begins                            | -0.0630 | 3.571&middot;10<sup>-5</sup>    | -0.0014                       | None                                           |
| China Begins The Great Leap Forward               | -0.0392 | 2.21&middot;10<sup>-5</sup>     | 0.0002                        | None                                           |
| Sputnik Is Launched                               | -0.0439 | 2.462&middot;10<sup>-5</sup>    | -0.0009                       | None                                           |
| The Warsaw Pact Is Signed                         | -0.0492 | 2.764&middot;10<sup>-5</sup>    | 0.0012                        | None                                           |
| The Korean War                                    | -0.0432 | 2.457&middot;10<sup>-5</sup>    | 0.0018                        | None                                           |
| The Marshall Plan Is Implemented                  | -0.0460 | 2.582&middot;10<sup>-5</sup>    | -0.0013                       | None                                           |
| The Truman Doctrine Is Announced                  | -0.0505 | 2.875&middot;10<sup>-5</sup>    | -0.0016                       | None                                           |
| Atomic Bombing Of Hiroshima And Nagasaki          | -0.0388 | 2.244&middot;10<sup>-5</sup>    | 0.0009                        | None                                           |


We know, this is a lot of numbers to digest...

5.2&middot;10<sup>5</sup>

you can look at stylesample.md to see what you can do..

Your page will display at : 


http://localhost:4000/similarity