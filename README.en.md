[Versão em Português - Clica aqui](https://github.com/Amilcar-Paco/a11ymoz)


# a11y.co.mz – Web accessibility in Mozambique
 
# Overview
In December 2020, the Mozambican Disabled Person’s Organisation Forum (FAMOD) teamed up with UK-based non-profit Data4Change to carry out a data-driven investigation into the web accessibility of 90 key websites in Mozambique. Websites were selected by FAMOD and ranged from online shopping to news sites, job sites and government information and services. More information about the investigation and the barriers faced by people with disabilities online can be found on project website, www.a11y.co.mz.

# Methodology
We used the axe-core library API (https://github.com/dequelabs/axe-core) to carry out automated accessibility testing on 18,704 web pages across 90 Mozambican websites, according to WCAG guidelines. 

For each of the websites, internal links (up to level-2 internal links) were assessed using axe-core. Here “up to level-2 internal links” means; including 102 initially specified links (level-0 links), links found on 102 pages initially specified (level-1 links) and links found on level-1 pages (level-2 links).

We supplemented this automated testing with a day of manual testing on a small selection of the websites. This further confirmed the significant barriers faced by screen reader and colour blind internet users.

# Results
The automated testing captured 722,053 instances of accessibility ‘violations’. Each violation represents a barrier preventing someone with a visual, hearing, physical or cognitive impairment from fully engaging with the web page.

- Total number of websites assessed: 90
- Total number of web pages assessed: 18,704
- Total number of violations found: 722,053

# Analysis
We deliberately made the decision not to score, rate or compare websites against one another since automated testing can only test some accessibility errors and we therefore cannot fairly compare websites. (For example, if the only errors a website had were 100 images with no alt attributes a tool could find all of those and therefore 100% of the issues. However, if a website had an issue relating to focus order, a tool couldn’t find this issue and would get 0% of issues.)

Our results can tell us the most common accessibility violations found by automated testing. The top five major accessibility violations were as follows (and account for nearly 90% of all the accessibility violations on the web pages that we tested):
- 37% of violations: Elements have insufficient colour contrast
- 33%: Not all page content is contained by landmarks
- 11%: Links do not have discernible text
- 3%: Select elements do not have accessible names
- 2%: Images do not have alternate text

Note: In aggregating this list, we excluded "minor" violations, such as “id attribute value must be unique”. We also combined the violation “Document must have one main landmark” with “All page content must be contained by landmarks” and the violation “Form elements must have labels” with “Select element must have an accessible name".

# Data
The file **pages.csv** contains the results for each of the 18,704 web pages tested, detailing the number of accessibility rules passed, violated, inapplicable and incomplete-tests per page.

# Data dictionary

|Variable          |Description                                                                                                                                                               |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|website_id        |ID number of each website domain                                                                                                                                          |
|website_name      |Website domain name                                                                                                                                                       |
|website_url       |Website domain URL                                                                                                                                                        |
|website_category1 |Website Category , whether private or public.                                                                                                                             |
|website_category2 |Functional category of website domain (eg news, shopping, academic.)                                                                                                      |
|webpage_id        |Page ID generated from MD5 hash of page URL.                                                                                                                              |
|webpage_url       |The URL of the tested page.                                                                                                                                               |
|page_depth        |Link depth of the page from initial website URL                                                                                                                           |
|test_timestamp    |Time when the test was completed. https://github.com/dequelabs/axe-core/blob/develop/doc/API.md#timestamp                                                                 |
|passes_count      |Number of accessibility test rules passed.                                                                                                                                |
|violations_count  |Number of accessibility test rules violated.                                                                                                                              |
|inapplicable_count|Number of accessibility test rules that were inapplicable for the page.                                                                                                   |
|incomplete_count  |Number of accessibility tests that were aborted. This can happen either because of technical limitation to what the rule can test, or because a JavaScript error occurred.|



# About
## About a11y.co.mz
“A11y” is a common abbreviation for “accessibility”. The “11” represents the number of letters between the “a” and “y” in the word “accessibility”. a11y.co.mz was designed and developed by Amílcar Carlos Paco (IT Manager and Data Engineer at FAMOD) and Data4Change. FAMOD is among 13 civil society organisations who were successful in applying for the African Digital Rights Fund run by CIPESA (Collaboration on International ICT Policy in East and Southern Africa). The African Digital Rights Fund included the opportunity to receive data skills training and work on data-driven projects with Data4Change.

## About FAMOD
FAMOD is an umbrella organisation for civil society organisations working to support people with disabilities in Mozambique. FAMOD was founded in 2003 and works to support, coordinate and represent the interests of their member organisations, as well as to promote the human rights and wellbeing of people with disabilities in Mozambique. FAMOD is currently working to ensure that people with disabilities, including women and children, are not left behind in Covid-19 response and recovery plans. Visit www.famod.org for more information.

## About Data4Change
Data4Change is a UK-based non-profit, they create data-driven projects aimed at solving some of the world’s most pressing social and political challenges. Visit www.data4chan.ge for more information.

## About CIPESA
This project was carried out in the context of the Africa Digital Rights Fund with support from the Collaboration on International ICT Policy for East and Southern Africa (CIPESA). Since inception, CIPESA has positioned itself as a leading centre for research and analysis of information aimed to enable policy makers in the region to understand ICT policy issues, and for various multi-stakeholders to use ICT to improve livelihoods. Visit www.cipesa.org for more information.
