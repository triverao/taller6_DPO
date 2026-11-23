# Taller 6 – GUIs con Swing y Java2D (Restaurantes)

Aplicación de diario de restaurantes (visitados y por visitar) con interfaz gráfica en Swing y dibujo sobre el mapa con Java2D.

## Contenido
- `src/` – código fuente (proyecto Eclipse).
  - `uniandes.dpoo.swing.mundo` – modelo: `Diario`, `Restaurante`.
  - `uniandes.dpoo.swing.interfaz.principal` – `VentanaPrincipal`, `PanelBotones`, `PanelLista`, `PanelDetallesRestaurante`.
  - `uniandes.dpoo.swing.interfaz.agregar` – `VentanaAgregarRestaurante`, `PanelMapaAgregar`, `PanelEditarRestaurante`, `PanelBotonesAgregar`.
  - `uniandes.dpoo.swing.interfaz.mapa` – `VentanaMapa`, `PanelMapaVisualizar`.
- `imagenes/` – mapa y estrellas de calificación.
- `diagrama_clases.png` – diagrama de clases de la aplicación completa.

## Cómo ejecutar

### En Eclipse
1. `File > Import… > General > Existing Projects into Workspace`.
2. Seleccionar la carpeta `Taller6_GUI_Restaurantes` y finalizar.
3. Abrir `src/uniandes/dpoo/swing/interfaz/principal/VentanaPrincipal.java`.
4. Clic derecho → `Run As > Java Application`.

> Las imágenes se cargan con la ruta relativa `./imagenes/…`, por lo que el directorio de trabajo debe ser la raíz del proyecto (es el valor por defecto en Eclipse).

### Desde la terminal (desde la raíz del proyecto)
```bash
javac -encoding UTF-8 -d bin $(find src -name "*.java")
java -cp bin uniandes.dpoo.swing.interfaz.principal.VentanaPrincipal
```

## Uso
- **Nuevo**: abre la ventana para crear un restaurante. Haga click en el mapa para marcar la ubicación, escriba el nombre, escoja la calificación (1–5) e indique si ya fue visitado; luego **Crear restaurante**.
- **Ver todos**: abre el mapa con todos los restaurantes. Con los botones **Todos / Visitados** se filtra lo que se dibuja.
- Al seleccionar un restaurante en la lista se muestran su nombre, su calificación (estrellas) y si fue visitado.
