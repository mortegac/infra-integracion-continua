# 


Versión 1

:

* [Jenkins](https://jenkins.io/)
### Que es Jenkins?
Servidor de integración continua opensource y muy utilizado. En el proceso de integración continua Jenkins permite programar tareas en las que se compruebe un repositorio de contro de versiones donde se ueda compilar y correr test.
Si el resultado no es el esperado o existen errores Jenkins lo comunica a Sonarqube o genera alguna alerta por email u otro medio


* [Sonarqube](https://www.sonarqube.org/) 
### Que es Sonarqube?
Plataforma opensource para evaluar el código fuente de una aplicación. Inicialmente fue desarrollado para Java pero permite mediante Plugins otros lenguajes de programación.  Se integra con Maven, Ant y herramientas de integración continua como Atlassian Bamboo, Jenkins y Hudson).

![Diagrama Funcionamiento](https://camo.githubusercontent.com/a3ea8f9dd6be7e3bcf4b16f6f781b51171f51010/68747470733a2f2f312e62702e626c6f6773706f742e636f6d2f2d51386b326a6a4b534c47592f5672757370316f78776b492f4141414141414141414f342f6c526a4a50425572636f632f73313630302f323031362d30322d31305f31362d32312d33312e706e67)

___________________________________________________________________________
## INSTALACION  ##

1.- Instalar NodeJS y NPM: 

* Para sistemas operativos Linux 	y Windows [Ingrese Aqui](http://www.w3resource.com/node.js/installing-node.js-windows-and-linux.php)
* Para sistemas operativos OSX [Ingrese Aqui](https://coolestguidesontheplanet.com/installing-node-js-on-macos/). 
* Si necesita utilizar varias versiones de node puede usar [nvm](https://github.com/creationix/nvm)

2.- Instalar dependencias:   
```
$ yarn install o npm install
```

3.- Instalar Docker-Compose:
	
```
[Resumen instalación](https://gist.github.com/mortegac/db6a824fcc94b900672326eabe44464b)

[Repositorio y más información]
(https://github.com/docker/compose)
```


___________________________________________________________________________
## EJECUCION ENTORNO DE DESARROLLO  ##

Para ejecutar el entorno de Desarrollo fue considerado el uso de contenedores en Docker, fue consideradas imagenes con jenkins, sonarqube y PostgreSQl .

1.- Instalación y Pre-Requisitos para instalar Docker-Compose`: 
	* [Procedimeinto de instalación](https://docs.docker.com/compose/install/#prerequisites)  

2.- Estructura de carpetas`:  Se considero el uso de la siguiente estructura 
	
```
│   ├── jenkins
│   └── postgres
│	
│   └── sonarqube_extensions
│   └── sonarqube_plugins
│	
└── docker-compose.yml
```
Donde:

___________________________________________________________________________
## EJECUCION  ##

* [Servidor de Jenkins localhost:8080](http://localhost:8080/)  

* [Servidor de Sonarqube localhost:9000](http://localhost:9000/)  
