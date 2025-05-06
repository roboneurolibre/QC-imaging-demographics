# Introduction

 The purpose of this Jupyter Notebook is to explore demographic data gathered from human MRI and/or PET brain imaging studies conducted in Quebec, Canada from 1992 to 2023. We would like to visualize trends and relationships between various demographic factors, as well as assess whether there are issues in participant selection and in the reporting of demographic data.

 **Why do we focus on demographics?**
 Our understanding of human health comes from scientific studies, each typically focusing on a specific aspect of disease and treatment. These studies shape medical research priorities and clinical decision-making. However, if a study's participant sample is not representative of the broader population, its findings may only benefit certain groups. For example, if a landmark Alzheimer's study primarily includes male participants but makes general conclusions about disease progression, it risks creating a misleading narrative, one that might differ if the study included more female participants or a balanced sampe.

 **What is the potential problem with reporting?**
 Standards for reporting demographic data vary across publications and institutions, and many reputable journals may not prioritize details like sex, race and ethnicity, or age. When this information is omitted, readers may struggle to determine which populations the study’s conclusions accurately appy to.

 **The content of this Jupyter book**
 In this notebook, you will find figures illustrating the demographics of Quebec MRI and PET brain imaging study participants, some of which contain interactive elements, and brief descriptions of what has been done to create those figures and why. Discussion and interpretation of results can be found in the full preprint.

 # Study selection
We used Medline, Embase, and Google Scholar databases, retrieved all records involving MRI and/or PET brain imaging in Quebec between 1992 and 2023, and screened those results. The Sankey diagram shows the screening process in detail. You can hover over the connections between blocks for information regarding screening criteria.

## Figure 1

:::{figure} #fig1cell
:label: fig1

CAPTION HERE
:::

We identified 1549 studies that were conducted in Quebec using MRI, PET, or both imaging modalities to study the healthy or diseased brain. These studies took place in different parts of Quebec, and focused on a wide variety of conditions. A breakdown of how studies were categorized is shown in the following treemap. 

You can click on each box in the figure to expand the category, and each individual study can be expanded to see the title and a DOI link to the article. You may click at the top of the current box to zoom back out.
 
The first level of distinction is the imaging technique. The second level is the region(s) of Quebec in which the studies take place. The final level is a categorization of study populations among the following: healthy population (studies of healthy brain connectivity and cognition, testing of imaging techniques in healthy populations, etc.), epilepsy, Parkinson's disease, Alzheimer's disease, mental and behavioral disorders (excluding dementia), multiple sclerosis, cerebrovascular disease, cancer and tumors, newborns and infants, concussion and injury, vision disorders, and pain. Categories also exist for populations concerning multiple of the above categories, labelled “Multiple Categories”, and for studies concerning any other patient population which has not been categorized here, labelled “Other”.

## Figure 2

:::{figure} #fig2cell
:label: fig2

CAPTION HERE
:::

# Regional breakdown of studies

The studies within Quebec were conducted in different administrative regions of the province. The following map shows the regional distribution of studies that were conducted with MRI and/or PET. You may zoom and drag the map. The drop down menu can be used to change the imaging modality, and each bubble can be hovered over to see the corresponding region’s name and number of studies.
 
## Figure 3

:::{figure} #fig3cell
:label: fig3

CAPTION HERE
:::

# Basic demographic breakdown

We aimed to visualize how imaging studies are distributed across age groups to understand which populations are most represented and why certain age groups are commonly studied. To achieve this, we categorized studies based on the average age of the participants and plotted the results in a histogram. 

On the right, in gray, are studies that failed to report participant ages or only provided limited information, such as an age range. Using the drop down menu, you can choose whether the histogram displays the number of studies within each age bin or the total number of participants in those studies.
 
Both counting methods are similarly limited. Binning by average age removes details about the age distribution within each study, which may lead to a misleading representation. However, since most studies do not provide comprehensive demographic breakdowns, this visualization offers the best possible insight given the available data.

## Figure 4

:::{figure} #fig4cell
:label: fig4

CAPTION HERE
:::

We also wanted to see if studies were properly reporting participant sex, and if they were appropriately including male and female participants. The split of male and female participants as well as participants whose sex is unreported is shown in this pie chart.

## Figure 5

:::{figure} #fig5cell
:label: fig5

CAPTION HERE
:::

# Relation between age and sex

