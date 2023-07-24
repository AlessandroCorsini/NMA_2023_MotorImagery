# NMA_2023_MotorImagery

## Exploring the role of DLPFC in motor imagery

### Research Proposal(W1D5)
**Abstract**. Various studies have found the pattern of cortical activity to have similar spatial distribution and general pattern in Motor Imagery (MI)  and Motor execution (ME) tasks. Different studies have also found the activity of DLPFC, especially in the theta band, to have a major role in MI tasks.
The majority of these studies have used EEG and MEG data, with a few that have investigated Ecog recordings. 
Our dataset consists of continuous Ecog voltage time series (sampled at 1000 Hz.) recording from 46 electrodes across the left frontal and parietal lobes, during Motor Execution (ME) and Motor Imagery (MI) tasks, for Hand and Tongue movements. The data was recorded for 30 trials per condition, 376 seconds.

To test the hypothesis that whether or not the activity of DLPFC is different during motor imagery and motor execution tasks, we used a logistic regression classifier to the activity of electrodes of an Ecog grid placed on the left frontal and parietal cortices to distinguish MI and ME, in hand and tongue movements separately.
The Theta band power in DLPFC, as well as high (70-100Hz) and low (8-32Hz) frequency band power in the motor areas, were chosen as features.
The results of a  preliminary logistic regression classification show that the high-frequency band power ( HFBp) in the motor electrodes has the most discriminating power (classification accuracy= ?), followed by low-frequency band power( LFBp) in the same electrodes with a classification accuracy of ?? , both exceeding that of Theta band power in DLPFC that had an accuracy of ??  in distinguishing MI and Me for hand movements.

**Introduction**. Decoding brain signals associated with motor imagery (MI) is a unique tool for studying the relevance of rehabilitation of patients with various motor disorders, for example, it can open up new possibilities for the use of neuroprostheses that could significantly improve the quality of life of patients. Working on the same dataset, Miller et al. (2010) found similar spatial distribution of local neuronal population activity during MI and actual motor movement (ME). However, EEG studies have shown that certain areas of the brain that are not directly related to motor activity can play an important role in MI (Lee M et. al., 2020, Kim Y et. al. 2018). Thus, it was revealed that DLPFC is closely related to cortical movement control, may be associated with the supplementary motor area (SMA) (Middleton and Strick, 1994) and plays an important role in MI (Kim Y et. al., 2018). 

**Question**. Does Theta band power in DLPFC predict the activity in PMA and SMA during Motor Imagery tasks?

**Hypothesis**. We hypothesize that theta-band activity in the DLPFC can predict the activity in PMA and SMA during motor Imagery tasks more than it does during the motor execution tasks.

**Dataset**. Our dataset is structured as follows: continuous Ecog voltage time series (sampled at 1000 Hz.) recording from 46 electrodes across the left frontal and parietal lobes, during Motor Execution (ME) and Motor Imagery (MI) tasks, for Hand and Tongue movements. The data was recorded for 30 trials per condition, 376 seconds in total.

**Variables**. The independent variable will be the theta band (4-8 Hz) power in DLPFC. The dependent variables will be the high (70-100 Hz) and low (8-32 Hz) band frequency power in the primary and supplementary motor areas.

**Methods**.  First we will establish the existence of our hypothesized role for the DLPFC using conventional methods. Then we will use computational modeling schemes to verify the results of the first step, comparing the extent of their efficacy to detect the influence of DLPFC on PMA and SMA.

### Abstract (W2D5)
**Abstract**. Various studies have investigated the cortical activities in the motor areas during Motor Imagery (MI)  and Motor execution (ME) tasks and found  a difference in lower activity powers, but similar spatial distribution in the case of MI engagement. In addition, different studies associated the activity of the dorsolateral prefrontal cortex (DLPFC), especially in the theta band, with a major role in MI tasks. Most of these studies have used EEG and MEG data, with a few investigating ECoG recordings. 
  Our dataset consists of continuous ECoG voltage time series recording across the left frontal and parietal lobes, during ME and MI tasks, for Hand and Tongue movements. 
  Our aim was to test the hypothesis that the activity of different regions of DLPFC are different during MI and ME tasks, or in other words, whether MI and ME are distinguishable just by looking at the activity of DLPFC. We performed a single case study using a logistic regression classifier with 8 fold cross-validation and L2 penalty to distinguish MI and ME, in hand and tongue movements separately.
  The Theta band power in two different regions of DLPFC, roughly the Broadman Areas 9 and 46 (BA9 and BA46), as well as high (70-100Hz) and low (8-32Hz) frequency band power in the motor areas were chosen as features. To ensure appropriate proportions in the design matrix, the power data in each trial were averaged over 5 windows, reducing the total number of features.
  The results of a preliminary logistic regression classification performed on hand movement data show that the high-frequency band power (HFBp) in the motor electrodes has the most discriminating power (classification accuracy = 98%). Accuracy was also high for low-frequency band power (LFBp) in the same electrodes, with a classification accuracy of 94%, Both exceeding the Theta band power in DLPFC, that had an accuracy of about 50% distinguishing MI and ME. Of note is that the electrodes located in BA9 showed slightly higher (62%) accuracy than that of BA46 (56%).
  The same test performed for tongue movements showed similar results, with accuracies of 95%,81%,68% and 58% For HFBp and LFBp in motor areas and theta band power in BA46 and BA9, respectively, only this time, BA46 showed higher classification accuracy than BA9.
   Contrary to our initial hypothesis, these results suggest that the Theta band activity of DLPFC, at least if looked at synchronously, is not as reliable as HFBp and LFBp of the motor areas in discriminating MI and ME.


**The following contribuited equally to this project:**

  - Alessandro Corsini (https://alessandrocorsini.github.io/)
  - Melchior Steimen (steimenmelchior@gmail.com)
  - Mila Makarova (makarova-milka@mail.ru)
  - Saman Lashgari (smnlashkari@gmail.com)
  - Ricardo De Haro Mancha (ricardomeine96@gmail.com)

We thank our Teaching Assistant: Joao Araujo (https://github.com/joaoaraujo1)
