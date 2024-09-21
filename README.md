# A Machine Learning Analysis of Gaps in Africa's Global Health Crisis Response

### Introduction

The global health sector has already recorded a total of seven pandemics and epidemics, yet the world is only in the first quarter of the 21st century. The HIV/AIDS epidemic has been ongoing since its first outbreak in the 1980s, while COVID-19 and Monkeypox are the most recent global pandemics. Of the seven, H1N1 influenza had a considerably higher intervention success rate. However, even with its relatively high response success rate compared to the others, its effectiveness in Africa was notably lower, similar to every other global health intervention. So, how can Africa break free from over-reliance on the international health sector, and adequately prepare independently for future global health crises?

This project aims to build a predictive model of the H1N1 influenza vaccination uptake with the objective of identifying gaps in the patterns of both H1N1 and Seasonal vaccination predictions.

### Problem Statement

**Background:** 
Efforts by the global health sector to ensure global immunity against COVID-19 through vaccination achieved a worldwide average of 65.1% complete vaccination uptake. In contrast, Africa registered a discouragingly low vaccination coverage of 32.1%. Therefore, there is an urgent need for Africa to take the initiative to study past pandemic vaccination patterns, identify gaps that limit vaccination access, and plan for future global health interventions within the continent.

### Objectives:

**1. Build a regression model to predict H1N1 and seasonal flu vaccination uptake.**

*Evaluate the model’s performance to identify areas for improvement and ensure it meets a desired reliability standard.*

**Findings:** A **logistic regression** model was used to predict H1N1 vaccination uptake. The model attained an accuracy score of 0.8680 and a relatively high AUC score of 0.8924 on the train-test set. Additionally, the training set score and the test set score had a difference of 0.002, which indicates the model’s ability to generalize well to unseen data. 

To accommodate the bimodal distribution of the seasonal flu uptake, a **decision tree** classifier was used to predict seasonal flu vaccination uptake. The model achieved an accuracy score of 0.7756, with precision, recall, and F1 scores averaging to 0.80 for the vaccinated population and 0.75 for the not vaccinated population.

Overall, both the logistic regression model and the decision tree classifier achieved a relatively high accuracy score of 86.80% and 77.56%, respectively. Therefore, both models are expected to perform well on unseen data.


**2. Analyze the probability distributions of the train-test set predictions.**

*Investigate past H1N1 and Seasonal flu vaccination patterns to identify trends, gaps in vaccination coverage and potential predictors for future models.*

**Findings:** There are distinct patterns of vaccination uptake probabilities, suggesting significant differences in population behavior towards the H1N1 and seasonal flu vaccines.

For instance, the probability distribution of receiving the H1N1 vaccine is positively skewed, with the majority of the population having only a 0.1 chance of receiving the vaccine. This pattern could be attributed to factors such as vaccine hesitancy, lack of awareness, concerns about safety, and limited access to vaccines.

In contrast, the seasonal flu vaccine uptake shows a bimodal distribution, indicating the presence of two distinct groups in the population with differing likelihoods of receiving the vaccine. This pattern likely reflects a class imbalance in vaccine uptake, driven by varying characteristics such as age, access to information, health beliefs and the H1N1 vaccination status of these groups.

**3. Predict the future probabilities of receiving H1N1 and seasonal flu Vaccines.**

*Use these predicted probabilities to assess future vaccination patterns and uncover the potential gaps in vaccination coverage.*

**Findings:** Both probability distributions are predicted to show gaps between the distribution bars, indicating the presence of distinct clusters or gaps in the data, with certain predictor values having fewer or no occurrences. 

The distribution for the H1N1 vaccine is predicted to be more positively skewed, while the seasonal flu vaccine distribution is expected to be multimodal.

**Recommendations**

To enhance Africa’s preparedness for future health crises, the AU’s Africa CDC should take immediate action on the following solutions:

* *Strengthen vaccine education and awareness.*

Develop targeted communication strategies to address vaccine hesitancy and misinformation. This includes using local languages and culturally relevant messaging to improve awareness of the benefits and safety of vaccines.

* *Enhance access to vaccines.*

Collaborate with local governments and stakeholders to ensure equitable distribution of vaccines, particularly in rural and underserved areas. This could involve mobile vaccination units and community health worker training to increase outreach.

* *Invest in data infrastructure.*

Build robust data collection and management systems to continuously monitor vaccination uptake and public health outcomes. This will help in adapting strategies in real-time and improving the predictive models for future health crises.

* *Promote research and local innovation.*

Encourage research into local health beliefs and behaviors affecting vaccine uptake. Support local institutions in developing tailored solutions that reflect the unique contexts of various African communities.

* *Focus on bimodal distribution characteristics.*

Specifically address the distinct groups identified in the bimodal distribution of seasonal flu vaccine uptake. Develop tailored interventions for these groups based on their unique characteristics and barriers to vaccination.

* *Create a comprehensive health policy framework.*

Advocate for a policy framework that prioritizes preventive health measures, including vaccination, within national health agendas. This framework should align with broader health system strengthening efforts across the continent.
