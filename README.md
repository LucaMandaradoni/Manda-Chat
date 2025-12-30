# Manda-Chat
Aprendiendo a hacer chat con servers a través de internet!

-------SISTEMA OPERATIVO-------
Este programa corre en Linux, por lo que si queres ejecutarlo en windows se debe instalar WSL para su funcionamiento
ejecuta una terminal de powershell como administrador y escribí:

wsl --install

Una vez finalice la instalación reiniciá la computadora y vas a buscar en el inicio "Ubuntu". Esto abrirá una terminal de Linux.


-------INSTALACIÓN-------
en la terminal de Ubuntu crearas tu usuario y contraseña y luego podras clonar este repositorio con:
git clone https://github.com/LucaMandaradoni/Manda-Chat

una vez termine haz:
cd Manda-Chat
./install.sh

Con esto iniciará la instalación de todas las dependencias del codigo!

-------EJECUCION-------
Una vez finalice estaras listo para lanzar tu server y/o conectarte a uno que lance otra persona. Para ello utilizaras:
./run-client.sh  o  ./run-server.sh 
según sea el caso.

Para lanzar el server necesitaras una herramienta para abrir un "tunel" TCP, es decir, abrir un puerto.
La forma en la que yo lo hice fue con bore, el cual es gratuito y facil de usar.

-------BORE-------
Abre una nueva terminal de Ubuntu e instala Bore con el siguiente comando:
cargo install bore-cli

luego para lanzarlo pon en es terminal:
bore local 9191 --to bore.pub

9191 es el puerto que dejé seteado en el codigo para ser utilizado por el programa.
Una vez lanzado te dará algo como -> bore.pub:12345
esta es la IP (bore.pub) y el PUERTO (12345) que deberan colocar los usuarios que deseen conectarse a tu server para chatear!!!


-------ULTIMOS DETALLES-------
1 - Tiene que haber un server levantado antes de poder conectarse con ./run-client.sh
2 - El programa funciona. Sin embargo, fue hecho con propositos de aprendizaje por lo que es bastante básico y pequeño.
4 - Intentaré actualizarlo para que sea mas user-friendly en el futuro!

Muchas gracias por leer!!!









