# Initial Grid

A fully customizable CSS flexbox grid system for a fast starting point.

## Usage

### Columns of the same size

```html
<div class="row">
	<div class="column">...</div>
	<div class="column">...</div>
	<div class="column">...</div>
</div>
```

### Columns of different size

```html
<div class="row">
	<div class="column-4">...</div>
	<div class="column-8">...</div>
</div>
```

### Horizontal modifiers

Para cambiar la alineación horizontal de las columnas, agrega solamente una de estas clases junto a la clase `row` que desees.

| Class | Description |
|---|---|
| `columns-left` | Columns aligned to the left of the row. |
| `columns-center` | Columns are centered along the row. |
| `columns-right` | Columns are aligned toward to end of the row. |
| `columns-between` | Columns are evenly distributed in the row; first column is on the start, last column on the end. |
| `columns-around` | Columns are evenly distributed in the row with equal space around them. |

### Vertical modifiers

Si por otra parte deseas cambiar la alineación vertical de las columnas, solo agrega una de estas clases junto a la clase `row` que desees.

| Class | Description |
|---|---|
| `columns-top` | Columns aligned to the top of the row. |
| `columns-middle` | Columns aligned in the middle of the row. |
| `columns-bottom` | Columns aligned in the bottom of the row. |

También puedes alinear verticalmente alguna de las columnas de manera individual. Recuerda que para que las columnas se vean alineadas, el contenedor tiene que ser más grande que las columnas.

| Class | Description |
|---|---|
| `column-top` | Column aligned to the top of the row. |
| `column-middle` | Column aligned in the middle of the row. |
| `column-bottom` | Column aligned in the bottom of the row. |

### Offsets

Nos sirven para compensar el espacio vacío en el `row` que contiene una columna de menor tamaño. Supongamos que solo queremos una columna de ancho de 6 columnas, si le agregamos una clase `column-offset-3` está quedará centrada (3 + 6 + 3) por ser un grid de doce columnas:

```html
<div class="row">
	<div class="column-6 column-offset-3">
		<span>...</span>
	</div>
</div>
```

### Responsive classes

| Class | Description |
|---|---|
| `column-small-<number>` | Tamaño de la columna en pantallas que tienen un ancho menor a 640 píxeles. |
| `column-medium-<number>` | Tamaño de la columna en pantallas que tienen un ancho desde 640 píxeles. |
| `column-large-<number>` | Tamaño de la columna en pantallas que tienen un ancho desde 1024 píxeles. |

### Collapse columns

A veces hay momentos en los que es mejor trabajar con columnas sin márgenes, agrega la clase `columns-collapse` a cualquier `row` para remover los espacios entre las columnas.

You can see the grid in action on demo page.
