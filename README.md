#Personalities_In_Agile
<h2> Master`s Thesis on the The Importance of Personality Traits in Agile Software Development, A Case Study. </h2> 
<h3>Abstract:</h3>
During the last decade, more and more companies have transformed their way of working to agile, making it the most common software development methodology in the industry. The core principle of Agile as given in the original manifesto states, that individuals and their interactions are more important than the tools and processes. This convention leads to the need for the study of the software developer individuals in the psychological level of personality and the performance results associated with the specific personality. There researches that study the personality of the developers and their performances have been set either, in academia, or in the different software development methodology environment, than agile. This study aims to describe the relationship between the software developers’ personalities based on the Big Five model and the performance of the developers based on agile software development metrics. Within this research, the logs of 8 open-source projects that use the most common agile issue tracker, JIRA, are used to retrieve the personality trait of the developers involved and to calculate their performance metrics. Finally, association rules are mined using this dataset, and the consistency of the findings are checked against the existing literature. Evidently, the analysis has shown interesting relationships between the personality types and metrics, that can favour the work of both, the management of the software development teams and the developers themselves.

<h3>Repository</h3>

Source JIRA teams datasets are located in folder input_data/
Data analysis based on the source datasets is done in Jupyter Notebooks. Analysis work is split into three main notebooks:<ul>
    <li>P1_text_mining_IBM_personalities.ipynb</li>
    <li>P2_jira_metrics.ipynb</li>
    <li>P3_association_rules.ipynb</li></ul>
First part is all about extracting and cleaning of the handwritten texts from Jira fields, preparing for the IBM Watson Personality Insights API and retrieving personality traits assesment results of the developers based in their input texts within Big 5 Personality traits model.<br/>
In the second notebook file we fetch data from source dataset and calculate performace metrics.<br/>
In the last part, the former two are combined to create association rules of personality traits and Jira metrics. Furthermore, the results are compared to the findings of E.Scott that was performed in the SCRUM virtual learning environment. Scott et. al used Felder-Silverman`s learning style models in his research, therefore, for comparability, we used the correlation of FSLSM and Big5 model.
