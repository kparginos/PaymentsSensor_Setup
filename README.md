# PaymentsSensor Containers Update
This setup will involve the usage of three(3) different containers under Docker-Compose infrastructure. These containers are described as following:
1. The Database container which will maintain all the configuration information for the Email Scanner API
2. The Email Scanner Configiuration API
* Current release v1.1.0

3. The Email Scanner API

* Current release v1.2.7

<p>
<details><summary>How to update the container on a host machine</summary>

<p>

1. Before updating the container you must download the following file depending on your OS:

  >* [PaymentsSensor-Containers-WinSetup.yml for Windows OS](https://github.com/kparginos/PaymentsSensor_Setup/blob/main/PaymentsSensor-Containers-WinSetup.yml)
  
</p>

<p>

2. To update to the latest version you need to do the following:

* For the Windows Host, go to the folder where the .yml file is located and run the following command:

```
docker-compose -f PaymentsSensor-Containers-WinSetup.yml pull
```

Once finished, run the following to update the containers:

```
docker-compose -f PaymentsSensor-Containers-WinSetup.yml up -d
```


</p>

</details>
  
<details><summary>Bug Fixes</summary>

* ### Scanner app version 1.2.5:

> Fix made to save attachments under separate folder when sender has multiple receivers, where part of file name is the receiver subfolder
  
* ### Scanner app version 1.2.1:

>1. Fix made to scan all availiable emails.
  
>2. Fix made to store attachments to folder based on Sender's Code as this is defined in the configuration.
  
</details>

<details><summary>Enhancements</summary>

* ### Configuration app version 1.1.0(latest):

> Allow user to specify the keyword to be used in order to detect the href link on the email body, which leads to the attachment to be downloaded
  
* ### Configuration app version 1.0.8:

> Add sorting capabilities to tables for all pages.

* ### Configuration app version 1.0.7:

> Service Broker support for future use by the Analyzer
 
* ### Configuration app version 1.0.6:

>1. Configuration now support Senders with multiple receivers based on delimeter at the attachment file name.
>2. List of Senders are sorted by name
  
* ### Configuration app version 1.0.5:
  
> Configuration app supports refresh of the active configurations when a change is made to the database

* ### Scanner app version 1.2.7(latest):

> Scanner app adds timestamp to file downloaded from link at the email body

* ### Scanner app version 1.2.6:

> Scanner app now supports the ability to download attachment provided in email by a link

* ### Scanner app version 1.2.4:

> Scanner now support Senders with multiple receivers based on delimeter at the attachment file name.

* ### Scanner app version 1.2.3:

>1. Scanner app creates attachments folder under date in which the email has beeen received

>2. Restart of the app with logout all logged in users.

* ### Scanner app version 1.2.0:

>1. Scanner now supports MS-Graph authentication in order to be able to read emails.

</details>
</p>

