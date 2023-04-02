# PaymentsSensor Containers Update
This setup will involve the usage of three(3) different containers under Docker-Compose infrastructure. Currenctly only the first two(2) containers will be availiable, containting the database and the Configuration API

* Current release v1.0.0

<p>
<details><summary>How to update the container on a host machine</summary>

<p>

1. Before updating the container you must download the following file depending on your OS:

  >* [PaymentsSensor-Containers-WinSetup.yml for Windows OS](https://github.com/kparginos/PaymentsSensor_Setup/blob/main/PaymentsSensor-Containers-WinSetup.yml)
  
</p>

<p>

2. To update to the latest version you need to do the following:

* For the Windows Host, go to the folder where the .yml file is located and run this command:

```
docker-compose -f PaymentsSensor-Containers-WinSetup.yml pull
```

Once finished, run the following to update the containers:

```
docker-compose -f PaymentsSensor-Containers-WinSetup.yml up -d
```


</p>

</details>
</p>

