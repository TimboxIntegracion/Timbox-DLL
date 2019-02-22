# Timbox DLL 
TimboxLibrary.dll ha sido hecha en C#, con el motivo de facilitar la integración en diferentes
lenguajes.

## Características
**Framework**: .NET V4.0.30319

## Lenguajes Soportados
* C#
* Visual Basic
* Visual FoxPro 9.0 
* Delphi

## Archivos
**URL**: https://bitbucket.org/timboxmx/timbox-dll/src/master/TimboxLibrary/bin/Debug/

**Archivos**:

* TimboxLibrary.dll
* TimboxLibrary.pdb
* TimboxLibrary.tlb

## Requisitos
* [.NET Framework 4.0 ](https://www.microsoft.com/en-us/download/details.aspx?id=17851a)
* [Microsoft Visual Studio](https://visualstudio.microsoft.com/es/)
* [Visual Foxpro 9 ](https://docs.microsoft.com/en-us/previous-versions/visualstudio/foxpro/mt490121(v%3dmsdn.10))
* [RAD  Studio](https://www.embarcadero.com/products/rad-studio)

## Instalación

### Windows  
Puede ser registrada la DLL (TimboxLibrary.dll) en system32. 

1-. Abrir el procesador de comandos de Windows (**cmd**) como "Administrador".

2-. Ejecutar los siguientes comandos:

* gacutil -i +  Location\TimboxLibrary.dll

 **Ejemplo**:
```
 C:\Windows\system32> gacutil -i C:\Users\Current User\Your Project\TimboxLibrary.dll
```

* regasm /codebase +  Ubicacion\TimboxLibrary.dll

**Ejemplo**:
```
C:\Windows\system32> regasm /codebase C:\Users\Current User\Your Project\TimboxLibrary.dll
```

* regasm /tlb +  Ubicacion\TimboxLibrary.dll

**Ejemplo**:
```
C:\Windows\system32> regasm /tlb C:\Users\Current User\Your Project\TimboxLibrary.dll
```

### RAD Studio
En el caso de RAD Studio tendrá que agregarse como un nuevo componente de la siguiente manera:

1-. Seleccionar en el menu la opcion **Component** > **Import Component**.

2-. Seleccionar **Import a TypeLibrary**.

3-. Seleccionar el boton **Add** y agregar el archivo **Timboxlibrary.tlb**

4-. En Palette Page: selecciona la opción  **ActiveX** y en Unit Dir Name seleccionar la ruta en la cual será guardado el archivo con 
las extensión **.pas**.

5-. Por ultimo seleccionamos la opción **Create Unit**  y damos clic en el boton **finish**.

**Nota**: Una vez generado un archivo con extensión **.pass**, este archivo deberá ser agregado a nuestro proyecto.

## Integración
A continuación, se muestra los enlaces de integración para C#, Visual Basic, Visual FoxPro 9.0 y Delphi.
 
* [C#](https://github.com/TimboxIntegracion/TimboxDLLCSharp)
* [Visual Basic](https://github.com/TimboxIntegracion/TimboxDLLVB)
* [Visual FoxPro 9.0](https://github.com/TimboxIntegracion/TimboxDLLVpf)
* [Delphi](https://github.com/TimboxIntegracion/TimboxDLLDelphi)