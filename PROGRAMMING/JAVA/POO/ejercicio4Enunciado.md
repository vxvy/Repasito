Ejercicio: Sistema de Gestión de Biblioteca

**Descripción:**

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
   
Los libros pueden ser prestados a un sólo usuario por vez. Los usuarios no pueden rentar un libro que ya ha sido prestado. No hay tiempo límite para el préstamo.
Los libros deben tener nombre, género(fantasía, sci-fi, historia, etc.), número de páginas, FECHA de publicación y código ISBN definidos. En caso de no tener alguno de estos atributos el libro no aparecerá disponible para ser prestado

No uses una base de datos. Debería bastarte con colecciones de Java que sigan la interfaz <List>, la más sencilla es <ArrayList>

**Desafíos Adicionales:**
- Implementa un sistema de notificaciones cuando un libro se vuelve disponible.
- Añade una funcionalidad para calcular multas por retraso en la devolución de libros.
- Consultar los libros que se pueden prestar según su género 

**Requisitos:**

1. **Encapsulación:**
   - Todos los atributos de las clases deben ser privados.
   - Proporciona métodos públicos para acceder y modificar los atributos (getters y setters).

2. **Herencia:**
   - Crea una clase base llamada `ItemBiblioteca` que contenga atributos comunes como `id`, `titulo`, y `añoPublicacion`.
   - Hereda de `ItemBiblioteca` para crear dos clases: `Libro` y `Revista`. `Libro` añade atributos específicos como `autor` y `ISBN`, mientras que `Revista` añade `numero` y `periodicidad`.

3. **Modularidad:**
   - Divide el sistema en módulos lógicos: gestión de libros, gestión de usuarios, y préstamos.
   - Cada módulo debe estar en su propio paquete y contener clases e interfaces que permitan realizar las operaciones relevantes.

5. **Funcionalidades Específicas:**
   - Un usuario no puede tener más de 3 libros prestados simultáneamente.
   - Los libros pueden ser buscados por título, genero o ISBN.
   - Los usuarios pueden ser buscados por nombre o email.
   - Siempre que se imprima la lista de libros, debe estar ordenada
