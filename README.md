# Configurar Extensión Microsoft Remote - SSH de Visual Studio Code en Microsoft Windows 7 con Autenticación por Clave Pública
Instalar la extensión Remote - SSH de Microsoft para Visual Studio Code nos permite editar archivos presentes en otra computadora directamente a través de SSH.

Esto nos ahora los pasos clásicos:
- Trasladar los archivos de la máquina objetivo a la máquina local
- Modificar los archivos localmente
- Trasladar los archivos modificados a la máquina objetivo

La autenticación por Clave Pública/Privada es recomendada sobre la autenticación por Usuario/Contraseña ya que es más segura y evita el ingreso de la contraseña del usuario en la mayoría de las ocasiones.

En los sistemas operativos Linux y Microsoft Windows 8, 8.1 y 10 es bastante sencilla la instalación de esta extensión y la configuración de autenticación por clave pública/privada.

Para configurar este tipo de autenticación en Microsoft Windows 7 es un poco más difícil y voy a tratar de explicarlo.

## Requisitos
Es necesario instalar el software de control de versiones Git y el editor de código Microsoft Visual Studio Code.

## Pasos
### Paso 1 - Instalar Remote SSH - Microsoft
![Remote SSH - Microsoft Extension para Visual Studio Code](/paso_1_remote_ssh_extension.png "Extension Remote SSH")

### Paso 2 - Configurar la aplicación SSH para la extensión
![Configurar la aplicación SSH](/paso_2_ssh_path.png "Aplicación SSH a utilizar")

### Paso 3 - Generar las claves compatibles (si se tienen claves PuTTY)
Ver [Reusing a key generated in puttygen](https://code.visualstudio.com/docs/remote/troubleshooting#_reusing-a-key-generated-in-puttygen)

### Paso 4 - Configurar el Host Remoto
Se debe configurar el archivo de clave privada para autenticar al usuario
![Configuración de clave privada para el host remoto](/paso_4_configurar_remote_host.png "Configuración de clave privada para el host remoto")

## Referencias
- [Remote development over SSH](https://code.visualstudio.com/docs/remote/ssh-tutorial)
- [Remote Development Tips and Tricks](https://code.visualstudio.com/docs/remote/troubleshooting)

