# a11y.co.mz
 
# Overview
In December 2020, the Mozambican Disabled Person’s Organisation Forum (FAMOD) teamed up with UK-based non-profit Data4Change to carry out a data-driven investigation into the level of web accessibility across 90 key websites in Mozambique, ranging from online shopping to news sites, job sites and government information and services. More information about the investigation and the barriers faced by people with disabilities online can be found on www.a11y.co.mz.

# Methodology
We used the axe-core library API to carry out automated accessibility testing on 18,704 web pages across 90 Mozambican websites, according to WCAG guidelines. 

For each of the websites, internal links (up to level-2 internal links) were assessed using axe-core. Here “up to level-2 internal links” means; including 102 initially specified links (level-0 links), links found on 102 pages initially specified (level-1 links) and links found on level-1 pages (level-2 links).

We supplemented this automated testing with a day of manual testing on a small selection of the websites. This further confirmed the significant barriers faced by screen reader and colour blind internet users.

# Results
The automated testing captured 722,053 instances of accessibility ‘violations’. Each violation represents a barrier preventing someone with a visual, hearing, physical or cognitive impairment from fully engaging with the web page.

- Total number of websites assessed: 90
- Total number of web pages assessed: 18,704
- Total number of violations found: 722,053

# Analysis
We deliberately made the decision not to score, rate or compare websites against one another since automated testing can only test some accessibility errors and we therefore cannot fairly compare websites. For example, if the only errors a website had were 100 images with no alt attributes a tool could find all of those and therefore 100% of the issues. However, if a website had an issue relating to focus order, a tool couldn’t find this issue and would get 0% of issues. 

However, our results can tell us the most common accessibility violations found by automated testing. 

The top five major accessibility violations were as follows (and account for nearly 90% of all the accessibility violations on the web pages that we tested):
- 37% of violations: Elements have insufficient colour contrast
- 33% of violations: Not all page content is contained by landmarks
- 11% of violations: Links do not have discernible text
- 3% of violations: Select elements do not have accessible names
- 2% of violations: Images do not have alternate text

Note: In aggregating this list, we excluded "minor" violations, such as “id attribute value must be unique”. We also included the violation “Document must have one main landmark” under “All page content must be contained by landmarks” and the violation “Form elements must have labels” under “Select element must have an accessible name".

# Data
The file **pages.csv** contains the number of accessibility rules passed, violated, inapplicable and incomplete-tests per page (18,704 observations) 

# Data dictionary
*list of each column name and its description to come*

# About
## About a11y.co.mz
“A11y” is a common abbreviation for “accessibility”. The “11” represents the number of letters between the “a” and “y” in the word “accessibility”. a11y.co.mz was designed and developed by Amílcar Carlos Paco (IT Manager and Data Engineer at FAMOD) and Data4Change. FAMOD is among 13 civil society organisations who were successful in applying for the African Digital Rights Fund run by CIPESA (Collaboration on International ICT Policy in East and Southern Africa). The African Digital Rights Fund included the opportunity to receive data skills training and work on data-driven projects with Data4Change.

## About FAMOD
FAMOD is an umbrella organisation for civil society organisations working to support people with disabilities in Mozambique. FAMOD was founded in 2003 and works to support, coordinate and represent the interests of their member organisations, as well as to promote the human rights and wellbeing of people with disabilities in Mozambique. FAMOD is currently working to ensure that people with disabilities, including women and children, are not left behind in Covid-19 response and recovery plans. Visit famod.org for more information.

## About Data4Change
Data4Change is a UK-based non-profit, they create data-driven projects aimed at solving some of the world’s most pressing social and political challenges. Visit data4chan.ge for more information.

## About CIPESA
This project was carried out in the context of the Africa Digital Rights Fund with support from the Collaboration on International ICT Policy for East and Southern Africa (CIPESA). Since inception, CIPESA has positioned itself as a leading centre for research and analysis of information aimed to enable policy makers in the region to understand ICT policy issues, and for various multi-stakeholders to use ICT to improve livelihoods. Visit cipesa.org for more information.
