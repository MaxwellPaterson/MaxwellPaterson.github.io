# Portfolio Scorecard Report

## The Project

This project was created as a way to quickly and easily look at the metrics associated to different buildings that were in our database.  

<p align = 'center'>
  <img src="/images/scorecardview.png?raw=true" height = "80%" width = "80%"> 
</p>

During the development of this dashboard I learned a lot of new things about excel. This is mainly due to the fashion in which I was trying to construct this project. The main unique thing about this Excel project for me was that all of the visuals run off of the same sheet, and the same cells. There is no need to create static data for each of the buildings. Instead I have created a dynamic data sheet that the charts run off of, where as you change the building you want to look at all of the data is automatically recalculated. This reduces the amount of calculations needed in this spreadsheet as we do not have to calculate for each of the building individually.  

<p align = 'center'>
  <img src="/images/portfoliodropdown.png?raw=true" height = "50%" width = "50%"> 
</p>  

With the nature of the dynamic dashboard, some buildings are going to have more or less data than others. This causes a problem when creating the charts, if one building has five years of data and the other one only has one, we do not want to have static charts that always display five years. The workaround I found for this is using **Name Manager**.   

<p align = 'center'>
  <img src="/images/portfolionamemanager.png?raw=true" height = "50%" width = "50%"> 
</p>  

This is a feature that I had previously never worked with but it proved very helpful in this specific instance. With this feature I am able to create a formula, that shrinks and grows to the amount of data present for whichever building is specific. This is very important because then I can reference these formulas in the charts I create, instead of having to reference a static amount of cells. This gives the charts I have made the ability to change dimensions on their own, from displaying five years to displating two years automatically and not leaving the formatting looking poor.  
  
<p align = 'center'>
  <img src="/images/portfoliosizechange.png?raw=true" height = "80%" width = "80%"> 
</p>

Of course there is lots of other very carefully created formulas in this project that have not been discussed here. If you want to play around with the excel file click <a href="https://1drv.ms/x/c/84f846ad7ca6106f/EQ7pIhZu0GJFuhwN4TXQvMwBS1zvFsW-83QJw9Vxija5fQ?e=fYrijr" target="_blank" rel="noopener noreferrer"> here </a>.

Due to privacy reasons all the numbers and names in this project have been changed and do not represent the actual emmisions or usages of any buildings.
