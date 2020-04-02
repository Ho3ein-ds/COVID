# COVID-19: Data Analytics Perspective 
## Introduction
In December 2019, a local outbreak of pneumonia of initially unknown cause was detected in three patients with pneumonia connected to the cluster of acute respiratory illness cases from Wuhan (Hubei, China), and quickly determined to be caused by a novel coronavirus (COVID-19). The outbreak has since spread to every province of mainland China as well as at least 120 countries and regions.

Corona viruses are a family of viruses that are transmitted between people and animals. The disease causes respiratory illness (like the flu) with symptomes such as fever, cough, and in more severe cases, the infection can result in difficulty breathing. You can protect yourself by washing your hands frequently, avoiding toching your face, and avoiding close contact (1 meter or 3 feet) with people who are unwell. 

## Intersting stats & facts
* The COVID-19 pandemic won't end once warmer weather arrrives. The spread may slow slightly simply because there tends to be less coughing and sneezing during the warm months, but it's so easily transmissible that it will continue to circulate if we don't get a handle on it now. That's why social distancing is so important.

* **"It's possible that 70% to 80% of people may have mild to no symptoms, but still be very cautious because you may still be infectious,"** says Peter Gulick, infectious disease expert at Michigan State University. 

* People of any age can get COVID-19, including children. In fact, The New York Times recently reported (https://www.nytimes.com/2020/03/18/health/coronavirus-young-people.html) that nearly 40% of hospitalized coronavirus patients in the U.S. are under the age of 54.

* From 14011 cases reported to the **European Surveillance System**, mainly (97%) from Germany, the most commonly reported clinical symptom was fever (47%), dry or productive cough (25%), sore throat (16%), general weakness (6%) and pain (5%). Data on cases reported may be biased toward the more seriously ill because national policies have shifted focus towards testing of more severe cases.

* Robust estimates for COVID-19 are still lacking and potentially biased by incomplete outcome data and differences in testing policies. The mean crude case-fatality (proportion of deaths among total cases reported) from the EU/EEA and the UK by 23 March 2020 was 5.4% (median country-specific estimate: 0.5%; range: 0.0-9.3%).

* Based on a large dataset from cases in China, the overall case fatality risk (CFR) among laboratory-confirmed cases was higher in the early stages of the outbreak (17.3% for cases with symptom onset from 1-10 January) and has reduced over time to 0.7% for patients with symptom onset after 1 February.

* In data on diagnosed COVID-19 cases in China and South Korea, overall CFR was 2.3%and 0.5%, respectively, and increased with age in all settings, with the highest CRF among people over 80 years of age (14.8% and 3.7%, respectively). Similarly, age-specific estimates of crude case-fatality for Germany, Italy and Spain increased rapidly with age, particularly above 60 years of age.

* The absolute numbers of deaths also increased with age in each country: those aged 70–79 years accounted for 19% (Germany), 36% (Italy) and 20% (Spain) of all deaths per country; these proportions rose to 74% (Germany), 50% (Italy) and 67% (Spain) among those aged 80 years and above.

* Data from a country report for Italy as of 19 March 2020 showed an increased risk of death among males compared with females in all age groups from 50 years and above. The risk of death becomes more pronounced with age, with an overall male-to-female ratio among COVID-19 deaths of 2.4:1.

* Among deceased patients in Italy until 19 March 2020, 73.8% had hypertension, 33.9% diabetes, 30.1% ischaemic heart disease, 22.0% atrial fibrillation, 19.5% a cancer diagnosed in the last five years. About half (48.6%) of the COVID-19 deaths had three or more comorbidities, 26.6% had two comorbidities, 23.5% had one comorbidity, and 1.2% had none. The most common complications observed in Italy were respiratory insufficiency (96.5%), acute kidney failure (29.2%), acute myocardial damage (10.4%) and bacterial superinfection (8.5%).

* Children made up a very small proportion of the 50 068 cases reported to TESSy as of 24 March (with known age (<10 years (1%), 10–19 years (4%)). The male-to-female ratio (1.2:1 overall) was less pronounced in children (1.1 and 1.0 in those aged 10–19 and <10 years, respectively) and increased with age. 

* Recent publications have evaluated the survival of SARS-CoV-2 on different surfaces. The environmental stability of viable SARS-CoV-2 is up to 3 hours in the air post aerosolisation, up to 4 hours on copper, up to 24 hours on cardboard, and up to 2–3 days on plastic and stainless steel, albeit with significantly decreased titres. 

For more infographics and leaflets about COVID-19, refer to the following link: https://www.ecdc.europa.eu/en/covid-19/facts/infographics

## Data
There are plenty of different data sources, mostly relying on the **Johns Hopkins University (JHU)** COVID-19 case data (https://github.com/CSSEGISandData/COVID-19). However, the JHU datasets have some quirky issues to it that makes it a bit cubersome to prepare and analyze it. Some of these issues are as follows: (i) weird column names including special characters, (ii) countries and states in the mix, (iii) wide format which makes it quite unhandy for data analysis, (iv) import problems due to line break issues, etc.

Other data sources that would be useful for analytical purposes are as follows:

* **World Health organization (WHO)**: https://www.who.int/
* **National Health Commission of the People's Republic of China (NHC)**: http://www.nhc.gov.cn/xcs/yqtb/list_gzbd.shtml
* **Hong Kong Department of Health**: https://www.chp.gov.hk/en/features/102465.html
* **USA Centers for Disease Control (CDC) and Prevention**: https://www.cdc.gov/coronavirus/2019-ncov/index.html
* **Government of Canada**: https://www.canada.ca/en/public-health/services/diseases/coronavirus.html
* **Australia Government Department of Health**: https://www.health.gov.au/news/coronavirus-update-at-a-glance
* **European Centre for Disease Prevention and Control (ECDC)**: https://www.ecdc.europa.eu/en/geographical-distribution-2019-ncov-cases
* **Ministray of Health Singapore (MOH)**: https://www.moh.gov.sg/covid-19
* **Italy Ministry of Health**: http://www.salute.gov.it/nuovocoronavirus
* **WorldoMeters**: https://www.worldometers.info/coronavirus/

For all of statisticians / data scientists, who have been working with COVID-19 time series data, **STATWORKX** created an application program interface (API) for this purpose. The API uses official data from the European Centre for Disease Prevention and Control. This API delivers a concise and clear data structure for further in-depth statistical analysis. The API is built using Python 3 and deployed using **Google Cloud Run** (https://cloud.google.com/run?hl=en), a container-based serverless function framework in the cloud. For more information about this amazing API, please check the code in the **GitHub repository** (https://github.com/STATWORX/covid-19-api) and also the website (https://www.statworx.com/de/).

