# Ó CÓMO AGREGAR UN CHATBOT IA A TU PÁGINA SEPROSAT GPS

## Guía Paso a Paso

Tu página de Seprosat GPS ya está **ONLINE** en:
**`https://tovaryasmil-sys.github.io/seprosat-gps/`**

---

## Ð PASO 1: Elegir un Proveedor de Chatbot IA

Existen varias opciones gratuitas y de pago:

### Opciones Recomendadas:

1. **Botpress** (Gratuito + Premium)
   - URL: https://botpress.com
   - Ideal para chatbots inteligentes
   - Ofrece un script de incrustación listo para usar

2. **Rasa** (Gratuito y Open Source)
   - URL: https://rasa.com
   - Para chatbots más avanzados
   - Requiere más configuración

3. **Tidio** (Gratuito hasta 1,000 chats/mes)
   - URL: https://www.tidio.com
   - Fácil de usar
   - Perfecto para comenzar

4. **Drift** (Prueba gratuita)
   - URL: https://www.drift.com
   - Muy profesional
   - Ideal para soporte al cliente

5. **Chatbase** (Gratuito con limitaciones)
   - URL: https://www.chatbase.co
   - Construido con IA moderna
   - Fácil integración

---

## Ð PASO 2: Registrarte en el Servicio de Chatbot

1. Elige uno de los servicios anteriores
2. Haz clic en "Sign Up" o "Empezar Gratis"
3. Completa tu información (Email, contraseña, nombre)
4. Verifica tu correo electrónico

---

## Ð PASO 3: Obtener el Código del Widget

Cada servicio tiene un panel de control. Busca la opción:
- "Get Code"
- "Embed Widget"
- "Incrustación"
- "Integration"

Copiarás un código similar a este:

```html
<script>
  (function (w, d, s, o, f, js, fjs) {
    w[o] = w[o] || function () { (w[o].q = w[o].q || []).push(arguments) };
    js = d.createElement(s); fjs = d.getElementsByTagName(s)[0];
    js.id = o; js.src = f; js.async = 1; fjs.parentNode.insertBefore(js, fjs);
  })(window, document, 'script', 'Chatbase', 'https://www.chatbase.co/embed.min.js');
  
  Chatbase.init({
    chatbotId: 'YOUR-BOT-ID'
  });
</script>
```

---

## Ð PASO 4: Añadir el Código a tu Página

### Opción A: Edición Rápida en GitHub

1. Ve a tu repositorio: https://github.com/tovaryasmil-sys/seprosat-gps
2. Haz clic en el archivo **`index.html`**
3. Haz clic en el lápiz (Edit)
4. Busca la línea que dice: `<!-- AQUÍ VA EL CÓDIGO DEL CHATBOT IA -->`
5. Reemplaza el comentario con tu script del chatbot
6. Haz clic en "Commit changes"
7. ¡Listo! Tu chatbot aparecerá en 1-3 minutos

### OpciÓn B: Edición Avanzada (Local)

1. Descarga el archivo `index.html` desde GitHub
2. Ábrelo en un editor de texto (Notepad++, VS Code, Sublime)
3. Busca el final del archivo, antes de `</body>`
4. Pega el script de tu chatbot
5. Guarda el archivo
6. Sube el archivo actualizado a GitHub

---

## Ð EJEMPLO: Código Completo Modificado

```html
<!-- ... resto del código ... -->
    </footer>
    
    <script>
        function handleSubmit(event) {
            event.preventDefault();
            const name = document.getElementById('name').value;
            alert('¡Gracias ' + name + '! Tu mensaje ha sido recibido.');
            document.querySelector('form').reset();
        }
    </script>
    
    <!-- TU CHATBOT IA AQUI -->
    <!-- Ejemplo con Chatbase -->
    <script>
      (function (w, d, s, o, f, js, fjs) {
        w[o] = w[o] || function () { (w[o].q = w[o].q || []).push(arguments) };
        js = d.createElement(s); fjs = d.getElementsByTagName(s)[0];
        js.id = o; js.src = f; js.async = 1; fjs.parentNode.insertBefore(js, fjs);
      })(window, document, 'script', 'Chatbase', 'https://www.chatbase.co/embed.min.js');
      
      Chatbase.init({
        chatbotId: 'TU-ID-DE-BOT-AQUI'
      });
    </script>
    
</body>
</html>
```

---

## Ð PASO 5: Probar tu Chatbot

1. Espera 2-3 minutos a que GitHub Pages reconstruya el sitio
2. Ve a: https://tovaryasmil-sys.github.io/seprosat-gps/
3. Deberías ver el chatbot en la esquina inferior derecha
4. Haz clic y prueba una converación

---

## Ð CONSEJOS Y TRUCOS

### Personalizar el Chatbot

- **Nombre del Bot**: Cambia en el panel del proveedor (ej: "Seprosat Bot")
- **Mensaje Inicial**: Configura el primer mensaje que aparece
- **Colores**: Personaliza para que coincidan con tu marca (púrpura y blanco)
- **Respuestas**: Entrena el bot con preguntas frecuentes sobre GPS

### Preguntas Frecuentes para Entrenar

1. "¿Qué es Seprosat GPS?"
   - Respuesta: "Seprosat GPS ofrece soluciones avanzadas de localización en tiempo real..."

2. "¿Cuál es el precio?"
   - Respuesta: "Contáctanos para una demostración personalizada..."

3. "¿Cómo funciona?"
   - Respuesta: "Nuestro sistema utiliza tecnología GPS de última generación..."

### Problemas Comunes

#### El chatbot no aparece
- Espera 3-5 minutos a que GitHub Pages se reconstruya
- Recarga la página con Ctrl+F5
- Verifica que el ID del bot sea correcto

#### El chatbot se ve feo
- Aj usta el CSS en el archivo de configuración del proveedor
- Algunos proveedores permiten CSS personalizado

#### El chatbot no responde
- Verifica que el bot esté "activo" en tu panel
- Asegúrate de haber entrenado el bot con respuestas

---

## Ð ALTERNATIVA: Más Pasos Avanzados

Si quieres mayor control, puedes crear un bot personalizado en Replit:

1. Ve a: https://replit.com
2. Crea un proyecto Python + Flask
3. Integra una API de IA (OpenAI, Hugging Face)
4. Despliega en Replit
5. Conecta a tu página GitHub Pages

---

## Ð RESUMEN FINAL

✅ **Tu página está ONLINE**  
✅ **Tienes un formulario de contacto funcional**  
✅ **Ahora agrega un chatbot IA en 5 pasos**  
✅ **Personaliza y optimiza**  
✅ **¡Listo para atraer clientes!**

---

## Contacto y Soporte

Si necesitas ayuda:
1. Revisa la documentación del proveedor de chatbot
2. Consulta los tutoriales en YouTube
3. Contacta al equipo de soporte de tu proveedor

**¡Mucho éxito con tu página de Seprosat GPS!**
