# mk-query

This tool is just a prototype to highlight the ease of the Meraki API. Lots of refactor is in its future, maybe?   

[Meraki Dashboard v1 reference](https://developer.cisco.com/meraki/api-latest/#!introduction/meraki-dashboard-api)

## TODO

Make this tool not completely suck  

* argparse
* configparse
* structure return JSON(tabulate?)
* make it modular with classes

## Prerequisites

#### API Key  
You will need to generate an API key first:  

[Dashboard API generation](https://documentation.meraki.com/General_Administration/Other_Topics/Cisco_Meraki_Dashboard_API)

#### 3rd Party Modules
readline  
requests  


#### Required files 

#### The tool uses minimal obfuscation through the use of <b>your API</b> key base64 encoded. Instructions below:  

<table><td>
➜  mk-query git:(master) ✗ python<br><br>
Python 3.9.13 (main, May 24 2022, 21:28:31)
[Clang 13.1.6 (clang-1316.0.21.2)] on darwin. 
Type "help", "copyright", "credits" or "license" for more information.   
<br>>>> 
<br>>>>  
<br>
>>> import base64.
<br>
<br>
>>> base64.b64encode(b'yourAPIkeyHere')
<br>
<br>
b'eW91ckFQSWtleUhlcmU='
<br>>>>
</td></table>

</td></table>

Copy the key, excluding the byte distinguisher(<b> eW91ckFQSWtleUhlcmU= </b>) and drop this into a file named 'config' in the root directory. 


## What can it do
Its menu driven currently and very limited

<table><td>
<b>➜  mk-query git:(master) ✗ ./mk-query </b> 

Loading tool.... 
<br>**********  
Meraki query tool
<br>**********  
API Key Loaded!    
Orginization ID: <your orgID>  
API URL: https://api.meraki.com/api/v1/ 
<br>**********  
<br>**********  
1.) List All devices  
2.) List All networks  
3.) Take Camera Screenshot  
4.) Exit  

</td></table>

