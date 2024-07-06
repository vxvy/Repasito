Ejercicio: Sistema de Gesti�n de Biblioteca

**Descripci�n:**

Desarrolla un sistema para una biblioteca que permita gestionar libros y usuarios. 
El sistema debe permitir:
   - Agregar libros
   - Modificar libros
   - Eliminar libros
   - Buscar libros
   
   - Registrar usuarios 
   - Modificar usuarios 
   - Eliminar usuarios
   - Buscar usuarios 
   
Los libros pueden ser prestados a un s�lo usuario por vez. Los usuarios no pueden rentar un libro que ya ha sido prestado. No hay tiempo l�mite para el pr�stamo.
Los libros deben tener nombre, g�nero(fantas�a, sci-fi, historia, etc.), n�mero de p�ginas, FECHA de publicaci�n y c�digo ISBN definidos. En caso de no tener alguno de estos atributos el libro no aparecer� disponible para ser prestado

No uses una base de datos. Deber�a bastarte con colecciones de Java que sigan la interfaz <List>, la m�s sencilla es <ArrayList>

**Desaf�os Adicionales:**
- Implementa un sistema de notificaciones cuando un libro se vuelve disponible.
- A�ade una funcionalidad para calcular multas por retraso en la devoluci�n de libros.
- Consultar los libros que se pueden prestar seg�n su g�nero 

**Requisitos:**

1. **Encapsulaci�n:**
   - Todos los atributos de las clases deben ser privados.
   - Proporciona m�todos p�blicos para acceder y modificar los atributos (getters y setters).

2. **Herencia:**
   - Crea una clase base llamada `ItemBiblioteca` que contenga atributos comunes como `id`, `titulo`, y `a�oPublicacion`.
   - Hereda de `ItemBiblioteca` para crear dos clases: `Libro` y `Revista`. `Libro` a�ade atributos espec�ficos como `autor` y `ISBN`, mientras que `Revista` a�ade `numero` y `periodicidad`.

3. **Modularidad:**
   - Divide el sistema en m�dulos l�gicos: gesti�n de libros, gesti�n de usuarios, y pr�stamos.
   - Cada m�dulo debe estar en su propio paquete y contener clases e interfaces que permitan realizar las operaciones relevantes.

5. **Funcionalidades Espec�ficas:**
   - Un usuario no puede tener m�s de 3 libros prestados simult�neamente.
   - Los libros pueden ser buscados por t�tulo, genero o ISBN.
   - Los usuarios pueden ser buscados por nombre o email.
   - Siempre que se imprima la lista de libros, debe estar ordenada
