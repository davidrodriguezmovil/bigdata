# 🌪️ WSL
Windows Subsystem for Linux (WSL)

## Requisitos previos

Considérase unha máquina con Microsoft Windows 10/11

## Instalación

Require permisos de administrador ou root para instalar por primeira vez o compoñente no sistema.

Abrimos unha consola de PowerShell e escribimos o comando

``` bash
wsl --install
```

Por defecto instalaranos unha máquina de Ubuntu.

Tras a instalación é preciso reiniciar, avísanos coa mensaxe: *La operación solicitada se realizó correctamente. Los cambios se aplicarán una vez que se reinicie el sistema.*

Tras reiniciar, se non nos entra cun simple comando *wsl*, volvemos a unha consola de PowerShell como usuarios e volvemos escribir:

``` bash
wsl --install
```

Se queremos outro sabor de GNU/Linux podemos executar:

``` bash
wsl --list --online
```

E instalar a versión desexada, por exemplo:

``` bash
wsl --install Debian
```

## Entrar no sistema

Abrimos unha consola de PowerShell e executamos

``` bash
wsl
```

Para ver as distribucións instaladas:

``` bash
wsl -l
```

Se temos máis dunha distribución, debemos seleccionar cal queremos executar (ou executará a por defecto). Por exemplo:

``` bash
wsl -d Debian
```

## Actualización de wsl

Abrimos unha consola de PowerShell e escribimos o comando

``` bash
wsl --update
```

## Erros comúns

Se da un erro do tipo: 

~~~~
<3>WSL (10) ERROR: CreateProcessParseCommon:711: Failed to translate X:\
~~~~

Trata de executar os comandos de WSL na unidade por defecto onde está instalado o sistema operativo (habitualmente C:\).
