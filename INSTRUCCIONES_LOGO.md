# 📋 Instrucciones para Reemplazar el Logo de TRIAX

## 🎯 Ubicaciones del Logo Placeholder

El logo placeholder aparece en dos lugares:

### 1. Header (Navegación Superior)
**Archivo**: `index.html`  
**Líneas**: 17-19

```html
<div class="logo">
    <div class="logo-placeholder">LOGO TRIAX</div>
</div>
```

### 2. Footer (Pie de Página)
**Archivo**: `index.html`  
**Líneas**: 439-441

```html
<div class="footer-logo">
    <div class="logo-placeholder">LOGO TRIAX</div>
</div>
```

---

## 🔧 Cómo Reemplazar el Logo

### Opción 1: Logo como Imagen (Recomendado)

1. **Guardar el logo oficial**
   - Formato recomendado: PNG con fondo transparente o SVG
   - Nombre sugerido: `logo-triax.png` o `logo-triax.svg`
   - Ubicación: carpeta `assets/`

2. **Reemplazar en el Header**
   ```html
   <div class="logo">
       <img src="assets/logo-triax.png" alt="TRIAX" class="logo-image">
   </div>
   ```

3. **Reemplazar en el Footer**
   ```html
   <div class="footer-logo">
       <img src="assets/logo-triax.png" alt="TRIAX" class="footer-logo-image">
   </div>
   ```

4. **Agregar estilos CSS** (en `styles.css`)
   ```css
   .logo-image {
       height: 45px;
       width: auto;
       transition: var(--transition);
   }
   
   .logo-image:hover {
       transform: scale(1.05);
       filter: brightness(1.1);
   }
   
   .footer-logo-image {
       height: 60px;
       width: auto;
       margin-bottom: var(--spacing-sm);
   }
   ```

### Opción 2: Logo como SVG Inline

Si tienes el código SVG del logo, puedes insertarlo directamente:

```html
<div class="logo">
    <svg class="logo-svg" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
        <!-- Código SVG del logo aquí -->
    </svg>
</div>
```

Con estos estilos:
```css
.logo-svg {
    height: 45px;
    width: auto;
    fill: var(--primary);
    transition: var(--transition);
}

.logo-svg:hover {
    fill: var(--accent-green);
    transform: scale(1.05);
}
```

---

## 🎨 Especificaciones de Diseño

### Dimensiones Recomendadas
- **Header**: Alto máximo 45px, ancho proporcional
- **Footer**: Alto máximo 60px, ancho proporcional

### Colores del Logo
Asegúrate de que el logo use los colores oficiales de TRIAX:
- Verde petróleo: `#17403C`
- Verde oliva: `#5C6A35`
- Beige: `#F2F2F0`

### Formato
- **PNG**: Fondo transparente, resolución mínima 300x300px
- **SVG**: Preferible para mejor calidad en todas las resoluciones

---

## ✅ Checklist de Implementación

- [ ] Logo guardado en carpeta `assets/`
- [ ] Código HTML actualizado en header
- [ ] Código HTML actualizado en footer
- [ ] Estilos CSS agregados
- [ ] Logo se ve correctamente en desktop
- [ ] Logo se ve correctamente en móvil
- [ ] Hover effect funciona correctamente
- [ ] Logo mantiene proporciones correctas

---

## 🆘 Soporte

Si necesitas ayuda con la implementación del logo, contacta al desarrollador o revisa la documentación en `README.md`.

**Nota**: El placeholder actual está diseñado para ser fácilmente reemplazable sin afectar el resto del diseño.
