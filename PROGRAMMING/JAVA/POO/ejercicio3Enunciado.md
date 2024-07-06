Ejercicio: Sistema de Inventario para una Tienda de Art�culos Variados

**Descripci�n:**

Desarrolla un sistema de inventario para una tienda que vende art�culos variados, incluyendo libros, electr�nicos y ropa. El sistema debe permitir gestionar el inventario de estos art�culos, aplicando descuentos espec�ficos y mostrando detalles del producto de manera polim�rfica.

No uses una base de datos. Deber�a bastarte con colecciones de Java que sigan la interfaz <List>, la m�s sencilla es <ArrayList>

**Requisitos:**

1. **Abstracci�n:**
   - Crea una clase abstracta `Articulo` que contenga atributos comunes a todos los art�culos de la tienda, como `id`, `nombre`, `precio` y `cantidadEnStock`.
   - Define m�todos abstractos en `Articulo` para `aplicarDescuento()` y `mostrarDetalles()`.

2. **Polimorfismo:**
   - Implementa clases concretas para `Libro`, `Electronico` y `Ropa` que extiendan de `Articulo`.
   - Cada clase debe sobrescribir los m�todos `aplicarDescuento()` y `mostrarDetalles()`, proporcionando implementaciones espec�ficas. Por ejemplo, los libros podr�an tener un descuento diferente en comparaci�n con los electr�nicos y la ropa.

3. **Gesti�n de Inventario:**
   - Crea una clase `GestorInventario` que contenga una lista de `Articulo`. Esta clase debe permitir agregar art�culos al inventario, eliminarlos y mostrar los detalles de todos los art�culos.

4. **Funcionalidades Espec�ficas:**
   - `Libro` debe tener atributos adicionales como `autor` y `ISBN`.
   - `Electronico` puede tener atributos como `marca` y `modelo`.
   - `Ropa` podr�a incluir `talla` y `color`.
   - Implementa un m�todo en `GestorInventario` para aplicar descuentos a todos los art�culos y otro para mostrar los detalles de cada uno, demostrando polimorfismo.

**Desaf�os Adicionales:**
- A�ade una funcionalidad para buscar art�culos por nombre o categor�a (libro, electr�nico, ropa).
- Sobrecarga el m�todo equals para poder comparar Art�culos
- Crea una funci�n para saber cu�ntos Art�culos hay en inventario

