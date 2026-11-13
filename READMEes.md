<p align="center">
    <a href="https://github.com/cheat-engine/cheat-engine/raw/master/Cheat%20Engine/images">
        <img src="https://github.com/cheat-engine/cheat-engine/raw/master/Cheat%20Engine/images/celogo.png" />
    </a>
</p>

<h1 align="center">Cheat Engine</h1>

Cheat Engine es un entorno de desarrollo centrado en la modificación de juegos y aplicaciones para uso personal.


# Descarga

  * **[Última versión](https://github.com/cheat-engine/cheat-engine/releases/latest)**

[Versiones anteriores](https://github.com/cheat-engine/cheat-engine/releases)


# Enlaces

  * [Sitio web](https://www.cheatengine.org)
  * [Foro](https://forum.cheatengine.org)
  * [Foro (alternativo)](https://opencheattables.com/)
  * [Foro (alternativo)](https://fearlessrevolution.com/index.php)
  * [Wiki](https://wiki.cheatengine.org/index.php?title=Main_Page)

## Redes sociales

  * [Reddit](https://reddit.com/r/cheatengine)
  * [Twitter](https://twitter.com/_cheatengine)

## Donaciones

  * [Patreon](https://www.patreon.com/cheatengine)
  * [PayPal](https://www.paypal.com/xclick/business=dark_byte%40hotmail.com&no_note=1&tax=0&lc=US)


## Instrucciones básicas de compilación

  1. Descarga Lazarus 2.2.2 desde https://sourceforge.net/projects/lazarus/files/Lazarus%20Windows%2064%20bits/Lazarus%202.2.2/ Instala primero `lazarus-2.2.2-fpc-3.2.2-win64.exe` y luego `lazarus-2.2.2-fpc-3.2.2-cross-i386-win32-win64.exe`.
  
  2. Ejecuta Lazarus y haz clic en `Project->Open Project`. Selecciona `cheatengine.lpi` dentro de la carpeta `Cheat Engine` como el proyecto.
  3. Haz clic en `Run->Build` o presiona <kbd>SHIFT+F9</kbd>.
      * También puedes hacer clic en `Run->Compile many Modes` (consejo: selecciona los tres primeros modos de compilación).
      * Si deseas ejecutar o depurar desde el IDE en Windows, deberás ejecutar Lazarus como administrador.
      
  No olvides compilar los proyectos secundarios que desees utilizar:
  
     speedhack.lpr: Compila las DLL de 32 y 64 bits para habilitar la funcionalidad de speedhack
     luaclient.lpr: Compila las DLL de 32 y 64 bits para habilitar la funcionalidad de {$luacode}
     DirectXMess.sln: Compila para 32 y 64 bits para habilitar el D3D overlay y las capacidades de snapshot
     DotNetcompiler.sln: Para el comando Lua cscompile
     monodatacollector.sln: Compila las DLL de 32 y 64 bits para obtener las funciones de Mono que permiten inspeccionar el entorno .NET del proceso
     dotnetdatacollector.sln: Compila los EXE de 32 y 64 bits para obtener símbolos .NET
     dotnetinvasivedatacollector.sln: Compila esta .DLL administrada (managed) para agregar soporte de runtime JIT
     cejvmti.sln: Compila las DLL de 32 y 64 bits para habilitar el soporte de inspección de Java
     tcclib.sln: Compila 32-32, 64-32 y 64-64 para agregar soporte de {$C} y {$CCODE} en scripts
     vehdebug.lpr: Compila las DLL de 32 y 64 bits para agregar soporte de la interfaz del VEH debugger
     dbkkernel.sln: Para funciones en kernelmode (settings->extra). Deberás compilar la versión no-sig y arrancar con soporte para drivers sin firma, o bien firmar el driver tú mismo
    
Los archivos *.SLN requieren Visual Studio (generalmente 2017).

## Contribuye al proyecto

Si deseas contribuir:
  1. Haz un fork del repositorio en GitHub.
  2. Crea una rama para tus cambios.
      * A Lazarus le gusta modificar archivos automáticamente cuando los abres o mueves algo, así que asegúrate de incluir únicamente los cambios necesarios para lo que intentas implementar.
  3. Sube tu rama a tu fork personal.
  4. Ve al repositorio original de Cheat Engine y crea un Pull Request.
      * Haz clic en `compare across forks` y selecciona tu fork junto con tu nueva rama.
