# 1. Predicting Surveillance Technologies Used by Government Agencies

# 2. Team Members

Robin Hurtado
Amy Tran 

# 3. Project Overview

This project analyzes public datasets to identify which surveillance technologies are likely to be used by different types of government agencies. 
We plan to use machine-learning methods to we build a  classification model that predicts the likelihood that an agency uses each technology category based on its type and location.

# 4. Research Questions

(narrow this down as we get closer)

Which surveillance technologies are most commonly used by different agency types?

Can we predict the set of technologies an agency is likely to use?

(maybe this one? Which features (agency type, jurisdiction, etc.) best explain technology usage patterns?)

# 5. Data Description

A collection of data with metrics on surveilance used by government organizations such as local governments and police departments. Includes data such as methods of surveilance, name of organization, number of hits, and links to sources of the data. 

U.S. law-enforcement agencies + what surveillance technologies they use (body-worn cameras, drones, ALPRs, etc) from the Electronic Fronteir Foundation From [https://www.atlasofsurveillance.org/data-library] date link: [https://www.atlasofsurveillance.org/download.csv]

Automated License Plate Reader Dataset from the Electronic Frontier Foundation at [https://www.eff.org/pages/download-alpr-dataset]

Definitions for reference when using the EFF-MuckRock 2016-2017 ALPR DATA.csv dataset Article at [https://www.eff.org/pages/]automated-license-plate-reader-dataset Data files description, and definitions found at [https://www.eff.org/tl/document/eff-muckrock-alpr-data-2016-2017-0]

Field Descriptions for reference when using the EFF-MuckRock 2016-2017 ALPR DATA.csv dataset

Atlas of Surveillance: Southwestern Border Communities "The Electronic Frontier Foundation has partnered up with the University of Nevada, Reno's Reynolds School of Journalism to begin an inventory of what surveillance technologies law enforcement agencies across the country have acquired. We started with communities along the U.S.-Mexico border: areas of contention and controversy, where discussions of “virtual walls” have resulted in increased funding and focus on surveillance. " Compiled by students of Reynold School. from [https://www.eff.org/pages/atlas-de-vigilancia-comunidades-fronterizas-del-suroeste]

This dataset accompanies the March 9, 2021 report "Scholars Under Surveillance: How Campus Police Use High Tech to Spy on Students." Hailey Rodis, a student at the Reynolds School of Journalism at the University of Nevada, Reno, was the primary data wrangler on this project. from [https://www.eff.org/ur/document/campus-police-surveillance-dataset] and report at [https://www.eff.org/deeplinks/2021/03/scholars-under-surveillance-how-campus-police-use-high-tech-spy-students]

# 6. Methods

(list all steps here before final submit - steps are noted and annotated in the notebook)

Import data from Electronic Frontier Foundation on use of Automated License Plate Readers - multiple states

* First thing - opened files in Excel and did some clean up.  
* Filtered each column and scrolled through the unique/ filterable values Excel found.  
* Filled all blank values with an empty string to avoid NaN errors.  
* Changed full state name to two-letter state abbreviation for consistency across all State columns.  
* Removed invalid characters, spaces from column headers, changing them to PascalCase instead.
* AOS Data had some blank entries for counties.  Looked them up using Google. 
* Entered the Census area as county for AK cities that do not have an actual county. 
* Entered DC Metro Area as county for Washington DC
* Entered CityName (no county) for independent US cities not existing in a county (ex: St Louis, MO, Baltimore, MD)
* Separated multiple counties listed in one cell to multiple cells county1, county2..
* Checking for typos/ misspelled counties/ invalid characters

# 7. Results

(TBD)

# 8. Limitations

(Scope, Data weakness, missing data? )

