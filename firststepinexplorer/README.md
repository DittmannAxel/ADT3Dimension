# Create the windturbine in ADT Explorer

First go through the setup for the service as described here:
https://docs.microsoft.com/de-de/azure/digital-twins/quickstart-azure-digital-twins-explorer 

Stop if you can see the window of the explorer. Than add the *.json files from the files-directory as nodes to the UI.<br>
<p align="center">
<img src ="uploadfile.jpg">
</p><br>
If you have successfully uploaded all the files your explorer should show all these nodes: <br>
<p align="center">
<img src ="nodes.jpg">
</p><br>
And than we need to upload the *.xlsx file to define the graph and use some initial data to populate the nodes.<br>
<p align="center">
<img src ="uploadxlsx.jpg">
</p><br>
After the success message **do not forget to save**, because only after that the graph is in the system. The screen should look like this:<br>
<p align="center">
<img src ="graph.jpg">
</p><br>
And you can also see some intitial values from the *.xlsx file, if you klick on one node:
<br>
<p align="center">
<img src ="initialvalue.jpg">
</p>
<br>
Now query:<br>
<p>
<strong>"SELECT * FROM digitaltwins T where T.powerproduction > 250"</strong></p> <br>
And the result should be: <strong>the node Generator</strong>


<a href="https://github.com/DittmannAxel/ADT3Dimension">-back-</a>


