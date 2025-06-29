# ⚔️ Skin.club Battle Tracker 💰

## ✨ Características

Este script de Tampermonkey te proporciona un tracker en tiempo real directamente en la interfaz de Skin.club, ofreciendo las siguientes funcionalidades:

-   **📊 Seguimiento de Ganancias/Pérdidas**: Muestra tu total actual y el de tus oponentes (o equipo) en tiempo real.
-   **🤝 Detección Automática de Modos**:
    -   **Modo Clásico**: Rastrea tu progreso contra oponentes individuales.
    -   **Modo Equipo**: Calcula el total de tu equipo (tú + compañero) contra el equipo enemigo.
    -   **Modo Compartido (Sharing)**: Muestra el total acumulado de la batalla y tu parte proporcional.
-   **👁️ Modo Observador**: Si no estás participando en la batalla (es decir, tu nombre de usuario no se encuentra en ningún slot), el tracker se adapta para mostrar las estadísticas de los jugadores que están batallando, indicando quién va ganando y el total acumulado de la batalla.
-   **✅ Indicadores de Detección**: Pequeños iconos (✅/❌) en el tracker te informan si el script ha detectado correctamente el modo de juego, tu slot y la información del equipo.
-   **🔄 Robustez y Reintentos**: Implementa un sistema de reintentos con backoff exponencial para asegurar que las detecciones funcionen incluso si la página tarda en cargar o si hay cambios dinámicos en el DOM.
-   **🗑️ Botón de Reset**: Un botón conveniente para reiniciar los totales del tracker en cualquier momento.

## 🛠️ Cómo Instalarlo y Usarlo

1.  **Instala Tampermonkey**: Si aún no lo tienes, instala la extensión Tampermonkey en tu navegador (Chrome, Firefox, Edge, Opera, etc.).
    -   [Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
    -   [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
2.  **Crea un Nuevo Script**: Haz clic en el icono de Tampermonkey en tu navegador, luego selecciona `Crear un nuevo script...`.
3.  **Pega el Código**: Borra el código preexistente y pega todo el contenido de `skinclub-battle-tracker.js` en el editor.
4.  **Guarda el Script**: Ve a `Archivo` > `Guardar` (o presiona `Ctrl + S` / `Cmd + S`).
5.  **Configura tu Nombre de Usuario**: Abre el script en Tampermonkey y busca la línea `myUsername: 'EvasorFiscal'`. Cambia `'EvasorFiscal'` por tu nombre de usuario exacto en Skin.club.
6.  **Navega a Skin.club**: Abre o recarga cualquier página de batalla en `https://skin.club/`. El tracker debería aparecer en la esquina superior derecha.

## Ejemplo de Interfaz
![image](https://github.com/user-attachments/assets/6317a82c-3149-4906-b5cc-2f6b8d280bde)
