# Propuesta TP DSW

## Grupo
### Integrantes
* 52315 - Axinte, Adrian
* 53221 - Rosatelli, Bruno
* 54245 - Benitez, Laureano

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)

## Tema
### Descripción
El sistema se va a destinar a la gestion de un comercio minorista. El objetivo es optimizar las operaciones diarias del negocio mediante el control del stock de productos, el registro de ventas y administracio de proveedores. De esta forma, se busca mejorar la eficiencia del negocio, reducir pérdidas por faltantes y facilitar la administracion comercial.

### Modelo
<img width="641" height="911" alt="Modelo Dominio Desarrollo Nuevo drawio" src="https://github.com/user-attachments/assets/8db8c652-f29b-4e85-b7f9-8b4c6fd9d947" />


## Alcance Funcional (para Regularidad y Aprobacion Directa)

| Req                     | Detalle                                                                                                                                                                                                                                                                                                                           |
| :---------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CRUD simple             | 1. CRUD Producto<br>2. CRUD Proveedor<br>3. CRUD Empleado<br>4. CRUD Rol<br>5. CRUD Categoria_Prod                                                                                                                                                                                                                                |
| CRUD dependiente        | 1. CRUD Producto depende de CRUD Categoria_Prod y CRUD Proveedor<br>2. CRUD Empleado depende de CRUD Rol <br>                                                                                                                                                                                                                                                                |
| Listado<br>+<br>detalle | 1. Listado de productos con stock bajo, muestra alertas automáticamente => detalle AlertaStock<br>2. Listado de ventas por rango de fechas => detalle Venta<br>3. Listado de pedidos por estados (pendiente, recibido, cancelado) => detalle Pedido<br>4. Listado de proveedores con sus productos asociados => detalle Proveedor |
| CUU/Epic                | 1. Registrar una venta y actualizar stock automáticamente<br>2. Generar pedido de reposición a proveedor<br>3. Registrar recepción de pedido y actualizar stock<br>4. Generar alerta de stock mínimo                                                                                                                              |
