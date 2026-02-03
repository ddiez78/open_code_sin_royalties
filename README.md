# Música para Cuentos

Generador de música instrumental calmada con base de piano, diseñada específicamente para cuentos infantiles.

## Características

- 🎹 Piano sintetizado con sonido suave y relajante
- ⏱️ Duración configurable: 2, 2.5 o 3 minutos
- 🎚️ Intensidad ajustable (suave/rico)
- ⬇️ Descarga en formato WAV
- 🌐 Aplicación web (HTML + JavaScript)
- 🔇 Sin dependencias de servidor

## Uso

1. Abre el archivo `index.html` en tu navegador (Chrome, Firefox, Edge, Safari)
2. Selecciona la duración deseada (2, 2.5 o 3 minutos)
3. Ajusta la intensidad del piano si lo deseas
4. Clic en "Generar Música"
5. Espera a que termine la reproducción
6. Reproduce o descarga el archivo WAV

## Instalación Local

Simplemente abre el archivo `index.html` directamente en tu navegador:

```bash
# En Windows
start index.html

# En macOS
open index.html

# En Linux
xdg-open index.html
```

## Despliegue Web

### GitHub Pages (Gratis)

1. Crea un repositorio en GitHub
2. Sube el archivo `index.html`
3. Ve a Settings > Pages
4. Selecciona la rama main y guarda
5. Tu app estará disponible en `https://tuusuario.github.io/repo/`

### Vercel (Gratis)

1. Ve a [vercel.com](https://vercel.com)
2. Arrastra el archivo `index.html` a la página
3. Tu app estará disponible instantáneamente

### Netlify (Gratis)

1. Ve a [netlify.com](https://netlify.com)
2. Arrastra el archivo `index.html`
3. Tu app estará disponible inmediatamente

## Licencia

**Creative Commons Zero (CC0) - Dominio Público**

Esta obra está dedicada al dominio público. Puedes copiar, modificar, distribuir y ejecutar la obra, incluso con propósitos comerciales, sin necesidad de permiso previo.

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

## Información Técnica

- **Motor de audio**: Tone.js + Web Audio API
- **Formato de salida**: WAV (PCM 16-bit)
- **Tempo**: 65 BPM (lento, relajante)
- **Escala**: C Major
- **Progresión armónica**: C → Am → F → G
- **Licencia del código**: MIT
- **Licencia de la música generada**: CC0

## Requisitos

- Navegador moderno con soporte para Web Audio API
- Conexión a internet para cargar Tone.js (CDN)
- Altavoces o auriculares

## Personalización

### Cambiar el tempo

Busca en el código JavaScript:
```javascript
const bpm = 65; // Cambia este valor
```

### Cambiar la escala musical

Busca y modifica:
```javascript
const scale = ['C4', 'D4', 'E4', 'F4', 'G4', 'A4', 'B4', 'C5', 'D5', 'E5'];
```

### Añadir más reverb

```javascript
const reverb = new Tone.Reverb({
    decay: 5,  // Más tiempo de reverb
    wet: 0.5   // Más intensidad
}).toDestination();
```

## Contribuciones

Las contribuciones son bienvenidas. Siéntete libre de forkear el proyecto y mejorarlo.

## Créditos

- Built with [Tone.js](https://tonejs.github.io/)
- Inspirado en música para cuentos infantiles clásicos
