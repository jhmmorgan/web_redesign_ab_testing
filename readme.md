---
output: 
  html_document: 
    keep_md: yes
---

# Which version of the website should you use?

**James Morgan (jhmmorgan)**

*2022-07-27*

## 📖 Background

You work for an early-stage startup in Germany. Your team has been working on a redesign of the landing page. The team believes a new design will increase the number of people who click through and join your site.

### The Task

They have been testing the changes for a few weeks and now they want to measure the impact of the change and need you to determine if the increase can be due to random chance or if it is statistically significant.

## 📋 Testing the changes

The team have created a new landing page (called a treatment) and new images. When customers land on the website, they will randomly be assigned \* Either the new or old landing page \* Either the new or old set of images

We therefore have 4 groups of customers

-   User group **A**: saw the **new** version of the landing page, with **new** set of images.

-   User group **B**: saw the **new** version of the landing page, with **old** set of images.

-   User group **C**: saw the **old** version of the landing page, with **new** set of images.

-   **Control** user group: saw the **old** version of both landing page and set of images.

------------------------------------------------------------------------

## 📊 Outcome

Following several weeks of testing, we can easily identify, with confidence that to get the highest conversion, we should use: \* The new treatment (the new version of the landing page); and \* The old set of images

These were the customers in **Group B**. There is an approx 1.3% uplift in conversion in this group, over the control group.

![](images/ab%20testing.png)

This has been confirmed through multiple methods of testing.

**Group A** The chance of Group A customers having a better conversion than the control group is 93.6% (through Baysian testing), however we can't rule out that the increased conversion was due to random chance (Frequentist testing).

**Group B** The chance of Group B customers having a better conversion than the control group is 99.7% (through Baysian testing), and it's significantly unlikey that the increased conversion is due to random chance (Frequentist testing).

**Group C** The chance of Group C customers having a better conversion than the control group is 89.6% (through Baysian testing), however like Group A, we can't rule out that the increased conversion was due to random chance (Frequentist testing). Expected loss of 0.000222 is below our loss threshold.

**Please read the Jupyter notebook to understanding how we've come to this conclusion.**
