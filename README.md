#U - DETECT FRIDA

## Comenzando 🚀

Estas instrucciones te permitirán obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas.

Mira **Deployment** para conocer como desplegar el proyecto.

Que hace este proyecto?

- Detectar a través de canalizaciones con nombre utilizadas por Frida
- Detectar a través de un hilo con nombre específico de frida
- Compare la sección de texto en la memoria con la sección de texto en el disco tanto para libc como para la biblioteca nativa

Además, este proyecto tiene 3 mecanismos para endurecer el código nativo.

1.  Reemplazar ciertas llamadas libc con syscalls
2.  Reemplazar cadena, operación relacionada con la memoria con implementación personalizada
3.  Aplicar la ofuscación nativa de O-LLVM

### Pre-requisitos 📋

Android Studio

## Despliegue 📦

1. Clonar Repositorio
2. Copiar carpeta app/src/main/c en su proyecto Android.
3. Agregar en app/build.gradle llamados a Librerias Nativas Cmake

´
cmake {
path "src/main/c/CMakeLists.txt"
version "3.10.2"
}
´

4. Compile Aplicación en Android y Acepte nuevos componentes.

## Contribute

Elias Manriquez <eamanriquez@gmail.com>

## Autores

https://github.com/darvincisec/DetectFrida

## Licencia 📄

Este proyecto está bajo la Licencia (CC) - mira el archivo [LICENSE.md](LICENSE.md) para detalles
