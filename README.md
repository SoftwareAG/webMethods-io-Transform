# webMethods.io-Transform
## Getting Started
The transform feature lets you perform various operations on the input data in order to help you customize your workflow output or the data you send to the next action. This feature is available in all actions supported by webMethods.io Integration. <br/>
In webmethod.io there are manny transform available for use wrt different data type. <b>Please click on the hyper links to get more details about each data type's Transform. </b>
1. <b>[Array](https://github.com/SoftwareAG/Transform-Array)</b>
2. <b>[Date](https://github.com/SoftwareAG/Transform-Date)</b>
3. <b>[JSON](https://github.com/SoftwareAG/Transform-JSON)</b>
4. <b>[Math](https://github.com/SoftwareAG/Transform-Math)</b>
5. <b>[Util](https://github.com/SoftwareAG/Transform-Util)</b>
6. <b>[Object](https://github.com/SoftwareAG/Transform-Object)</b>
7. <b>[String](https://github.com/SoftwareAG/Transform-String)</b><br/>

## Creating a workflow with transform
1. Log in to your webmethod.io account then go to `webMethods.io Integration`.
2. Create a new workflow under a `Project`.<br/>
![image](https://user-images.githubusercontent.com/60179170/89011752-887bea00-d32e-11ea-83a2-7c6d9196702b.png)<br/>
![image](https://user-images.githubusercontent.com/60179170/89011807-aba69980-d32e-11ea-8f69-557fc494085c.png)<br/>
3. Go to the search pannel on the `connector list` and search `Logger`.<br/>
![image](https://user-images.githubusercontent.com/60179170/89011920-e3154600-d32e-11ea-8d97-f9f839270b7e.png)
4. Now put this logger in your work flow.<br/>
![image](https://user-images.githubusercontent.com/60179170/89012007-07712280-d32f-11ea-9ce8-a8431d98ccec.png)
5. Now `Double Click` on the Logger and click `Next`. On the next window you will get a option `Transform` Click on that.
![image](https://user-images.githubusercontent.com/60179170/89012186-5b7c0700-d32f-11ea-9ba7-37cd3a1c6158.png)
6. Now Click on `add new`. Give the transform a name and select `Transform data` which Transform you want to test. 
![image](https://user-images.githubusercontent.com/60179170/89012757-5075a680-d330-11ea-8380-edf6d69a99f3.png)
7. Now you can provide hard coded values or use a weebhook to pass the values to the transfrom. Click `Done`. 
![image](https://user-images.githubusercontent.com/60179170/89012880-8a46ad00-d330-11ea-8cd2-e88fe525078f.png)
8. Now the transform `output data` to logger `Input` And click `Next` and `Done`.
![image](https://user-images.githubusercontent.com/60179170/89012936-a2b6c780-d330-11ea-9e21-6c71a7dc31cf.png)
9. Now connect the whole workflow `Start` to `End`.
![image](https://user-images.githubusercontent.com/60179170/89013103-ee697100-d330-11ea-817f-44d845020180.png)
10. Now `Run the WorkFlow`. In the logger you will see the result of the transform. Here you can see the length of the string.
![image](https://user-images.githubusercontent.com/60179170/89013245-2ec8ef00-d331-11ea-8127-9d8b7a4ad499.png)

## Using webhook to pass the data.
1. Open the logger and hover over the transform name. You will goin to see a `edit icon` there Click on that icon.<br/>
![image](https://user-images.githubusercontent.com/60179170/89014430-1fe33c00-d333-11ea-9f34-f66e00ee1e4c.png)
2. Now from the Action Configure window cheack what are the input the transform need and its datatypes. Here the transform only need one input and data type is string.<br/>
![image](https://user-images.githubusercontent.com/60179170/89014614-62a51400-d333-11ea-8b4e-d40906093bfb.png)
3. Configure a JSON object wrt the input. <br/>
if the inputs are a string and a array, configure the JSON as <br/>
{"data1":"string","data2":[1,2,3,4]}<br/>
Here the tranfrom need only one input we will configure the JSON as <br/>
{"data1":"Anshuman Saikia"}
4. Now `double click` on the start .<br/>
![image](https://user-images.githubusercontent.com/60179170/88809305-9700bf00-d1d1-11ea-91a2-235dfaf46578.png).
5. From the list click on webhook.<br/>
![image](https://user-images.githubusercontent.com/60179170/89008115-b447a180-d327-11ea-8fbe-e0c48f8f8a92.png)
6. Click `Next`.<br/>
![image](https://user-images.githubusercontent.com/60179170/88910377-05995780-d27a-11ea-99cc-b472dac0f0ef.png)
7. From the next window coppy the link.
![image](https://user-images.githubusercontent.com/60179170/89015385-93d21400-d334-11ea-9b1f-1b30cac54687.png)
8. Now open the Postman and paste the link. And also paste the configured JSON data in the body. <b> keep the body type as `raw` and formate as `JSON` </b>
Click on `Send`.
![image](https://user-images.githubusercontent.com/60179170/89015717-21156880-d335-11ea-9fd9-9f2498a4ec6d.png)
9. Go to your browser and click on `Fetch` on your webhook. After data has been fetch successfully click on `Next`.
![image](https://user-images.githubusercontent.com/60179170/89016124-cd574f00-d335-11ea-8699-6a6f7adcb6be.png)
10. Select and on the Auto Connect return data option and click `Next`. and `Done`.
![image](https://user-images.githubusercontent.com/60179170/89016300-1f987000-d336-11ea-9615-34f804fd620c.png)
11. Now Connect the webhook with the logger and then logger to Return data on Synch and then to Stop.
![image](https://user-images.githubusercontent.com/60179170/89016432-5c646700-d336-11ea-9f2f-fa3fde42d92f.png)
12. Open the `Logger` And go to the `Transform Configure ` window.
![image](https://user-images.githubusercontent.com/60179170/89016544-83229d80-d336-11ea-8c3b-f49eee4e7d54.png)
13. Expand the webhook and map the data to the transfrom input fields. <b> Erase the previous data from the input fields.</b>. Click `Done` and `Next`.
![image](https://user-images.githubusercontent.com/60179170/89016708-cbda5680-d336-11ea-8102-52ad46fb908c.png)
14. Now click on `Test` and `Done`. 
![image](https://user-images.githubusercontent.com/60179170/89017258-a4d05480-d337-11ea-917c-7ff5d8d31deb.png)
15. Now `double click` on  `return data on sync webhook ` connector and map the logger output data to `response data`. Click `Next`. 
![image](https://user-images.githubusercontent.com/60179170/89016785-ef050600-d336-11ea-8587-3a9d9a2792ce.png)
16. 14. Now click on `Test` and `Done`. 
![image](https://user-images.githubusercontent.com/60179170/89017355-d0533f00-d337-11ea-865d-490610b9f6a0.png)
17. Now hover over the weebhook and click on settings icon and coppy the link.
![image](https://user-images.githubusercontent.com/60179170/89017520-0b557280-d338-11ea-93ca-a507d1d4c155.png)
18. Go to the postman and replace this link with the previous one. `Send` we will going to get the output as response.



For more details please [click here](https://docs.webmethods.io/integration/additional_features/data_transformation/#gsc.tab=0).
