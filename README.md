# IISSI-2 IS: Simulacro de examen de laboratorio

## Enunciado

La empresa ha decidido ofrecer a los propietarios la posibilidad de asociar un descuento (entero entre 0 y 100,
por ejemplo: 10) a sus restaurantes, para que posteriormente el sistema muestre y aplique el descuento
especificado a sus productos. Los propietarios podrán establecer un porcentaje de descuento diferente para cada
uno de sus restaurantes y que después se aplicarían a los productos de cada restaurante.
Sin embargo, algunos propietarios han indicado que no todos los productos de sus catálogos se promocionan
habitualmente. Por ello, la empresa ha decidido, además de permitir al restaurante indicar el porcentaje de
descuento sobre el precio original, dar la posibilidad de indicar en cada producto si será promocionado o no.
Todos los productos promocionados de un restaurante serán promocionados con el mismo porcentaje de
descuento que el propietario indique en las propiedades de sus restaurantes. Tenga en cuenta que un producto
puede estar promocionado pero, si el porcentaje de descuento indicado en el restaurante es 0%, no tendrá
ningún efecto. Sólo los propietarios de un restaurante podrán activar y desactivar los productos promocionados
así como indicar el descuento promocional.
Por defecto, los restaurantes no tendrán ningún porcentaje de descuento (es decir, el porcentaje de descuento
será 0).
Recuerde validar en el backend que, al promocionar/despromocionar un producto, el restaurante asociado tenga
un porcentaje de descuento superior a 0. En caso contrario, no podrá ser promocionado.
Por lo tanto, las vistas de edición y creación de los restaurantes deben incorporar un campo nuevo en el
formulario (InputItem) para cambiar el porcentaje de descuento, permitiendo al propietario ajustar el valor de la
propiedad. Recuerde validar en frontend (y backend) que el valor de ese nuevo campo es compatible con el tipo
de dato y las restricciones mencionadas.
Para que el propietario pueda determinar a qué productos se les aplica el descuento del restaurante, modifique la
vista de detalle del restaurante, donde se muestra el listado de sus productos, para que incluya un botón que
permita al propietario activar o desactivar la promoción para ese producto. En caso de que el restaurante no
tenga un descuento mayor que 0, no se mostrará este botón.
Las vistas de creación y edición de producto no incluirán la opción de aplicar o no aplicar el descuento.
El sistema debería mostrar los restaurantes con el descuento aplicado y la opción de promocionarlos o quitarles la
promoción tal y como se muestra en la siguiente captura de pantalla:

Recuerda que:
1. El descuento está en el intervalo [0,100].
2. Si un restaurante activa el descuento promocional, los productos pueden estar promocionados o no.
