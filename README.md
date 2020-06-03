# Comandos de Drozer

Algunos comandos para manejar la herramienta Drozer

- Comandos de conexión

adb forward tcp:31415 tcp:31415

drozer console connect --server 192.168.0.2

- sacar el nombre de la apk

run app.package.list

- Superficies de ataque

run app.package.attacksurface com.android.insecurebankv2

- Información de los permisos

run app.package.info -a com.android.insecurebankv2

- detecta los permisos de Broadcast

run app.broadcast.info -a com.android.insecurebankv2

run app.broadcast.info -a com.android.insecurebankv2 -i

- busca vulnerabilidad

run scanner.provider.injection -a com.android.insecurebankv2

- ver información de urls

run scanner.provider.finduris -a com.android.insecurebankv2

- Ver la información de los activities

run app.activity.info -a com.android.insecurebankv2

run app.activity.info -a com.android.insecurebankv2 -u

--> Ver los activities de forma directa

run app.activity.start --component com.android.insecurebankv2 com.android.insecurebankv2.ChangePassword

- información del manifest

run app.package.manifest com.android.insecurebankv2
