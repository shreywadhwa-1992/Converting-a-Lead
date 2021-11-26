# Converting-a-Lead
Significance of Simple Classification Techniques - Logistic Regression

An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. 

The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals. Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%. 

Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone. 

There are a lot of leads generated in the initial stage but only a few of them come out as paying customers. In the middle stage, we have to nurture the potential leads well (i.e. educating the leads about the product, constantly communicating etc.) in order to get a higher lead conversion.

The Major Goal is to predict the promising leads i.e. the leads that are most likely to convert into paying customers. The company wants to build a model wherein lead scores will be assigned to each of the leads such that the customers with higher lead score have a higher conversion chance and the customers with lower lead score have a lower conversion chance. 
Apart from the major goal, the company also wants to know the factors that are majorly contributing towards conversion of the lead. 

Approach Towards the Problem:
1. Data Understanding: 
After Analyzing the Business Goal, looking at the Data we have. Dataset from the past with around 9000 data points. This dataset consists of various attributes such as Lead Source, Total Time Spent on Website, Total Visits, Last Activity, etc. which may or may not be useful in ultimately deciding whether a lead will be converted or not. The target variable, in this case, is the column ‘Converted’ which tells whether a past lead was converted or not wherein 1 means it was converted and 0 means it wasn’t converted. 

2. Data Cleaning:
• Handling large number of null values and columns with large null percentage.
• Defining threshold for dropping columns with more than null percentage than threshold.
• Correcting datatypes.
• Handling incorrect spellings leading to higher cardinalities.

3. Exploratory Data Analysis
• Univariate Analysis – Data imbalance check for Target variable, boxplots and histograms for numeric variables. countplots and pie charts for categorical variables.
• Bivariate Analysis – Bar plots for categorical variables against the target variable. Boxplots for numeric against target variable.
• Weight of Evidence Analysis for categorical variables to determine the feature importance.

4. Data preprocessing for modelling:
• Dummy encoding and ordinal encoding for categorical variables.
• Dropping variables, which can lead to data leakage for target column.
• Standardizing the numeric variables.

5. Model Building:
• Train Test split before modelling
• Logistic Regression using Recursive Feature Elimination and Variance Inflation Factor.
• Using a performance metrics of Precision-Recall and ROC-AUC curve.
• Making the model Lean with only 11 features at the end for targeting.

6. Recommendations:
• If client is spending more than 500 hours on Platform, he/she will more likely to be prospective candidate.
• The variables which are majorly contributing towards in determining the Person are Lead origin-landing page submission, Tags-Already a student and Lead_origin_API. These variables should be checked, if client is falling in any one these categories, he/she has high chances of NOT being converted.
• Tags are most important characteristics while determining the lead. If the clients are associated with Tags stated above. Tags can only be provided after the Clients have been contacted already. Therefore, initial attempt have to made to connect with Client and based on the response or tag provided, Clients should be followed up and resources should be allocated for the Clients to successfully converting them.
• Apart from looking at Tags other variables should also be checked like time spent on page and Lead sources. Clients coming through API, Landing Page, Social Media not specifying their employment are less likely to be converted into a lead.
• During the Internship program, company gets to train many interns. At this stage Manpower is much more and more number of Clients can be focused. 
i. To make the lead conversion more and more aggressive at this stage X-Education can focus on clients with lower lead Scores as well.
ii. Earlier a cutoff of 30 was chosen and leads having a lead score beyond 30 were targeted. Now we can reduce the cutoff value so that leads with lead Scores as low as 10 can also be targeted.
iii. Already converted leads can be contacted for referrals. Referrals should be focused on as they have high chance of being converted because on influence of already converted lead.
• Sometimes, company reaches the Quarter target before the Deadline. At this point, only necessary calls should be made to avoid unnecessary phone call charges.
i. During this period company can focus on marketing the products much more. Marketing can be done on platforms such as televisions, colleges etc.
ii. Providing offers to already converted leads to provide referrals. Provide leads with Emails with attractive offers.
iii. X-Education can form collaborations with a Companies related to the courses offered. So that, employees of companies can be trained through X-education only.
iv. Free Courses, books, blogs etc. should be provided by X-Education, so that leads spend much more time on their platform. The leads spending more time on the Platform have higher chance of being converted.









