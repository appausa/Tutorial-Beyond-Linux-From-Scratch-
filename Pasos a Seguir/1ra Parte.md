# Beyond, Linux From Scratch!
**La intalación de Linux Mas allá de Poco a Poco**

Tenemos que crear algunas cosas que demos hacer para comenzar, veremos en tamaño del sources si es que tenemos las carpetas creadas**
```bash
du -sh /sources/  &&
cd sources/BLFS &&
ls -l
```
Los paquetes y parches que se descargaran, deberán almacenarse en un lugar fácilmente accesible durante toda la compilación. También se requiere un directorio de trabajo para descomprimir el código fuente y compilarlo. Este directorio /sources/BLFS/ puede usarse tanto para almacenar los archivos tar y parches como para el directorio de trabajo. Al usar este directorio, los elementos necesarios se ubicarán en la partición de BLFS y estarán disponibles durante todas las etapas del proceso de compilación. Si no existe creelo...
```bash
mkdir -v /sources/BLFS 
```
Establezca este directorio como permanente y con permisos de escritura. "Permanente" significa que, incluso si varios usuarios tienen permisos de escritura en un directorio, solo el propietario de un archivo puede eliminarlo dentro de un directorio permanente. El siguiente comando habilitará los modos de escritura y permanente:
```bash
chmod -v a+wt /sources/BLFS 
```
Nos vamos a la carpeta sources
```bash
cd /sources/BLFS 
```
Para descargar todos los paquetes y parches utilizando wget-list como entrada para el comando wget, utilice:
```bash
wget https://github.com/appausa/Tutorial-Beyond-Linux-From-Scratch-/blob/main/Archivos/wget-list
```
Ahora tomamos el siguiente enlace las descargamos
```bash
wget --input-file=wget-list --continue --directory-prefix=/sources/BLFS 
```
Puede descargar el archivo [wget-list](https://github.com/appausa/Tutorial-Beyond-Linux-From-Scratch-/blob/main/Archivos/wget-list) y desde el disco por ejemplo descarga intalarlas
```bash
cd ~Dounloads/ 
cat wget-list
wget --input-file=wget-list --continue --directory-prefix=/sources/BLFS 
```
# Es el momento de comenzar la intalación

**Wget-1.25.0**

Descomprimimos el primer paquete y accedemos a el
```bash
tar -xjvf wget-1.25.0.tar.gz
cd wget-1.25.0 
```
Preparar wget-1.25.0 para la compilación e intalar
```bash
time { ./configure --prefix=/usr    \
            --sysconfdir=/etc       \
            --with-ssl=openssl && make && make
```
Borramos la carpeta de wget-1.25.0 antes creada
```bash
cd ..
rm -rf wget-1.25.0
```
