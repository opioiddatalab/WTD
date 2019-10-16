
## Waiting Time Distributions for Opioids
The intent of this analysis is to explore whether parametric (reverse) Waiting Time Distribution (WTD) methods can improve opioid pharmacoepidemiology methods by more accurately and explicitly representing actual patient-level opioid exposure, in the United States.

By Nabarun Dasgupta (nab@unc.edu)

### 1 | Background
The foundational papers (with PDFs) are in [this bibliography](https://www.evernote.com/l/AhF42dfsTmtJLY3O55AY9EdE3eilGszKjfg).<br>
<br>
The originators are Henrik Støvring, Anton Pottegård, and Jesper Hallas at Aarhus University in Denmark. The WTD methods arose out of neccesity; major Danish health datasets do not have indication, dosage, or refill information, making it impossible to observe when someone has stopped taking a drug (e.g., defining the end of the exposed period, or right censoring). These models take advatange of <b>time between prescription refills</b> to estimate how long people actually consume the medicine. Turns out that these distributions can be modeled with considerable (statistical) efficiency using parametric equations, meaning that people are fairly consistent <em>when</em> they go get refills (including people at the extremes, which too is predictable). So, we can build a distribution from the observed refill data (vertical bars in the histograms for warfarin below), and draw a line to follow the tops of the bars. The line is powerful because it allows us to model the use of opioids with a level of control we have never had before.<br>
<br>
<img src="model fits Fig 1.png">

<em>But before we go any further, let us remind ourselves that all models are wrong (AMAW) because they are models, and not reality.</em>
<br>
<br>
Where WTD methods potentially gets really interesting for opioids:
1. This method may mean that we no longer have to assume that patients took the opioids as prescribed. 
2. We may be able to provide a handy way to see how our models change if we assume that some percent (say, 20%) of patients don't finish their opioids from a surgery, and use them again months (years?) later for a sprained ankle.
3. We know that the "days' supply" variable can be unreliable (more on that to come from another study in our group). Using PMP data, we may be able externally "validate" WTD methods and/or have cleaner days supply variables under explicit assumptions.
4. As US states pass legislation on opioid dispensing, including limits on days' supply (e.g., to 3 days post-surgery), we may have calendar time-varying effects in raw PMP and claims and EHR data that make it difficult to compare or pool with earlier data. So, having a parametric model for length of time exposed could extend the life of existing datasets.<br>
<br>

### Glossary

<ol>
    <li>Waiting time distribution (WTD)</li>
    <li>Reverse WTD</li>
    <li>Inter-arrival distance (IAD)</li>
    <li>Backward recurrence density (BRD)</li>
    
## 2 | Hypotheses
1. This method may mean that we no longer have to assume that patients took the opioids as prescribed. 
2. We may be able to provide a handy way to see how our models change if we assume that some percent (say, 20%) of patients don't finish their opioids from a surgery, and use them again months (years?) later for a sprained ankle.
3. We know that the "days' supply" variable can be unreliable (more on that to come from another study in our group). Using PMP data, we may be able externally "validate" WTD methods and/or have cleaner days supply variables under explicit assumptions.
4. As US states pass legislation on opioid dispensing, including limits on days' supply (e.g., to 3 days post-surgery), we may have calendar time-varying effects in raw PMP and claims and EHR data that make it difficult to compare or pool with earlier data. So, having a parametric model for length of time exposed could extend the life of existing datasets.<br>
