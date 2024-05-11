# IT-Specialist-Data-Analytic-3

Welcome to "IT Specialist for Data Analytics 3"! 🌟

Prepare to delve into the essential skills of Data Visualization and Communication, as well as Responsible Analytics Practices. Throughout this course, we'll guide you to effectively report data, create meaningful visualizations, and derive actionable conclusions. Additionally, we'll explore crucial topics such as data privacy laws, responsible data handling, and identifying and mitigating biases in data collection and interpretation.

Get ready to enhance your abilities in conveying insights through tables, charts, and visualizations, and to navigate the ethical considerations of data analysis. Let's embark on this journey of mastering the art of data-driven decision-making together!

Thanks for joining us on this learning adventure! 🚀📊

# Data Visualization Using Python
Python offers several plotting libraries, namely Matplotlib, Seaborn, and many other such data visualization packages with different features for creating informative, customized, and appealing plots to present data in the most simple and effective way.

## Matplotlib and Seaborn
Matplotlib and Seaborn are Python libraries that are used for data visualization. They have inbuilt modules for plotting different graphs.

`1. Matplotlib`
- It is used for basic graph plotting like Line Chart, Bar Graphs, etc.
- It mainly works with datasets and arrays.
- Matplotlib acts productively with data arrays and frames. It regards the aces and figures as objects.
- Matplotlib is more customizable and pairs well with Pandas and Numpy for Exploratory Data Analysis.
  
`2. Seaborn`
- It is mainly used for statistics visualization and can perform complex visualizations with fewer commands.
- It works with entire datasets.
- Seaborn is considerably more organized and functional than Matplotlib and treats the entire dataset as a solitary unit.
- Seaborn has more inbuilt themes and is mainly used for statistical analysis.

```python
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns
```

## Line Chart
A line chart is a graph that represents information as a series of data points connected by a straight line. In line charts, each data point or marker is plotted and connected with a line or curve.

Let's consider the apple and manggo yield (tons per hectare) in Kanto. Let's plot a line graph using this data and see how the yield of apples and manggo changes over time. We are going to both plot by using Matplotlib and Seaborn as follows:

`Using Matplotlib`

```python
plt.plot(years, apples)
plt.plot(years, manggo)

plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')

plt.title('Crop Yields in Kanto')
plt.legend(['Apples', 'Manggo'])
```
<div align="center"><img src="https://github.com/Aisyahrahmap/IT-Specialist-Data-Analytics-3/assets/166115307/bc50f730-3665-4783-880e-beec89b9ef61" /></div>


Chart in Python. For make a chart use `matplotlib and seaborn`.
<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/5205be3f-f7ae-44cc-ae13-79ddc0ba10da" /></div>

You can also add `years` if you data is timestamp.

<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/805534d1-bf6a-405a-8a94-cc2b1e0439ce" /></div>

Add label for for easiest your chart visualization.

<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/85ec896d-64ac-45a9-b6e0-456ce64b58ea" /></div>

### Multiple Datasets 

Multiple datasets means you have `more than 1` datasets.

<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/ca2a36e3-66ff-4dd8-b370-1d0498c96b0e" /></div>

If multiple datasets make it difficult for you to read your chart, use a `legend`.

<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/1e737c43-81a4-45f1-b9da-8d7ea4e2f2e3" /></div>

### Dataframe

If your data is in a dataframe, we can use seaborn (sns).
syntax:
> ax = sns.lineplot(x='Name', y='Name', data = name_data)
> 
> ax1 = sns.lineplot(x='Name2', y='Name2', data = name_data)
> 
> plt.show()

<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/ce5fe3c1-1c59-4749-93e7-d9066f0fd43d" /></div>

But you can use matplotlib if you need bar chart.
Syntax:
> plt.bar(name_x, name_y)
>
> 
> plt.xlabel('name_x')
> 
> plt.xlabel('name_x')
>
> 
> plt.title("title_chart")


