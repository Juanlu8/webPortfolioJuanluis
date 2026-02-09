# Configuración de Formspree para el Formulario de Contacto

## ⚡ Pasos Rápidos (5 minutos)

### 1. Crear Cuenta en Formspree

1. Ve a: https://formspree.io/register
2. Regístrate con tu email (puedes usar `juanluisbertoncini@gmail.com`)
3. Verifica tu email (revisa tu bandeja de entrada)

### 2. Crear un Nuevo Formulario

1. Una vez logueado, haz clic en **"+ New Form"**
2. Dale un nombre al formulario, por ejemplo: "Portfolio Contact"
3. Como email de destino, pon: `juanluisbertoncini@gmail.com`
4. Haz clic en **"Create Form"**

### 3. Obtener tu Form ID

Después de crear el formulario, verás una URL como:
```
https://formspree.io/f/xyzabc123
```

El **Form ID** es la parte después de `/f/`, por ejemplo: `xyzabc123`

### 4. Configurar tu Código

1. Abre el archivo: `script.js`
2. Busca la línea (aproximadamente línea 551):
   ```javascript
   const response = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
   ```
3. Reemplaza `YOUR_FORM_ID` con tu Form ID real:
   ```javascript
   const response = await fetch('https://formspree.io/f/xyzabc123', {
   ```

### 5. ¡Prueba tu Formulario!

1. Abre `index.html` en tu navegador
2. Rellena el formulario de contacto
3. Haz clic en "Enviar Mensaje"
4. Deberías ver el mensaje: "¡Mensaje enviado correctamente!"
5. Revisa tu email - ¡deberías recibir el mensaje!

## 📊 Plan Gratuito de Formspree

- ✅ 50 envíos por mes (suficiente para un portfolio personal)
- ✅ Sin publicidad
- ✅ Validación de spam incluida
- ✅ Notificaciones por email

## 🔧 Personalización Opcional

En el panel de Formspree puedes configurar:
- **Email de confirmación**: Enviar un email automático a quien te contacta
- **Mensaje de agradecimiento personalizado**
- **Redirección después de enviar** (opcional)
- **Filtros anti-spam**

## 🆘 Solución de Problemas

### "Error al enviar el formulario"
- Verifica que hayas reemplazado `YOUR_FORM_ID` correctamente
- Asegúrate de estar conectado a internet
- Revisa la consola del navegador (F12) para más detalles

### "No me llega el email"
- Revisa tu carpeta de spam
- Verifica que el email en Formspree sea el correcto
- Espera unos minutos (a veces tarda un poco)

### Límite de 50 mensajes alcanzado
- El plan Pro cuesta $10/mes y permite 1000 envíos
- O simplemente espera al próximo mes (se reinicia)

## 🚀 Alternativas (si prefieres otra opción)

### EmailJS
- También gratis (200 emails/mes)
- Más configuración inicial
- Instrucciones en `CONFIGURACION-FORMULARIO.md`

### Netlify Forms
- Requiere alojar tu sitio en Netlify
- 100 envíos/mes gratis
- Muy simple si ya usas Netlify

---

**¿Necesitas ayuda?** Contáctame en juanluisbertoncini@gmail.com
