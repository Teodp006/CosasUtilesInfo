<!--Este README.md está hecho en formato HTML, por si queréis aprender más sobre este lenguaje, también subiré tutoriales-->

<html>
  <body>
  <h1> Menu desplegable de Emojis </h1>
  <h2> Instalando el Paquete necesario</h2>

  <p> Con tan solo hacer <code>Windows + .</code> (desde Linux también) podrás abrir el siguiente panel: </p>
  <img src = "https://github.com/Teodp006/CosasUtilesInfo/blob/main/EmojisUbuntu/PreviewAplicacion.png">
  <p> Donde solo tendrás que seleccionar el emoji, por ejemplo el primero, darle a <code>copiar</code> y pegarlo: 😀</p>

  <p> Lo primero que tenemos que hacer es descargar el paquete <strong> Emoji Picker </strong> de <a href = "https://www.gnome.org/">Gnome</a>. </p>
  <p> Para ello ejecutamos el siguiente comando de terminal: <pre><code> sudo apt install gnome-shell-extension-manager </code></pre></p>

  <p> Ahora deberíamos ver lo siguiente: </p>
  <img src = "https://github.com/Teodp006/CosasUtilesInfo/blob/main/EmojisUbuntu/ResultadoInstalacion.png">
  <p> Tenemos una aplicación caracteres instalada (en mi caso dentro del grupo utilidades). Pero lo que nosotros queremos es poder ejecutar la aplicación
  cada vez que presionemos un cierto comando, puede ser <code>Windows + .</code> o cualquier otra cosa.</p>

  <h2> Creando el comando </h2>

  <p> En primer lugar lo que debemos obtener es la ruta que ejecuta el sistema operativo cada vez que nosotros clicamos al logo de la aplicación, para ello nos dirigiremos a nuestro Gestor de Archivos. Buscaremos en:
    <ul>
      <li> 📁<em>+Otras Ubicaciones</em>, luego en: </li>
        <ul>
          <li> 📁<em>Ubuntu</em>, luego en: </li>
            <ul>
              <li>📁<em>usr</em>, luego en: </li>
              <ul>
                <li> 📁<em>share</em> <br>
                      ⬆️ Aquí deberíamos ver un directorio lleno de archivos 📄<em>.desktop</em>.
                </li>
              </ul>
            </ul>
        </ul>
    </ul>
    Ahora simplemente buscamos gnome en la barra superior y seleccionamos uno que dice <em>org.gnome.Characters.desktop</em> o algo similar. Como podéis ver en pantalla: <br>
    <img src = "https://github.com/Teodp006/CosasUtilesInfo/blob/main/EmojisUbuntu/BuscarAplicacion.png",caption="Hola">
  </p>

  <p>
    Ahora abrimos el archivo anterior y encontramos lo siguiente:
    <img src= "https://github.com/Teodp006/CosasUtilesInfo/blob/main/EmojisUbuntu/MetadatosAplicacion.png">
    De lo que nos interesa la propiedad <code>Exec=/usr/bin/gnome-characters</code>. Esta es la dirrección del archivo que se ejecuta (<em>EXECute</em> en Inglés) cuando hacemos clic a este icóno desde el Escritorio.
    Podemos ver además que la propiedad <code>Icon=org.gnome.Characters</code> indica el icono que se muestra en pantalla.
  </p>


  <h2> Creando el atajo de teclado </h2>
  <p> 
    <ol>
      <li> Copiamos el contenido de la propiedad Exec del archivo anterior. </li>
      <li> Abrimos la aplicación ⚙️Configuración de Ubuntu.</li>
      <li> 🔍Buscamos "atajos" en la barra superior o nos dirijimos a le sección ⌨️Teclado.</li>
      <li> Clicamos en "ver y personalizar atajos" en la sección personalizar atajos.</li>
      <li> Bajamos hasta abajo hasta "Atajo personalizado".</li>
      <li> Clicamos en "Añadir atajo" y rellenamos los datos.</li>
      <li> Le damos a "Establecer atajo" y tecleamos <code>Windows + .</code> (Ubuntu lo entenderá como <code>Super + .</code>) o cualquier cosa que queramos</li>
    </ol>
  </p>

  
  <img src = "https://github.com/Teodp006/CosasUtilesInfo/blob/main/EmojisUbuntu/CreandoAtajo.png" alt="Imagen creando el atajo">
  </body>
</html>