<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/265b1edf-cfac-40e6-b56b-8ad984ec7759" /></div>

#### Stacked Bar Chart

<div align="center"><img src="https://github.com/salsanssp/IT-Specialist-Data-Analytic-3/assets/166114037/b56232ab-f2b2-437d-9346-e7c4aafc9085" /></div>

*1. Business Understanding*
     
  The Business Understanding phase focuses on understanding the objectives and requirements of the project. Aside from the third task, the three other tasks in this phase are foundational project management activities that are universal to most projects:  

- *Determine business objectives*: You should first “thoroughly understand, from a business perspective, what the customer really wants to accomplish.”
- *Assess situation:* Determine resources availability, project requirements, assess risks and contingencies, and conduct a cost-benefit analysis.
- *Determine data mining goals:* In addition to defining the business objectives, you should also define what success looks like from a technical data mining perspective.
- *Produce project plan:* Select technologies and tools and define detailed plans for each project phase.

### 6 phase of the CRISP-DM:

*1. Business Understanding*
     
The Business Understanding phase focuses on understanding the objectives and requirements of the project. Aside from the third task, the three other tasks in this phase are foundational project management activities that are universal to most projects:  

- *Determine business objectives:* You should first “thoroughly understand, from a business perspective, what the customer really wants to accomplish.”
- *Assess situation:* Determine resources availability, project requirements, assess risks and contingencies, and conduct a cost-benefit analysis.
- *Determine data mining goals:* In addition to defining the business objectives, you should also define what success looks like from a technical data mining perspective.
- *Produce project plan:* Select technologies and tools and define detailed plans for each project phase.

*2. Data Understanding*

Adding to the foundation of Business Understanding, it drives the focus to identify, collect, and analyze the data sets that can help you accomplish the project goals. This phase also has four tasks:   

- *Collect initial data:* Acquire the necessary data and (if necessary) load it into your analysis tool.  
- *Describe data:* Examine the data and document its surface properties like data format, number of records, or field identities.  
- *Explore data:* Dig deeper into the data. Query it, visualize it, and identify relationships among the data.  
- *Verify data quality:* How clean/dirty is the data? Document any quality issues.

*3. Data Preparation*

This phase, which is often referred to as “data munging”, prepares the final data set(s) for modeling. It has five tasks:  

- *Select data:* Determine which data sets will be used and document reasons for inclusion/exclusion.  
- *Clean data:* Often this is the lengthiest task. Without it, you’ll likely fall victim to garbage-in, garbage-out. A common practice during this task is to correct, impute, or remove erroneous values.  
- *Construct data:* Derive new attributes that will be helpful. For example, derive someone’s body mass index from height and weight fields.  
- *Integrate data:* Create new data sets by combining data from multiple sources.  
- *Format data:* Re-format data as necessary. For example, you might convert string values that store numbers to numeric values so that you can perform mathematical operations.

*4. Modeling*

What is widely regarded as data science’s most exciting work is also often the shortest phase of the project. Here you’ll likely build and assess various models based on several different modeling techniques. This phase has four tasks:  

- *Select modeling techniques:* Determine which algorithms to try (e.g. regression, neural net).  
- *Generate test design:* Pending your modeling approach, you might need to split the data into training, test, and validation sets.  
- *Build model:* As glamorous as this might sound, this might just be executing a few lines of code like “reg = LinearRegression().fit(X, y)”.  
- *Assess model:* Generally, multiple models are competing against each other, and the data scientist needs to interpret the model results based on domain knowledge, the pre-defined success criteria, and the test design.

*5. Evaluation*

Whereas the Assess Model task of the Modeling phase focuses on technical model assessment, the Evaluation phase looks more broadly at which model best meets the business and what to do next. This phase has three tasks:  

- *Evaluate results:* Do the models meet the business success criteria? Which one(s) should we approve for the business?  
- *Review process:* Review the work accomplished. Was anything overlooked? Were all steps properly executed? Summarize findings and correct anything if needed.  
- *Determine next steps:* Based on the previous three tasks, determine whether to proceed to deployment, iterate further, or initiate new projects.

