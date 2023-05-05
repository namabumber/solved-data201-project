Download Link: https://assignmentchef.com/product/solved-data201-project
<br>
The El Nin˜o-Southern Oscillation (ENSO) is a cycle of warm and cold surface sea water temperatures in the southern Pacific Ocean. As the area of warm sea water moves the air pressure gets higher on either the east or west of the Pacific. This has an effect on rainfall and temperature globally, but given our geographic location, it has a very strong effect on New Zealand weather. The cycle varies between two and seven years, with an average of four years.

In this project you are going to investigate exactly what kind of effect it has on New Zealand, and see if you can predict the strength of the El Nin˜o into the future.

There are three datasets provided as projectdata.zip in the dataset section of the course webpage. They are all from the Ministry for the Environment (https://data.mfe.govt.nz/. The data is in the csv files, which there is various information in the other files in the zip package.

<ol>

 <li>Load all three files into Python and take a look at them. Ensure that you understand what isrecorded in each. Compare the geographic locations of data collected, and the years. Create new dataframes that contain only the data for matched years and locations where appropriate. Deal appropriately with NaN datapoints. (3 marks)</li>

 <li>Make plots of the various timeseries and check if you can see the expected temporal patternin the ENSO index. (3 marks)</li>

 <li>Test whether or not there is a correlation between the rainfall and temperature and the index.(4 marks)</li>

</ol>

1

<ol start="4">

 <li>Test whether or not this correlation is stronger or weaker in different parts of the country. (5 marks)</li>

 <li>Using the Auckland data, predict the strength of the ENSO index for each year using therainfall and temperature data. You will need to:

  <ul>

   <li>Choose the appropriate data and normalise it</li>

   <li>Split it into training and testing sets</li>

   <li>Choose an appropriate algorithm</li>

   <li>Perform the training</li>

   <li>Report appropriate metrics</li>

  </ul></li>

</ol>

(15 marks)

<ol start="6">

 <li>Using just the ENSO index data, see if you can predict the strength of the ENSO index fordate <em>t </em>+ 1 using the index values for dates <em>t </em>− 1<em>,t </em>− 2<em>,t </em>− 3. The easiest way to do this is to assemble the data into an array with 3 columns. The first few rows would be (where <em>I<sub>m</sub></em><sub>−<em>y</em></sub><em>t </em>is the index value for date month-year):</li>

</ol>

<table width="146">

 <tbody>

  <tr>

   <td width="54"><em>I</em>01−86</td>

   <td width="54"><em>I</em>02−86</td>

   <td width="38"><em>I</em>03−86</td>

  </tr>

  <tr>

   <td width="54"><em>I</em>02−86</td>

   <td width="54"><em>I</em>03−86</td>

   <td width="38"><em>I</em>04−86</td>

  </tr>

  <tr>

   <td width="54"><em>I</em>03−86</td>

   <td width="54"><em>I</em>04−86</td>

   <td width="38"><em>I</em>05−86</td>

  </tr>

 </tbody>

</table>

Then use the first line to predict <em>I</em><sub>04−86 </sub>and so on.

You need to follow the same data preparation steps as in the previous question.

Compare the model with two others:

<ul>

 <li>Using the last 6 monthly values instead of the last 3</li>

 <li>Using the last 12 monthly values instead of the last 3</li>

</ul>

Explain why you get the results you do. (15 marks)

<ol start="7">

 <li>Test whether or not the ENSO is getting stronger or weaker over time. (5 marks)</li>

</ol>

2