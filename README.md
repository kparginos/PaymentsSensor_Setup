# PaymentsSensor Containers Update
This setup will involve the usage of three(3) different containers under Docker-Compose infrastructure. These containers are described as following:
1. The Database container which will maintain all the configuration information for the Email Scanner API
2. The Email Scanner Configiuration API
* Current release v1.0.2

3. The Email Scanner API

* Current release v1.2.0

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
</details>

<details><summary>Enhancements</summary>
  
* ### Configuration app version 1.0.2:

>1. New fields included to support MS-Graph authentication.

* ### Scanner app version 1.2.0:

>1. Scanner now supports MS-Graph authentication in order to be able to read emails.

</details>
</p>

