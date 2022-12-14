# Instal·lació moodle

Per a començar haurem d'afergir el ssh

![image](https://user-images.githubusercontent.com/104194787/203824274-fd62dc35-e871-45dc-acc6-1bc5cbba4601.png)

Seguidament el que farem serà instalar el apache2

![image](https://user-images.githubusercontent.com/104194787/203826244-03deed88-4c73-4911-be4a-31f152a799b8.png)

Instal·larem mariadb

![image](https://user-images.githubusercontent.com/104194787/203828883-94047302-eca3-444b-abf6-1edb0d67dca3.png)

Ara instal·larem la configuració de mysql

![image](https://user-images.githubusercontent.com/104194787/203829044-413cea1b-9025-49b2-8778-dd1e240f279e.png)

![image](https://user-images.githubusercontent.com/104194787/203829255-4f6e9ea9-dace-4966-aae0-2f61e8874bf1.png)

Comprovem que podem entrar a mariadb

![image](https://user-images.githubusercontent.com/104194787/203829505-85769915-2306-4846-9830-08a7491055e7.png)

Seguidament inst·lalarem el php7.3

![image](https://user-images.githubusercontent.com/104194787/205083138-878c8e75-dfb8-40bf-998b-ffbd38767731.png)

Llavors un cop instal·lat editarem el fitxer per a que es mostre index.php a canvi de index.html.

![image](https://user-images.githubusercontent.com/104194787/203830357-41550f08-b804-482e-bf19-09abe8a38cb7.png)

Seguidament reiniciarem el servidor apache2

![image](https://user-images.githubusercontent.com/104194787/203830529-d061e937-2c5b-4767-aab5-35f474ac4d16.png)

Ara comprovarem que el servidor està actiu

![image](https://user-images.githubusercontent.com/104194787/203830644-cea8b388-343f-46bd-99e5-01c2ff935665.png)

Llavors el que haure de fer serà crear el fitxer index.php

![image](https://user-images.githubusercontent.com/104194787/203830863-2bb81af0-3eac-4df9-8c80-d22ba5281646.png)

![image](https://user-images.githubusercontent.com/104194787/203831054-27d025fe-75b9-45b2-9a12-795054efb80e.png)

Seguidament instal·larem el moodle

![image](https://user-images.githubusercontent.com/104194787/203825041-658851f7-911d-459f-8373-f1ec01fdf778.png)

Llavors descomprimirem la carpeta

![image](https://user-images.githubusercontent.com/104194787/203831654-7f920b39-0965-4b81-ab26-0a9607b34722.png)

Canviarem els permisos

![image](https://user-images.githubusercontent.com/104194787/203831808-84422c65-2502-411d-9fff-c27b04f69ca8.png)

Entrarem al directori de /home, crearem la carpeta "moodledata" i li afegirem els permisos.

![image](https://user-images.githubusercontent.com/104194787/203832227-d41d9beb-fda7-4f40-a375-017bd0877bd1.png)

Seguidament accedirem a la base de dades amb el mode de root.

![image](https://user-images.githubusercontent.com/104194787/203832884-0179948d-fc81-4a53-ac97-1518934891d6.png)

Ara crearem l'usuari de "moodlemanager" dins de la base de dades.

![image](https://user-images.githubusercontent.com/104194787/203833375-839405b2-bdd1-4905-b358-e7c0e2f3c010.png)

Seguidament lo que haurem de fer serà crear la base de dades de moodle

![image](https://user-images.githubusercontent.com/104194787/203833463-d4029bc7-ca23-4a4c-9ece-af1f3857dbb6.png)

Ara li haurem de donar els permisos al usuari

![image](https://user-images.githubusercontent.com/104194787/203833718-e9842ea8-348f-499f-9406-725b5e63aed5.png)

![image](https://user-images.githubusercontent.com/104194787/203833848-a9a2d6e5-829b-4434-afe1-6f1153eaf0e6.png)

Seguidament entrarem al buscador i posarem (la nostra ip)/moodle

![image](https://user-images.githubusercontent.com/104194787/204021266-7f9c42f6-9c41-4564-ad4a-031758dd3fc6.png)

Llavors escollirem l'idioma català

![image](https://user-images.githubusercontent.com/104194787/205074962-5825650b-5c12-4b1d-ac65-7c9412bad06b.png)

Ens sortiran dos errors d'extensions per al PHP

![image](https://user-images.githubusercontent.com/104194787/205075294-f44832bb-9361-4386-8031-e962a52630a8.png)

Per a solucionar els errors haurem d'entrar al directori /var/www/html/moodle i posar la següent comanda:

![image](https://user-images.githubusercontent.com/104194787/205076133-7758d204-4981-4cd6-ab83-151b6b9606f0.png)

A continuació haurem d'entrar al directori /var/www/html/moodle i instal·larem el php7.3

![image](https://user-images.githubusercontent.com/104194787/205077470-ac6fbed8-cbf8-4da3-b299-a1e68789c5cd.png)

Ara farem el mateix que hem fet al curl

![image](https://user-images.githubusercontent.com/104194787/205077709-7f717a13-8b0d-4d68-be1a-f90f140ed5ad.png)

Una vegada fet instal·larem el php7.3 dins del directori /var/www/html/moodle

![image](https://user-images.githubusercontent.com/104194787/205078042-827df7de-6ecb-430b-9813-35c9225e9b30.png)

Ara reiniciarem el servidor apache2

![image](https://user-images.githubusercontent.com/104194787/205078299-b0a4afca-58d0-4ae2-b421-041dea4b6f11.png)

Un cop fet ja haurem entrat i ens demanara que li possesim el directori de dades amb el meu cas l'ubicare dins de home/moodledata

![image](https://user-images.githubusercontent.com/104194787/205079024-75c30000-0743-4fd3-9144-e1517c64a41b.png)

Seguidament sel·leccionarem el controlador de base de dades de MariaDB

![image](https://user-images.githubusercontent.com/104194787/205079214-adad6265-6b8e-485a-8010-74e26cbb7507.png)

Ara li haurem d''afegir un usuari i la contrasenya de la base de dades

![image](https://user-images.githubusercontent.com/104194787/205080335-d75e91d9-e603-4727-a6e3-0e6cbb37b1a1.png)

Seguidament instal·larem l'extensió xml del php7.3

![image](https://user-images.githubusercontent.com/104194787/205085741-a2ef424a-0537-4bf7-af7d-4d54db25a59f.png)

Reiniciarem el servidor i ja estara llest

![image](https://user-images.githubusercontent.com/104194787/205085926-81d2e805-864a-433b-b78b-5ef435377b42.png)

Seguidament haurem d'instal·lar mòdouls php

![image](https://user-images.githubusercontent.com/104194787/205086627-db7be31f-8d9f-4fb1-8242-a7b2fc147661.png)

I com podem veure un cop instal·lats tots els mòduls ens sortira tot correcte

![image](https://user-images.githubusercontent.com/104194787/205086917-fae580cb-7694-4709-9e6d-e79d6192e163.png)

Ara haurem de posar les dades de l'usuari

![image](https://user-images.githubusercontent.com/104194787/205089434-5289e9ea-e7da-4a64-a5c2-9a69a580bb9c.png)

![image](https://user-images.githubusercontent.com/104194787/205089898-4e488d14-1a29-4d7e-99ec-40618b2f98cf.png)

Ara haurem d'afegir més parametres

![image](https://user-images.githubusercontent.com/104194787/205090807-7829cfa9-18b3-49cb-8254-b23745a5ed5d.png)

Ja estarem dins del moodle

![image](https://user-images.githubusercontent.com/104194787/205091201-0a3b72fe-563d-4347-affc-45d4e03a979d.png)
