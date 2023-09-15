---
title: "Body performance"
output:
  html_document:
    df_print: paged
  html_notebook: default
  pdf_document: default
---

### Goal:

The primary objective of this project is to emphasize the significance of body performance in enhancing physical health and promoting exercise awareness among individuals. This will be accomplished by analyzing and extracting valuable insights from body performance datasets, monitoring the progression of human age, and subsequently improving the overall awareness of its importance.

### Data Source:

It from Kaggle website , The link( <https://www.kaggle.com/datasets/kukuroo3/body-performance-data>) show the source data.

### General Information about Body performance dataset :

Our dataset is called "Body performance" , The dataset provide the grade of performance and some data such as gender and age along with body measurements and other performance tests , It has 13394 row and each of them have 11 attributes.

*Table 1 : Data dictionary showing description of all Attributes*

| name                    | description                                                                                           | data type | possible value |
|------------------|------------------|------------------|-------------------|
| Age                     | The person's age in years                                                                             | numerical | 21-64          |
| Gender                  | The person's gender                                                                                   | binary    | F,M            |
| Height_cm               | The person's Height in cm                                                                             | numerical | 125-194        |
| weight_kg               | The person's weight in Kg                                                                             | numerical | 26.3-138       |
| body fat\_%             | the amount of essential fat .                                                                         | numerical | 3%-78.4%       |
| diastolic               | measures pressure the blood vessels when the heart is at rest                                         | numerical | 0-156          |
| systolic                | measures pressure in the arteries when the heart beats in minutes                                     | numerical | 0-201          |
| gripForce               | fingers flexibility tests                                                                             | numerical | 0-70.5         |
| sit and bend forward_cm | measures flexibility in sitting and bending forward in centimeters.                                   | numerical | -25-213        |
| sit-ups counts_cm       | measures the strength and endurance of the abdominals and hip-flexor muscles in centimeter.           | numerical | 0-80           |
| broad jump_cm           | It is a method of measuring how far a person can jump from a standing position to a landing position. | numerical | 0-303          |
