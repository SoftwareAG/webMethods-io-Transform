# Webmethod.io-Transform
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
2. Create a new workflow under a `Project`.
![image](https://user-images.githubusercontent.com/60179170/89011752-887bea00-d32e-11ea-83a2-7c6d9196702b.png)<br/>
![image](https://user-images.githubusercontent.com/60179170/89011807-aba69980-d32e-11ea-8f69-557fc494085c.png)
3. Go to the search pannel on the `connector list` and search `Logger`.
![image](https://user-images.githubusercontent.com/60179170/89011920-e3154600-d32e-11ea-8d97-f9f839270b7e.png)
4. Now put this logger in your work flow.
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


For more details please [click here](https://docs.webmethods.io/integration/additional_features/data_transformation/#gsc.tab=0).
