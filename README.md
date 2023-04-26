# Configuración para Visual Studio Code

Te dejo la configuración que utilizo en vscode para tener un editor más
prolijo y atractivo con extensiones productivas!

## Algunas extensiones recomendadas:

- Wildberries, Dracula Official, Nebula Oni Theme, SynthWave '84, Synthax: Temas de color
- MesloLGS NF: Fuente de editor
- Material Icon Theme: Logos para tus íconos
- Auto Rename Tag: Autocompletado de los tags html
- Babel JavaScript: Highlighting para js
- Black Formatter: Formatter para python
- CodeSnap: Para sacar capturas de tu código
- Indent-raibow: Para marcar las indentaciones con colores de arcoiris
- Indenticator: Para resaltar la indentación de la línea donde se encuentra tu cursor
- Live Server: Para tener un servidor rápido con html
- Prettier: Formatter para JavaScript, TypeScript, Flow, JSX, JSON, CSS, SCSS, Less HTML, Vue, Angular, HANDLEBARS, Ember, Glimmer, GraphQL, Markdown, YAML

## Cómo usar las mismas configuraciones?

Dentro de tu editor, presiona ctrl + shift + p. En el caso de mac: cmd + shift + p.
Luego busca settings.json y selecciona la opción que dice: `Open User Settings (JSON)`,
dentro pega la siguiente configuración.

```javascript
{
  "workbench.colorTheme": "Wildberries", // Tema Wildberries
  "editor.fontFamily": "'MesloLGS NF'", // Fuente MesloLGS NF
  "workbench.iconTheme": "material-icon-theme", // Tema de íconos
  "terminal.integrated.defaultProfile.linux": "zsh", // Terminal por defecto
  "editor.overviewRulerBorder": false, // Para quitar línea vertical derecha al lado de la barra deslizante
  "editor.hideCursorInOverviewRuler": true, // Para quitar esa pequeña franja que está en la barra deslizante
  "editor.scrollbar.vertical": "hidden", // Para ocultar la bara deslizante
  "editor.formatOnSave": true, // Para formatear al momento de guardar
  "editor.guides.indentation": false, // Para deshabilitar líneas fuertes en la indentación
  "indenticator.color.dark": "rgba(255, 255, 255, 0.1)", //(REQUIERE INSTALAR Indenticator extension) Para cambiar el color de las líneas de indentación (en este caso, blanco casi transparente, pero puedes elegir la que quieras :D)
  "editor.glyphMargin": false, // Ocultar la sección de depuración (los que están al lado de las líneas numéricas)
  "workbench.activityBar.visible": false, // Oculta la side bar
  "[python]": {
    "editor.defaultFormatter": "ms-python.black-formatter", // Black formatter para python (Muy buen formatter guiado por PEP)
    "editor.formatOnSave": true // Para formatear al momento de guardar
  },
  "python.formatting.provider": "black",
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "redhat.telemetry.enabled": true,
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "nebulaOni.update.restoreConfiguration": {
    "themeSettings": {
      "background": "Grey",
      "main": "Bumblebee",
      "highlight": "Ultra Violet",
      "focusBorder": "ON",
      "fontStyle": "Italic",
      "comments": "Dark Violet",
      "favorite": "OFF"
    },
    "favoriteSettings": {
      "background": "Glacial Blue",
      "main": "Sakura",
      "highlight": "Ultra Violet",
      "focusBorder": "ON",
      "fontStyle": "Italic",
      "comments": "Dark Magenta",
      "favorite": "Nebula Oni (Pegasus)"
    }
  },
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode" // Formatter de HTML
  },
  "[markdown]": {
    "editor.defaultFormatter": "yzhang.markdown-all-in-one" // Formatter de Markdown
  }
}
```
