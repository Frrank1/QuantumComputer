# QuantumComputer
Deploy a Microsoft Quantum Computer in Microsoft Azure

Select the type of Quantum Computer you need, select the number of qubits you need, and click the "Deploy to Azure" button. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmkiernan%2FQuantumComputer%2Fmaster%2Fazuredeploy.json" target="_blank">
   <img alt="Deploy to Azure" src="http://azuredeploy.net/deploybutton.png"/>
</a>


<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fmkiernan%2FQuantumComputer%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

Ok, so it's not really a quantum computer. It's a quantum simulator, based on Microsoft <a href=https://www.microsoft.com/en-us/research/project/language-integrated-quantum-operations-liqui/>LIQUi|></a>

This template deploys an Ubuntu VM with the Microsoft LIQUiD software pre-installed and configured.

You can read more about the Microsoft Quantum Computing project at <a href="https://stationq.microsoft.com/">Microsoft StationQ</a>, and access the LIQUiD "Language Integrated Quantum Operations Simulator" code on <a href="http://stationq.github.io/Liquid/">github.</a>

A complete demo of the Microsoft LIQUiD Software is also <a href="https://www.youtube.com/watch?v=9JEjqiq7pHE">available on YouTube.</a>

Once you've got the (classical) ubuntu machine up, simply follow the <a href="http://stationq.github.io/Liquid/getting-started/">getting started instructions</a>. 

Quick command reference to whet your whistle with some teleportation, entanglement and quantum chemistry:
<ul> 
<li>azureuser@quantum:/Liquid/linux$ mono Liquid.exe</li>
<li>azureuser@quantum:/Liquid/linux$ mono Liquid.exe "__Teleport()"</li>
<li>azureuser@quantum:/Liquid/linux$ mono Liquid.exe "__Entangle1(22)"</li>
<li>azureuser@quantum:/Liquid/linux$ mono Liquid.exe "__Entangle2(4)"</li>
<li>azureuser@quantum:/Liquid/linux$ mono Liquid.exe "__Chem("")"</li>
<li>azureuser@quantum:/Liquid/linux$ mono Liquid.exe "__Chem("H2O")"</li>
</ul>

... and don't forget to have a go at some prime factors with Shor's algorithm. 
