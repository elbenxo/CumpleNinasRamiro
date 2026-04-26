# Cumple 3er Trimestre - Infantil 3 Años B

Web de invitación para la fiesta de cumpleaños del tercer trimestre (junio, julio, agosto) de la clase Infantil 3 Años B del **CEIP Ramiro de Maeztu** (Madrid).

## Evento

- **Fecha:** Sábado 20 de Junio de 2026
- **Hora:** 11:00 - 13:30 h
- **Lugar:** Kangaroo's Parque Infantil, C/ Eugenio Salazar 45, 28002 Madrid (Chamartín)
- **Precio:** 18,50 € por niño/a, a cargo de cada familia
- **Comida:** Incluida (pizza/hamburguesa/perrito + bebida + tarta + chuches)
- **Confirmar asistencia:** Antes del 13 de junio

## Cumpleañeros

| Niño/a | Padres | Clase |
|--------|--------|-------|
| Andrea | Bea y Andrés | 3 Años B |
| Vera | Rosa y Víctor | 3 Años B |
| Jaime de la Puente | Yvonne y Javier | 3 Años B |
| Nora | Irene y Benxamín | 3 Años B |
| Claudia | Liz y Raúl | 3 Años B |
| Alicia | Ferrán y Amparo | 3 Años B |
| Juan | Cristina y Vicente | 3 Años B |
| Mateo | Dani y Paula | 3 Años C |

## Stack técnico

- **HTML/CSS/JS** puro (single page, sin framework)
- **Tipografía:** Fredoka (display) + Nunito (body) via Google Fonts
- **Hosting:** GitHub Pages desde rama `main`
- **Formulario RSVP:** Envía datos a Google Sheets via Google Apps Script (POST con `mode: no-cors`)
- **Calendario:** Botón que genera archivo `.ics` para añadir el evento al móvil
- **Escudo:** SVG inline del escudo real del CEIP Ramiro de Maeztu (CP/RM)

## Despliegue

- **Rama de desarrollo:** `claude/kindergarten-birthday-website-hhnWn`
- **Rama de producción:** `main` (GitHub Pages)
- **URL:** https://elbenxo.github.io/CumpleNinasRamiro/

Cada push a `main` se despliega automáticamente en GitHub Pages (1-2 min).

## Google Sheets (RSVP)

El formulario envía las respuestas a una hoja de Google Sheets mediante un Google Apps Script publicado como web app. La URL del script está configurada en la variable `SCRIPT_URL` en el archivo `index.html`.

Campos recogidos: nombre del niño/a, hermanos (sí/no + cantidad), alergias, comentarios.

## Historial de cambios

1. Creación inicial de la web con datos del evento y cumpleañeros
2. Corrección de horario (11:00 - 13:30) y simplificación de tarjetas de cumpleañeros (sin fechas de cumple)
3. Reemplazo del escudo SVG por el escudo real del CEIP Ramiro de Maeztu
4. Rediseño completo con directrices frontend-design (Fredoka/Nunito, paleta coral/teal/sunshine/lavender, animaciones scroll, sprinkle confetti, tarjetas rotadas)
5. Añadido Mateo (Dani y Paula, Infantil 3 Años C) como cumpleañero
6. Formulario RSVP integrado con Google Sheets via Apps Script
7. Ajustes de redacción del precio (feedback de Iren): "Como en los cumples trimestrales anteriores, el precio de las entradas corre a cargo de cada familia. Son 18,50 € por niño/a."
8. Botón de añadir evento al calendario (.ics) con recordatorio 1 día antes
9. Fix de error JS por comillas escapadas en la función del calendario
10. Indicación de que Mateo es de Infantil 3 Años C
