*Explicación*

HTML:

- La estructura básica incluye dos divs para los círculos de progreso.
- Cada círculo tiene un atributo data-percentage con el valor del porcentaje objetivo.

CSS:

- body, html: Configuración para centrar todo el contenido en la página.
container: Usa Flexbox para alinear los gráficos uno al lado del otro.
- circulo-progrecibo: Define el estilo de los gráficos de progreso:
- --porcentage: Variable CSS personalizada para almacenar el valor del porcentaje.
- animation: Aplica la animación definida en @keyframes loadProgress que ajusta la carga del círculo desde 0% hasta el valor del porcentaje.
- circulo-progrecibo-[data-percentage="..."]: Define el color y el porcentaje objetivo para cada círculo.
- circulo-progrecibo
: Añade un efecto de escala al pasar el ratón sobre el círculo.
- circulo-interno: Círculo interno más pequeño para crear un anillo.
- porcentage: Estilo para centrar el texto del porcentaje dentro del círculo interno.
@keyframes loadProgress: Define la animación que ajusta el fondo del círculo desde 0% hasta el porcentaje objetivo.

Con este enfoque, al cargar la página, cada círculo de progreso se animará desde 0% hasta su porcentaje objetivo definido en data-percentage, utilizando sólo HTML y CSS.