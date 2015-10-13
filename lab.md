# Pizza Developer

##### Requerimientos

  - Instalar NodeJS v0.12.4, si cuenta con una version superior a esta instalar nvm.
  - Android
    - Instalar JDK , Apache Ant, Gradle y Android SDK, asegurarse de que se puede ejecutar comandos de estos desde la terminal.
  - iOS
    - Instalar Xcode, Xcode CLI Tools, iOS SDK, Brew y Cocoapods. 

> Instalar nativescript desde la terminal usando npm:
 - npm install -g nativescript
 
>En sistemas operativos basados en UNIX puede requerir usar sudo:
>- sudo install -g nativescript

Cuando terminemos de instalar `nativescript` , en la terminal o consola de windows escribimos `tns` y lo ejecutamos

```
$ tns
```

Entonces se desplegara una lista de comandos, si la puedes ver, entonces estamos listos para comenzar.

```
$ tns
# NativeScript
+--------------------------------------------------------------------------+
¦ Usage   ¦ Synopsis                                                       ¦
¦ General ¦ $ tns <Command> [Command Parameters] [--command <Options>]     ¦
¦ Alias   ¦ $ nativescript <Command> [Command Parameters] [--command       ¦
¦         ¦ <Options>]                                                     ¦
+--------------------------------------------------------------------------+
## General Commands
...
```
## Paso 1: Clone el repo del taller o crea un nuevo proyecto de nativescript.

El repo contiene el template inicial de nuestra aplicacion :

```
$ git clone https://github.com/kiramishima/nativescript-workshop-starter-template.git
```

Crear un nuevo proyecto, sin clonar el repo : 

```
$ tns create PizzaDeveloper
```

Accedemos al directorio generado : 

```
$ cd nativescript-workshop-starter-template  --- Si estamos usando el repo
$ cd PizzaDeveloper -- Si estamos usando el que creamos sin bajar el repo.
```

## Paso 2: Agregar las Plataformas

Antes de que puedas correr esta app, NativeScript necesita inicializar la plataforma especifica para nuestro proyecto objetivo. Podemos iniciar agregando la plataforma de Android:

```
$ tns platform add android
```

Si estan trabajando en una Mac, puedes agregar la plataforma para iOS : 

```
$ tns platform add ios
```

Esta operacion usa los SDKs nativos para inicializar la plataforma especifica del proyecto y genera contenido en el directorio `platforms` de tu app.

## Paso 3: Correr el App

Despues de agregar la plataforma o plataformas, podemos lanzar la aplicacion en los emuladores o dispositivos que tengamos.
En Mac solo podremos ejecutar el app en el emulador.

```
$ tns run ios --emulator
```

En Android, podemos lanzar el app en el emulador ( --emulator ) del SDK , en genymotions si lo tenemos instalado y ejecutando alguna virtual y directamente en el dispositivo si hemos activado el modo desarrollador:

```
$ tns run android
```