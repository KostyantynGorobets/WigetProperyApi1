# WiggetProperyApi1
This is a collection of tests for widgets type integer or double. It has the exemple and you can run it.
For to run your example you should  install :
  1. Node.js - <https://nodejs.org/en/download>
  2. npm - ```npm install -g```
  3. newman - ```newman install -g```                                         
To run the test you need to download the repositories in any folder.
The file Collection.json has the kit of tests for requests API.
The file Environment.json has the kit of variables. These variables you should
edit "value" for your widgets. 
Exempel: 
``` "values": [
		{
			"key": "deviceToken",
			"value": "Your token",
			"type": "default",
			"enabled": true
		},
		{
			"key": "serverUrl",
			"value": "blynk-qa.com",//or blynk.cloud etc
			"type": "default",
			"enabled": true
		}
```                                                   


Don't forget to include pin numbers, dataStream, Min and Max. Property at the console "Show on/off labels" should be enabled.
To run tests - ........./Your folder> newman run Collection.json -e Environment.json
You can edit the number of iterations  ``` -n <number> ``` or timeout between tests ``` --delay-request <number ms> ``` etc. The full kit of commands is <https://www.npmjs.com/package/newman#command-line-options>.
