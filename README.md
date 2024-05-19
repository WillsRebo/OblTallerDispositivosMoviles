# OblTallerDispositivosMoviles
Obligatorio dle taller de Desarrollo de Dispositivos Móviles.

El objetivo de este obligatorio es desarrollar una pequeña parte de una aplicación web que permita aplicar los conceptos de desarrollo para dispositivos vistos en el taller.
Para ese objetivo se creará una aplicación que permita a un usuario la gestión de gastos y finanzas personales.

La consulta y persistencia de los datos se realizará mediante una API REST proporcionada por el equipo docente. La API REST no realizará ningún tipo de control de errores, es responsabilidad de los desarrolladores hacer llegar correctamente los datos al servidor.

Aplicación
La aplicación deberá permitir al usuario el registro de movimientos de gastos e ingresos de dinero, logrando de esta forma generar un histórico de gastos y análisis del mismo.

Con cada ingreso la aplicación deberá actualizar los datos estadísticos y métricas en tiempo real, en la misma pantalla y sin la necesidad de refrescar el navegador.

Se deberá prestar atención a los servicios disponibles en la API para poder utilizarlos todos.

Requerimientos funcionales
La aplicación deberá permitir realizar las siguientes funcionalidades:
1. Registro en la aplicación: se ingresará usuario, contraseña, departamento y ciudad. La API devolverá el éxito o el error en caso de que corresponda. En caso de éxito se devolverá la información del usuario y un token que se deberá agregar en todos los llamados a la API que se hagan. Se valorará el auto-login del usuario una vez hecho el registro mediante el uso de localStorage.

2. Login en la aplicación: En caso de éxito se devolverá la información del usuario y un token que se renueva al ingresar y se deberá agregar en todos los llamados a la API que se hagan.

3. Logout: se deberá poder cerrar la sesión para que otro usuario se loguee.

4. Agregar un gasto: la aplicación deberá permitir al usuario registrar gastos de diversos tipos y sus detalles.
• El usuario deberá agregar:
• Concepto de gasto, es decir, una descripción del gasto en concreto.
• Rubro. El usuario deberá seleccionar de un combo (previamente cargado con los valores devueltos por la API) el rubro al que corresponde el gasto, por ejemplo: Alimentación, Combustible, Educación, Paseos, Alquiler, Otros, etc.
• Medio. Los medios de pago pueden ser: Efectivo, Tarjeta de Débito o Tarjeta Crédito.
• Total. Importe en pesos del gasto.
• Fecha. Se deberá mostrar un calendario al usuario para que seleccione la fecha del gasto.

5. Agregar un ingreso: la aplicación deberá permitir al usuario registrar un ingreso. Para esto el usuario deberá completar la siguiente información:
• Concepto de ingreso, es decir, una descripción del ingreso en concreto.
• Rubro. El usuario deberá seleccionar entre los siguientes rubros: Aguinaldo, Sueldo, Honorarios, Salario vacacional, Rentas, Otros
• Medio. Los medios pueden ser: Efectivo o Banco.
• Total. Importe en pesos del ingreso.
• Fecha. Se deberá mostrar un calendario al usuario para que seleccione la fecha de ingreso.

6. Listado de movimientos: se listarán todos los movimientos del usuario, sin importar si son ingresos o gastos. De cada movimiento se deberán listar todos sus datos y además los mismos deberán tener un botón que permita eliminar el movimiento.

7. Filtro por tipo de movimiento: el listado de movimientos debe contar con un filtro que permita únicamente visualizar gastos o ingresos.

8. Montos totales: se deberá mostrar el valor total de gastos, ingresos y el saldo restante, es decir, ingresos menos gastos (tener en cuenta que este valor puede ser negativo)

9. Ubicar cajeros cercanos. Utilizando la ubicación del dispositivo. Se deberán mostrar en un mapa los cajeros que se encuentran a una distancia inferior a una distancia indicada. La información de los cajeros se obtiene de un llamado a la API que además devuelve si el cajero tiene disponibilidad de dinero o no, si recibe o no depósitos, y esa información debe reflejarse visualmente en el mapa.
    
10. Compartir que me gustó la aplicación. El usuario mediante un botón podrá compartir la URL de la aplicación (https://dwallet.develotion.com/site/) con sus contactos para recomendar su uso.

Requerimientos No funcionales
• La aplicación será construida utilizando Ionic Framework y JavaScript (sin combinarlo con ninguna otra librería o framework tales como Angular, React, Vue, etc.).
• Para el almacenamiento local, se utilizará local storage.
• La aplicación deberá ser generada únicamente para dispositivos Android.
• Se deberán controlar todos los posibles errores, ya sean devueltos por la API o generados del lado del cliente.

PRODUCTO Y ESTRUCTURA DE LA ENTREGA DEL OBLIGATORIO
El producto final deberá ser un APK instalable en dispositivos Android.
La entrega realizada deberá contener:
• El código fuente de la aplicación.
• El APK generado.

