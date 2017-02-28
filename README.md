# sUAS-ODK-forms
ODK sample forms for capturing sUAS flight metadata
#HowTo on using ODK for sUAS metadata capture
##Introduction
This is a HowTo/demo for trying out using Open Data Kit [ODK](https://opendatakit.org/) as a means of  capturing  small Unmanned Aircraft Systems [sUAS] relevant metadata.  Full details on setting up your own server and customising your own forms can be found in the great ODK documetation.  This readme will only show you how to use the forms supplied in this repo and how to upload data to a demo supplied server infrastructure that I've setup.  To use ODK for **your** sUAS operations you will need to set up your own systems but hopefully this demo is enough for you to decide if that's a good idea or not.  

In brief, ODK allows you to make and fill out custom forms on an android/iOS phone, and have the data synced/backed up on a self hosted server for later analytics.  The steps to acomplishing this in brief are:
1. Setup a serve hosting [Aggregate](https://opendatakit.org/use/aggregate/) Aggregate
2. Create (or copy/edit one from here) a relevant form and upload it to your server.
3. Install ODK Collect on your android phone and connect it to your server.
4. Collect data.

##Try it out 
###Step1: Setup your phone
1. Install ODK on your phone (just search the play store)
2. Configure ODK on your phone to connect to **my** server hosting these example forms:
-- In the app go to "General Settings" > "Configure platform settings" > URL
-- Paste: http://138.68.56.54:8080/ODKAggregate/
![](./images/Android3s.png) 


###Step2: Try entering data
1. In ODK app > Main Menu > "Get Blank Form" > download which ever form you want
2. Main Menu > "Fill Blank Form" > select which ever form you wish and fill it in. Move to the next question by swiping left.
3. Name and save the form.
4. Main Menu > "Send Finalised Form" to submit it to the Aggregate server.
5. ![](./images/Android4s.png) ![](./images/Android2s.png) ![](./images/Android1s.png)

###Step3: Visualise and use data in Aggregate (or simply retain for civil aviation records purposes)
![](./images/Aggregate1.png) 


##Helpful next steps
If you liked what you saw the next steps to having your own system are:
1. Setup [Aggregate](https://opendatakit.org/use/aggregate/) Aggregate on a internet accessible server.  For simplicity ODK does offer a AWS deployable instance and allows forms to be sent directly to a Google docs account.
2. Customise a xls (Excel/Libre) spreadsheet to your own needs, see:
- The ODK example form [here](https://opendatakit.org/wp-content/uploads/2013/06/sample_xlsform.xls) 
- The xls form sytax documentation is [here](http://xlsform.org/)
3. Create an xml form out of a xls document by uploading it [here](http://opendatakit.org/xiframe/) and downloading the resulting xml form.
![](./images/Convert1.png) 
4. Upload your custom xml form to your aggregate server and start capturing data.