*6. Deployment*

A model is not particularly useful unless the customer can access its results. The complexity of this phase varies widely. This final phase has four tasks:

- *Plan deployment:* Develop and document a plan for deploying the model  
- *Plan monitoring and maintenance:* Develop a thorough monitoring and maintenance plan to avoid issues during the operational phase (or post-project phase) of a model  
- *Produce final report:* The project team documents a summary of the project which might include a final presentation of data mining results.  
- *Review project:* Conduct a project retrospective about what went well, what could have been better, and how to improve in the future.

## Responsible Analytics Practices
### Describe data privacy laws and best practices
 1. GDPR : The General Data Protection Regulation is a regulation that governs data protection, where users must give permission before their personal data can be used.  `GDPR` is binding and must be complied with by all online service providers, including website owners.
    - Attack notification
    -  Right to access data
    -  Right to Erasure
    -  Data transfer
    -  Privacy is the main focus of the system
    -  Data Protection Officer
 2. FERPA : The Family Educational Rights and Privacy Act `(FERPA)` is a federal law in the United States that governs the privacy of student education records. `FERPA` ensures that educational institutions maintain the confidentiality, integrity, and availability of all student personal data governed by `FERPA`. Records protected by `FERPA`:
    - Educational Information: Records related to grades, course transcripts, financial accounts or loans, student assessments, assignments, or attendance.
    - Directory Information: These records refer to PII that is used to identify students for administrative purposes and include addresses, phone numbers, dates related to attendance or enrollment, and others. According to `FERPA`, these records are only guaranteed confidentiality if the student requests.
      
 3. HIPAA : (The Health Insurance Portability and Accountability Act) protects the privacy of personal health information (PHI) and medical records. It applies to health plans, healthcare clearinghouses, and healthcare providers that electronically conduct certain healthcare transactions.
    
 4. An Institutional Review Board (IRB) is an administrative body established to protect the rights and welfare of research subjects involving humans recruited to participate in research activities conducted under the auspices of the institution with which it is affiliated. The review by the IRB is guided by the under-listed four basic principles espoused in the Belmont Report:
    - Autonomy: respect for the research subject (human). This is the derivative principle for informed consent.
    - Beneficence: be kind to participants
    - Non-maleficence: avoid violence or harm to research participants
    - Distributive Justice: Research participants should be selected fairly. Therefore, the burdens and benefits of the research must be fair.

 5. PCI DSS stands for Payment Card Industry Data Security Standard. It is a set of security standards that aim to protect cardholder data and reduce the risk of fraud and data theft.

 ### Describe best practices for responsible data handling
 1. Methods of handling PII
    Personally Identifiable Information (PII) is data that can be used to identify or contact an individual. Handling PII must follow rules like GDPR in Europe, CCPA in California, and other global data protection regulations. The best ways to manage PII include protecting data with encryption, ensuring only authorized people can access it, and conducting audits and monitoring to prevent and detect unauthorized activities.
    
 2. Securing data
    Data security includes physical and digital measures to protect data from unauthorized access, damage, or loss. Threats to databases include theft and fraud. Perform regular data backups and design effective recovery plans, implement security protocols such as HTTPS and TLS for data transmission and use strong firewalls, and conduct regular penetration testing and security evaluations.
    
 3. Protecting anonymity with in small data
    Protecting anonymity within small data is crucial, especially when dealing with sensitive information. Here are some strategies to achieve this:
    - Aggregation and Generalization: Combine data points to create broader categories. For example, instead of storing individual ages, group them into age ranges.
    - Perturbation: Introduce random noise to the data. This makes it harder to identify specific individuals. However, striking the right balance between privacy and utility is essential.
    - K-Anonymity: Ensure that each record in the dataset is indistinguishable from at least k-1 other records. This prevents re-identification of individuals.
    -  Differential Privacy: Add controlled noise to query results to protect individual privacy. Differential privacy guarantees that the presence or absence of any individual’s data does not significantly affect the outcome.
  
 4. Protecting anonymity within small data
    In the context of increasing the level of anonymization or obfuscation of data, there is a trade-off between interpretability and the usefulness of the data for analysis.
    - Interpretability: The ability to understand and explain how data is processed and models are built. The higher the level of anonymization, the harder it is to interpret the data.
    - Data Usability: Data that is too anonymized may lose value for analysis. It is important to consider the usability of the data in a business or research context.
      Organizations should consider this compromise wisely. Consultation with legal and ethical experts is also necessary to ensure regulatory compliance and privacy protection.

