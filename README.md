# 🆘 Buscador de Personas — Sismo La Guaira 2026

Aplicación web de emergencia para localizar personas hospitalizadas tras el terremoto.  
Funciona completamente **sin internet**, **sin servidor** y desde **cualquier dispositivo**.

---

## ▶️ Cómo usar la aplicación

1. Abre el archivo **`index.html`** en cualquier navegador (Chrome, Firefox, Safari, Edge).
2. Haz clic en el recuadro "📂 Cargar / Actualizar Lista de Personas".
3. Selecciona el archivo Excel: `Terremoto Venezuela - Consolidado de personas de todos los archivos.xlsx`
4. ¡Listo! Puedes buscar por **cédula, nombre o apellido** al instante.

---

## 🔄 Cómo actualizar la lista de personas

Cuando llegue un nuevo archivo Excel consolidado:

1. Abre la página web en el navegador.
2. Haz clic en el recuadro de carga (o arrastra el nuevo archivo directamente).
3. Selecciona el nuevo `.xlsx`.
4. La lista se actualiza **inmediatamente** — sin tocar código.

> ⚠️ El archivo anterior se reemplaza solo en la sesión actual.  
> Para que otros usuarios vean la actualización, deben repetir el paso 2 en sus dispositivos.

---

## 📱 Acceso en móviles

La aplicación está optimizada para celular. Para compartirla con otras personas:

### Opción A — WhatsApp / Telegram (más rápido)
Envía el archivo `index.html` por WhatsApp o Telegram.  
El receptor lo abre en el navegador de su celular y carga el Excel.

### Opción B — Red local WiFi (recomendado para el refugio)
Si tienes un computador o Raspberry Pi en la misma red:
```
npx serve .
```
Luego comparte la IP local (ej: `http://192.168.1.10:3000`) con todos los equipos de rescate.

### Opción C — GitHub Pages / Netlify Drop (acceso web global)
1. Sube el `index.html` a [netlify.com/drop](https://app.netlify.com/drop)
2. Obtendrás una URL pública (ej: `https://wonderful-example.netlify.app`)
3. Comparte esa URL por WhatsApp a familiares y rescatistas

---

## 🔍 Funciones disponibles

| Función | Descripción |
|---------|-------------|
| 🔍 Búsqueda instantánea | Filtra por nombre, apellido o cédula mientras escribes |
| 🏥 Filtros por hospital | Botones rápidos para ver todos los pacientes de un centro |
| 📋 Tarjeta de detalle | Toca cualquier resultado para ver datos completos |
| 🎨 Código de colores | ✅ Verde = Alta/Mejoría · 🔴 Rojo = Crítico/Fallecido · 🚑 Naranja = Traslado |
| 📱 Mobile-first | Optimizado para usar desde el celular bajo estrés |

---

## 📁 Estructura de archivos

```
registro Maestro de Sismo 2026/
├── index.html                                          ← Aplicación web (este archivo)
├── Terremoto Venezuela - Consolidado de personas...xlsx ← Datos (cargar en la web)
└── README.md                                           ← Este manual
```

---

## ⚙️ Columnas del Excel reconocidas

| Columna | Campo |
|---------|-------|
| A | APELLIDO(S) |
| B | NOMBRE(S) |
| C | CÉDULA/ID |
| D | EDAD |
| E | ¿MENOR? |
| F | SEXO |
| G | HOSPITAL/CENTRO |
| H | ÁREA/ZONA |
| I | PISO/CAMA |
| J | PROCEDENCIA |
| K | DIAGNÓSTICO/SERVICIO |
| L | ESTADO/CONDICIÓN |
| M | FECHA REG. |
| N | HORA |
| O | FAMILIAR |
| P | FUENTE |
| Q | COMENTARIOS |

---

## 🔒 Privacidad

Ningún dato se envía a internet.  
Todo el procesamiento ocurre **localmente en el navegador** del dispositivo.

---

*Sistema de emergencia — Sismo La Guaira 2026*
