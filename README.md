# DAD-project
NOMBRE es una aplicación genérica de compra y venta de cosas. Cualquiera puede consultar las ofertas (los ítems a la venta en un momento dado), y los usuarios registrados pueden también (entre otras cosas) comprar o poner ítems en venta.

# Funcionamiento general de la aplicación
Los usuarios registrados pueden crear **ofertas**. Las ofertas tienen una serie de propiedades:
- Un **vendedor** (el usuario que las creó).
- Un **precio**, que establece el vendedor en su creación.
- Un **ítem**, que representa aquello que se está vendiendo.
- Una **fecha de creación** que se determina de forma automática.

Para que la búsqueda/filtrado de ofertas sea útil, los ítems también tienen propiedades:
- Un **nombre** (que no es único, es decir varios ítems de ofertas diferentes pueden tener el mismo nombre)
- Una **categoría**, que el creador de la oferta selecciona de una lista de categorías que le ofrece el sistema en el momento de su creación (la lista podría ser, por ejemplo, "comida", "muebles", y "otros"). 

Se pueden consultar las ofertas y filtrarlas utilizando cualquier combinación de estas propiedades (por ejemplo, las ofertas de ítems de categoría “comida” por debajo de 20 euros creadas por cierto vendedor).

Los usuarios registrados tienen cuentas. Las cuentas también tienen una serie de propiedades:
- Un **nombre** de usuario.
- Una **contraseña**.
- Una **puntuación de vendedor**, que se calcula en base a las puntuaciones que recibe de los compradores de sus ofertas.
- Puede haber uno o varios **comentarios** (de compradores) asociados a una cuenta.

Cuando un usuario _compra_ una oferta, debe puntuar al vendedor. La puntuación de vendedor de una cuenta es la media aritmética de todas las puntuaciones que recibe un usuario de este modo. Opcionalmente el comprador puede también dejar un comentario. Los comentarios tienen **autor** y **contenido**.
# Parte pública y privada de la aplicación
Los usuarios no registrados de la aplicación podrán:
- Consultar las ofertas (y filtrarlas).
- Ver perfiles de cuentas, donde podrán consultar la puntuación de vendedor y los comentarios de una cuenta.
- Crear una cuenta de usuario (registrarse).

Los usuarios registrados tendrán a su disposición toda la funcionalidad de la aplicación, pudiendo:
- Consultar ofertas y perfiles (igual que un usuario no registrado).
- Crear ofertas.
- _Comprar_ ofertas.
- Administrar su cuenta, por ejemplo cambiando la contraseña.

# Descripción de las entidades
# Descripción del servicio interno
