# MedWise #
Help you get the meds you need!

This project was done as a part of the Erdös Institute May 2021 BootCamp. <br>
All the data for this project was provided by [CoverMyMeds](https://www.covermymeds.com/main/).  

# Table of contents
* [Problem Description](#Problem-Description)
* [Data](#Data) 
* [Model](#Model)
* [Result](#Result)
* [Repository contents](#Repository-contents)
* [Acknowledgement](#Acknowledgement)

# Problem Description
CoverMyMeds, part of McKesson's Prescription Technology Solutions, is a fast growing healthcare technology company. The primary goal of CoverMyMeds is to help patients get the medications they need by seamlessly connecting the healthcare network to improve medication access. In this challenge, the participants are required to use simulated data provided by CoverMyMeds to answer the following questions :

1. Can a claim's approval be predicted from previous claim data? If so, what are the factors that influence claim approval?
2. If a claim is rejected, can the reason for rejection (rejection code) be predicted?
3. Can the approval of a Prior Authorization (PA) request be predicted? If so, what are the factors that influence PA approval?

<!-- # Data
There are four tables provided with the challenge : dim_claims.csv , dim_pa.csv , dim_date.csv and bridge.csv 

_dim_claims.csv_ contains information regarding the initial pharmacy claim, drug and payer. It also contains the information if the pharmacy claim was approved or rejected. If rejected, it provides the specific rejection code. 

There are four insurance companies - 417380, 417614, 417740, 999001, three drugs -  A, B and C and three rejection codes -  70, 75 and 76.

The reject_codes have the following meaning:
Code 70 : drug not in formulary
Code 75 : drug in formulary, needs PA
Code 76 : drug in formulary, number of fills exceeded.

A drug can be rejected by the payer for any of the three reasons, in which case a prior authorization (PA) can be applied for. There are more claims for drug A compared to drugs B and C. However, there is almost equally likely chance (55-64%) for the claim for a drug to be approved or rejected. While a drug may be rejected for any of the three reasons listed above, it turns out that in this particular data, each drug can be rejected by a company for only one reason.

The following information regarding the formulary of the four insurance companies was found after analyzing the data :

_BIN 417380_ : Drug C is not in the formulary, Drug A is in the formulary but needs PA, Drug B is covered but limit exceeded 

_BIN 417614_ : Drug A is not in the formulary, Drug B is in the formulary, needs PA, Drug C is covered but limit exceeded 

_BIN 417740_ : Drug B is not in the formulary, Drug C is in the formulary, needs PA, Drug A is covered but limit exceeded 

_BIN 999001_ : All drugs in formulary, limit exceeded for all.

The _dim_pa.csv_ table contains information regarding the PA request. For a given PA, it specifies whether the PA was approved or not. In addition, it also provides three columns justifying the need for the PA - ‘correct_diagnosis’, ‘tried_and_failed’ and ‘contraindication’. It turns out that PA requests that have checked ‘correct_diagnosis’ and ‘tried_and_failed’ have a higher chance of being approved, across claim reject_codes. ‘Contraindication’ seems to lower the chances of approval of a PA. Also, PAs for claims initially rejected with reject_codes 75 and 76 are highly likely to be approved, compared to reject_code 70 in general.

It turns out that two identical PAs for a certain drug rejected by an insurance company for a specific reason can either be rejected or approved. However, the chances of approval or rejection may depend on the boxes checked in the PA. 

I also noticed that date, whether workday, holiday or weekday, has limited impact on the PA approval status, suggesting the approval is not biased towards time. In addition to the given information, there might be other variables that influence the final decision on a PA.

For more information on the data, please refer to the [EDA notebook](EDA.ipynb)
 -->
<!-- # Model -->

<!-- # Result -->

<!-- # Repository contents -->

# Acknowledgement
All the work published in this repository are my own. However, I would like to thank [Siqi Sun](https://github.com/alohasiqi) and [Ruqiah Muhammad](https://github.com/Ruqiah314) with whom I had the wonderful opportunity to collaborate on this project during the course of the bootcamp. I am grateful to them for many wonderful discussions and brainstroming sessions!
