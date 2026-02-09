# Configuración del Formulario de Contacto

Tu portfolio ahora incluye un formulario de contacto funcional. Para que funcione completamente, necesitas configurar el servicio de envío de emails.

## 🚀 Opción 1: Formspree (Recomendado - GRATIS)

**Ventajas:**
- ✅ Completamente gratuito hasta 50 envíos/mes
- ✅ Sin necesidad de backend
- ✅ Configuración en 2 minutos
- ✅ Protección anti-spam incluida

### Pasos para configurar:

1. **Regístrate en Formspree:**
   - Ve a https://formspree.io
   - Crea una cuenta gratuita con tu email

2. **Crea un nuevo formulario:**
   - Click en "New Form"
   - Copia el Form ID que te dan (algo como `xpzgkwqr`)

3. **Actualiza el código:**
   - Abre `script.js`
   - Busca la línea 544:
     ```javascript
     const response = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
     ```
   - Reemplaza `YOUR_FORM_ID` con tu Form ID:
     ```javascript
     const response = await fetch('https://formspree.io/f/xpzgkwqr', {
     ```

4. **¡Listo!** 
   - Los mensajes llegarán directamente a tu email
   - Puedes ver todos los mensajes en el dashboard de Formspree

---

## 📧 Opción 2: EmailJS (Alternativa)

**Ventajas:**
- ✅ 200 emails gratis/mes
- ✅ Múltiples servicios de email (Gmail, Outlook, etc.)
- ✅ Templates personalizables

### Pasos para configurar:

1. **Regístrate en EmailJS:**
   - Ve a https://www.emailjs.com
   - Crea una cuenta gratuita

2. **Conecta tu email:**
   - Ve a "Email Services"
   - Conecta tu Gmail/Outlook/otro servicio

3. **Crea un template de email:**
   - Ve a "Email Templates"
   - Crea un nuevo template con estas variables:
     - `{{name}}` - Nombre del remitente
     - `{{email}}` - Email del remitente
     - `{{subject}}` - Asunto
     - `{{message}}` - Mensaje

4. **Obtén tus credenciales:**
   - User ID (en Account)
   - Service ID
   - Template ID

5. **Actualiza el código en script.js:**
   
   Reemplaza el código de Formspree (líneas 541-551) por:
   
   ```javascript
   // Inicializa EmailJS (ponlo al inicio del archivo, después de las primeras líneas)
   emailjs.init('TU_USER_ID');
   
   // En el submit del formulario:
   const response = await emailjs.send(
       'TU_SERVICE_ID',
       'TU_TEMPLATE_ID',
       {
           name: data.name,
           email: data.email,
           subject: data.subject,
           message: data.message
       }
   );
   ```

6. **Agrega el script de EmailJS en index.html:**
   
   Antes del cierre de `</body>`:
   ```html
   <script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
   <script src="script.js"></script>
   ```

---

## 🌐 Opción 3: Netlify Forms (Si despliegas en Netlify)

Si vas a desplegar tu portfolio en Netlify, es aún más simple:

1. **Agrega el atributo a tu formulario en index.html:**
   
   Cambia:
   ```html
   <form id="contactForm" class="contact-form">
   ```
   
   Por:
   ```html
   <form id="contactForm" class="contact-form" name="contact" netlify>
   ```

2. **Elimina el JavaScript del envío:**
   - Netlify manejará automáticamente el envío
   - Los mensajes aparecerán en tu dashboard de Netlify

---

## ✅ Probando el Formulario

Después de configurar cualquiera de las opciones:

1. Abre tu portfolio en el navegador
2. Ve a la sección de contacto
3. Completa el formulario
4. Haz clic en "Enviar Mensaje"
5. Deberías ver el mensaje de éxito
6. Verifica tu email o dashboard del servicio

---

## 🛠️ Solución de Problemas

### "Error al enviar el mensaje"
- Verifica que hayas reemplazado `YOUR_FORM_ID` correctamente
- Revisa la consola del navegador (F12) para ver el error específico
- Asegúrate de tener conexión a internet

### Los emails no llegan
- Revisa tu carpeta de spam
- Verifica que el email en tu cuenta de Formspree/EmailJS esté correcto
- Comprueba el dashboard del servicio para ver si el mensaje fue recibido

### El botón se queda en "Enviando..."
- Revisa la consola del navegador para ver el error
- Verifica que la URL del servicio esté correcta
- Comprueba que no haya errores de CORS

---

## 📝 Notas

- **Plan Gratuito de Formspree:** 50 submissions/mes
- **Plan Gratuito de EmailJS:** 200 emails/mes
- **Netlify Forms:** 100 submissions/mes (gratis)

Para la mayoría de portfolios personales, estos límites son más que suficientes.

---

¿Necesitas ayuda? Revisa la documentación oficial:
- Formspree: https://help.formspree.io
- EmailJS: https://www.emailjs.com/docs
- Netlify Forms: https://docs.netlify.com/forms/setup
