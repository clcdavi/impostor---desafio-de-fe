# Impostor - Desafío de Fe 🙏

Una aplicación web minimalista y responsiva para jugar **Impostor** con temática cristiana. Perfecta para grupos pequeños y medianos de comunidades de fe como la Juventud Roca Fuerte (JRF).

## ¿Cómo Jugar?

### Configuración Inicial
1. Selecciona el número de **jugadores** (2-12)
2. Elige cuántos **impostores** habrá (mínimo 1, máximo jugadores-1)
3. Personaliza los **nombres** de cada participante
4. ¡Presiona **Iniciar Juego**!

### Durante el Juego
1. **Cada jugador** recibe su turno para revelar su pista
2. **Mantén presionado** la pantalla para ver:
   - Una **palabra pista** (aceite, cruz, pan, etc.) si eres Discípulo
   - O la palabra **"IMPOSTOR"** si fuiste seleccionado
3. **Suelta** para volver a ocultar
4. ¡Presiona **Siguiente** cuando el jugador haya visto su pista!

### ¿Quién Habla Primero?
- Se elige **aleatoriamente** quién comienza a dar referencias
- Todos los **Discípulos ven la MISMA palabra pista**
- Los **Impostores no conocen el tema** 🕵️

### Revelación Final
- Se muestran todos los jugadores **sin revelar inicialmente** sus roles
- **Presiona "Revelar Impostores"** para descubrir quién era el impostor
- Opción para **jugar de nuevo** 🎮

---

## Características

✨ **Diseño Minimalista & Responsivo**
- Compatible con móviles, tablets y desktop
- Tema cristianamente inspirado (colores tierra, verde oliva, azul cielo, dorado)
- Fuentes elegantes (Poppins, DM Sans)

🎮 **Funcionalidad Completa**
- Selección aleatoria de impostores
- 20 palabras pista temáticas (aceite, cruz, manto, corona, pan, vino, etc.)
- Todos los Discípulos ven la MISMA pista en la ronda
- Selección aleatoria de quién habla primero
- Revelación de impostores con botón especial
- Reveal/Hide con touch y mouse
- Modo oscuro disponible
- Persistencia de tema en navegador

📱 **Experiencia Móvil Optimizada**
- Touch eventos (touchstart/touchend)
- Mouse eventos para testing en desktop
- Prevención de selección de texto
- Animaciones suaves

---

## Desplegar en GitHub Pages

### Opción 1: Crear un nuevo repositorio (Recomendado)

1. **Crea un repositorio** en GitHub:
   ```bash
   # En tu cuenta de GitHub, clickea "+" > "New repository"
   ```

2. **Clona el repositorio** localmente:
   ```bash
   git clone https://github.com/TU_USUARIO/impostor.git
   cd impostor
   ```

3. **Copia el archivo** `index.html` al repositorio

4. **Sube los cambios**:
   ```bash
   git add index.html README.md
   git commit -m "Initial commit: Impostor game"
   git push origin main
   ```

5. **Activa GitHub Pages**:
   - Ve a Settings → Pages
   - Source: `main` branch
   - Folder: `/ (root)`
   - Save

6. **Accede a tu juego**:
   ```
   https://TU_USUARIO.github.io/impostor/
   ```

### Opción 2: Usar GitHub Pages con tu sitio personal

Si ya tienes `TU_USUARIO.github.io`:

1. **Copia `index.html`** a una carpeta dentro de tu sitio:
   ```bash
   cp index.html ~/TU_USUARIO.github.io/impostor/index.html
   ```

2. **Accede en**:
   ```
   https://TU_USUARIO.github.io/impostor/
   ```

### Opción 3: Usar una rama específica (gh-pages)

```bash
git checkout --orphan gh-pages
git add index.html
git commit -m "Deploy: Impostor game"
git push origin gh-pages
```

Luego en Settings → Pages → Source selecciona `gh-pages` branch.

---

## Estructura del Proyecto

```
impostor/
├── index.html          # Aplicación completa (HTML + CSS + JS)
└── README.md          # Este archivo
```

## Personalización

### Agregar o cambiar palabras pista

Edita el array `biblicalCharacters` en `index.html`:

```javascript
const biblicalCharacters = [
    'aceite', 'cruz', 'manto', 'corona', 'sandalia',
    // Agrega tus propias palabras aquí:
    'tu palabra', 'otra palabra'
];
```

### Cambiar colores

Las variables CSS están en la sección `<style>`:

```css
:root {
    --color-primary: #8B7355;      /* Marrón tierra */
    --color-secondary: #6B8E23;    /* Verde oliva */
    --color-accent: #4A90E2;       /* Azul cielo */
    --color-gold: #D4AF37;         /* Dorado */
}
```

### Cambiar fuentes

Modifica la línea de Google Fonts en el `<head>` o añade tus propias fuentes.

---

## Requisitos Técnicos

- ✅ HTML5 + CSS3 + JavaScript vanilla
- ✅ Sin dependencias externas
- ✅ Compatible con navegadores modernos
- ✅ Funciona sin conexión (después de cargar)

## Navegadores Soportados

- Chrome/Chromium 60+
- Firefox 55+
- Safari 12+
- Edge 79+
- Mobile browsers (iOS Safari, Chrome Android)

---

## Tips para Jugar

🎯 **Juego Estratégico**
- Los impostores no saben cuál es la pista (solo ven "IMPOSTOR")
- Los discípulos TODOS ven la misma palabra pista
- Deben detectar quién está dando referencias falsas
- ¡Descubre quién miente! 🕵️

👥 **Mejor Experiencia**
- Usa en grupo de 4-8 personas
- Asegúrate de que todos vean la pantalla correctamente
- Mantén la presión de forma natural (no muy fuerte)

🎮 **Variaciones**
- Aumenta impostores para más desafío
- Cambia las pistas por temas semanales
- Lleva score entre rondas

---

## Licencia

Libre para usar y modificar. ¡Que disfrutes con tu comunidad! 🙏

---

## Créditos

Creado con ❤️ para **Juventud Roca Fuerte (JRF)**

---

## Contacto & Feedback

¿Problemas o sugerencias? Siéntete libre de:
- Crear un issue en el repositorio
- Hacer fork y contribuir mejoras
- Compartir tu experiencia jugando

¡Que Dios te bendiga! 🙌
