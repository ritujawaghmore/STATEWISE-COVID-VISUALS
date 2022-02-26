# Covid-19_India_Statewise_visualization


## About
The dataset used contains latest Covid-19 India State-wise data till January 2,2022. This dataset has been used to analyze covid in india by using powerbi-desktop to create various visualizations needed to understand covid-19 situation in india state-wise.

In our country, Covid-19 cases have been on the rise, with new mutations/variants cropping up on a regular basis. As a result, understanding, analysing, and visualising COVID-19 state-by-state statistics for our country has become increasingly vital in order to identify the states with the most cases, active cases, deaths, and so on. To study the statewise data for this project, I created a visualisation report with  the help of power-bi, which I then published on a website made with several azure technology. With dynamic visualization report on the data available, we will be able to comprehend the states in need , allowing the concerned authorities to aid in the right distribution of resources to those states, allowing them to manage and control the pandemic crisis to some extent.

## Dataset Attribute Information (<i>Covid-19 India Status.csv</i>)
<p>1. <b>State/UTs</b>- Names of Indian states and union territories.</p>
<p>2. <b>Total Cases</b>- Total number of confirmed cases</p>
<p>3. <b>Active</b>- Total number of active cases</p>
<p>4. <b>Discharged</b>- Total number of dicharged cases</p>
<p>5. <b>Deaths</b>- Total number of deaths</p>
<p>6. <b>Active Ratio (%)</b>- Ratio of number of active cases to total cases</p>
<p>7. <b>Discharge Ratio (%)</b>- Ratio of number of discharged cases to total cases</p>
<p>8. <b>Death Ratio (%)</b>- Ratio of number of deaths to total cases</p>
<p>9. <b>Population</b>- Population of State/UT</p>
   
## How this project was made
1. First created a resource group (Future_ready_talent_project) under which all resouces such as azure-sqldatabase, azure-sqlserver, azure-datafactory , azure-storage(blob)
   and static web app was deployed.
2. Uploaded the Latest Covid-19 India Status.csv to the blob storage in the input container.
3. Wrote sql query in the sqldatabase deployed (running on sql server) to create a table with the column headers that would take the respective data from blob storage 
   during copy data process.
4. Using data factory transferred the data from csv file to sql table using pipeline (Blob to SQL) with help of 2 linked services (input blob, output sql). 
   The pipeline succeeded in transferring data from blob to sql database.
5. After successful transfer of data from blob to sqldatabase , connected the sqldatabase to powerbi-desktop by connecting to sqlserver. Made Visualization using powerbi-
   desktop that can be used to analyze the covid-19 situation in india state-wise. Published the report to powerbi-app to get the secure-emmbbeded code which was added to html 
   file that was made for the static website deployed.
6. Pushed all the html files,png and other files to github repository through github-desktop.
7. Deployed static web app in azure and connected it to github repository to run a website made with basic html integrated with power-bi secure embbeded report.
     
<b> <p>Note that the secure embedded report in the website will not be accessible in most case (will show unavailable if logged in with normal id) because to access it you will     need organization-id of our university.</p>
   <p>To publish the publc url of report is not possible as permission to get that has been restricted by the admin</p>
</b>
<p><b> In case you are unable to see the power-bi dynamic visulization report , I have attached images of the visualization that was created in the website</b></p>

## Project Link -Repository URL
https://github.com/manvithk/Microsoft_futurereadytalent_Covid-19_Statewise_visualization
## Project Demo -Deployment URL
https://black-hill-067e5ca10.azurestaticapps.net