Our initial approach to analyzing age and sex demographics in imaging studies was to use a population pyramid, where age distributions for each sex are displayed as stacked horizontal histograms. However, this method presents challenges due to inconsistencies in how studies report age.

Some studies provide detailed age information, either by reporting individual ages (which is rare) or by reporting distribution metrics such as standard deviation alongside the mean. However, most studies lack this level of detail. By grouping studies solely based only on average age, we lose crucial information about the actual age distribution within each study. Additionally, this approach assumes that the age distributions of male and female participants within a study are similar, which may not be the case, potentially further skewing the data.

## Figure 6

:::{figure} #fig6cell
:label: fig6

CAPTION HERE
:::

To get a better idea on how the sex and age of participants might be related, a relational scatter plot was created. This plot compares the percentage of female and male participants vs. the average age of participants for each study. Each marker represents an individual study. Markers are colored based on the number of participants. Because a large number of low sample size studies have poor sex distribution, it is worth taking a look at the graph when looking at only studies with a larger sample size. Here, the cutoff for the sample size can be chosen with a slider. Each marker can be hovered over to see the sex ratio, mean age, and number of participants. 

Ultimately, both visualizations suffer from the loss of age distribution information within each study, highlighting the limitations of current age reporting practices. This reinforces the need for more comprehensive demographic reporting to enable more accurate and meaningful analyses.

## Figure 7

:::{figure} #fig7cell
:label: fig7

CAPTION HERE
:::

# Ethnicity

Here we break down the ethnicity of participants reported in these imaging studies. Box sizes for each category are proportional to their participant counts. Boxes in the treemap may be clicked on to be expanded. Each category's box shows the percentage of all participants in that category and the number of participants. For subcategories within the “reported ethnicity” category, the percentage of the total reported participants is also given.

## Figure 8

:::{figure} #fig8cell
:label: fig8

CAPTION HERE
:::

# Trends in participant sex by year of publication

Based on the age distribution, it appears that many healthy participant studies likely recruit from student university volunteer populations. We wanted to explore whether this, or other factors, might influence the sex distribution of participants over time, given the significant improvements in gender representation within scientific fields in recent decades. Additionally it is valuable to visualize the total number of participants included in imaging studies over time. The stacked bar chart shows the number of male and female participants by year of publication, with the full height of each bar representing the total participants studied in that year. The red line overlaid on the graph indicates the percentage of female participants in studies each year.

## Figure 9

:::{figure} #fig9cell
:label: fig9

CAPTION HERE
:::

# Age distribution by region

Since we know that the majority of MRI and PET studies take place in Montreal, it is worth investigating whether location influences the age distribution of participants. Given that fewer studies are conducted in other regions, namely Sherbrooke and Quebec City, these sites may be more selective in their participant recruitment or focused on studying more specific populations rather than enrolling any available healthy volunteers. 

The following raincloud plot visualizes this distribution. The box plots display the median (centerline), first and third quartiles (box edges), and the minimum and maximum data points at the edge of the whiskers (known as fences), excluding any outliers. In the scatter plots below each boxplot, each black dot represents a study. The overlaid half-violin plots illustrate the density of studies across the average age range for each region. Each distribution can be hovered over to display summary statistics.

## Figure 10

:::{figure} #fig10cell
:label: fig10

CAPTION HERE
:::

# Age distribution by study population category

We are particularly interested in how the average age distribution varies across different population categories, especially those expected to be skewed, such as Alzheimer's. The overall age distribution shown in Figure 4 can be seen as a composition of these individual distributions. By separating them, we gain further insight into how different study populations are selected. 

The following raincloud plot visualizes these distributions, similar to Figure 10, but categorized by study population. The box plots show the median (center line), first and third quartiles (box edges), and the minimum and maximum data points at the edge of the whiskers (known as fences), excluding any outliers. In the scatter plots below each boxplot, each black dot represents a study. The overlaid half-violin plots illustrate the density of studies across average participant age for each category. Each distribution can be hovered over to display summary statistics.

 ## Figure 11

:::{figure} #fig11cell
:label: fig11

CAPTION HERE
:::

# Trends in demographic reporting

Given our findings on the lack of demographic reporting, we wanted to examine whether this trend has changed over time. This final visualization tracks the reporting of demographic information over time. A bar plot in the background represents the total number of participants per year, while three line plots show the percentage of studies reporting each demographic variable over time.

## Figure 12

:::{figure} #fig12cell
:label: fig12

CAPTION HERE
:::