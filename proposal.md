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
<img width="500" alt="modeloDominio" src="https://github.com/user-attachments/assets/2ca92542-bf50-4934-aa97-aa79b9c655fa" />


## Alcance Funcional (para Regularidad y Aprobacion Directa)

|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Producto<br>2. CRUD Proveedor<br>3. CRUD Empleado<br>4. CRUD Venta<br>5. CRUD Pedido<br>6. CRUD AlertaStock<br>7. CRUD ItemVenta<br>8. CRUD ItemPedido <br>|
|CRUD dependiente|1. CRUD Venta {depende de} CRUD Producto y CRUD Empleado<br>2. CRUD Pedido {depende de} CRUD Proveedor y CRUD Empleado<br>3. CRUD ItemVenta {depende de} CRUD Venta y CRUD Producto<br>4. CRUD ItemPedido {depende de} CRUD Pedido y CRUD Producto<br>|
|Listado<br>+<br>detalle| 1. Listado de productos con stock bajo, muestra alertas automaticamente => detalle CRUD AlertaStock<br>2. Listado de ventas por rango de fechas => detalle CRUD Venta<br>3. Listado de pedidos por estados (pendiente, recibido, cancelados) => detalle CRUD Pedido <br>4. Listado de proveedores con sus productos asociados => detalle CRUD Proveedor<br>|
|CUU/Epic|1. Registrar una venta y actualizar stock automaticamente<br>2. Generar pedido de reposicion a proveedor<br>3. Registrar recepcion de pedido y actualizar stock<br>4. Generar alertas de stock minimo|
