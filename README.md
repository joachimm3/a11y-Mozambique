# a11y.co.mz
 
# Overview
In December 2020, the Mozambican Disabled Person’s Organisation Forum (FAMOD) teamed up with UK-based non-profit Data4Change to run automated accessibility testing on 90 of the most important and useful websites in Mozambique. 

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
The data folder contains the following two csv files:
- **pages.csv** Dataset showing the number of accessibility rules passed, violated, inapplicable and incomplete-tests per page (18,704 observations) 
- **violations.csv** Dataset detailing the count of each type of accessibility violation per page (128,377 observations)

# Data dictionary
## Page stats analysis
*list of each column name and its description to come*

## Violations analysis
*list of each column name and its description to come*