5. Shortcomings of Making Population-level Generalizations with Limited Sample Data
   Drawing conclusions about the entire population based on a small sample size may result in biased or inaccurate results. A sample size that is too small may not reflect the variation present in the entire population, so generalizations made from the sample may not be generally applicable. Therefore, it is important to understand the limitations of small sample data and be cautious about making broader conclusions without sufficient evidence.

### Describe types of bias that affect collection, and interpretation of data
1. Confirmation Bias
   Confirmation bias refers to the tendency of individuals to seek out or interpret information that aligns with their existing beliefs or values. It’s a cognitive bias that affects decision-making and information processing.A project manager who holds a strong belief that their project will meet its deadline may be inclined to actively seek and emphasize data that demonstrates positive advancement, while simultaneously overlooking or minimizing indications of possible delays.
   
2. Human cognitive Bias
Cognitive bias refers to the systematic errors in thinking that influence how we process information, perceive others, and make decisions. These biases can lead to irrational thoughts or judgments and are often based on our perceptions, memories, or individual and societal beliefs. An example of a cognitive bias is the availability heuristic. This bias occurs when individuals make judgments about the likelihood of events based on how easily they can recall examples from memory.

3. Motivasional  Bias
Motivational bias refers to the tendency for individuals to interpret information or make decisions in a way that aligns with their pre-existing motivations or desires. These motivations can be conscious or unconscious and may influence perception, judgment, and behavior. Someone who is strongly motivated to maintain a positive self-image might interpret feedback in a way that supports their self-esteem, while disregarding or minimizing criticism. Similarly, individuals may be motivated by financial incentives, social approval, or personal goals, leading them to exhibit biased behavior in pursuit of these motivations.
   
4. Sampling  Bias
Sampling bias occurs when the sample used in a study or survey is not representative of the larger population, leading to skewed or inaccurate results. For example, suppose a researcher wants to study the favorite ice cream flavors of people in a city. They decide to conduct their survey at a local ice cream shop during the day. However, this sampling method might introduce bias because it only captures responses from people who visit the ice cream shop during that specific time period.
  People who are unavailable during the day or who prefer different activities might be excluded from the sample, leading to an overrepresentation of individuals who enjoy ice cream and potentially biasing the results towards certain flavors. In this case, the sampling method does not accurately represent the broader population's preferences for ice cream flavors, resulting in sampling bias.
   
5. Selecting Visualizations/Data Representations to Avoid Bias
   Selecting visualizations and data representations to avoid bias involves choosing appropriate methods to accurately and transparently present data without distorting or misleading interpretations. This process includes considering the audience, using diverse visual formats, avoiding misleading visuals, providing contextual information, being transparent about data selection and processing, considering alternative representations, testing for bias, highlighting uncertainty, avoiding cherry-picking data, and promoting accessibility.

# Data Analytics Journey 🌟


Thank you for joining us in "IT Specialist Data Analytics 3" where we've explored a wealth of resources and code snippets to elevate your skills in data analytics. From mastering data visualization and responsible analytics practices to navigating biases and privacy laws, we've embarked on an enlightening journey together. Keep analyzing with confidence! 🚀 Happy exploring! 📊✨
