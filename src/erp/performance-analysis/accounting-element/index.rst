.. _ERPyA: http://erpya.com

.. |Estructura de Cuentas| image:: resources/Structure-Account.png

.. _src/erp/performance-analysis/accounting-element:

=====================
**Elemento Contable**
=====================

El elemento contable le permite definir de forma sistemática una estructura de cuentas y los parámetros que serán utilizados en el :ref:`documento/tipo-de-aplicación` contable.

Esta estructura actúa como el plan de cuentas contable, presentando una lista de cuentas contables en las cuales serán registrados los hechos contables generados desde los procesos administrativos de Solop ERP. Estos elementos generalmente son ordenados bajo una codificación que facilitan el reconocimiento de cada cuenta.

El método consiste en asignar un número decimal que nos permita asociar la clasificación de las cuentas:

**Cuentas Reales**: Son denominadas así las cuentas que mantienen saldo durante y posterior a un periodo contable y que son conservadas en el balances. Generalmente estas cuentas son útiles para :ref:`documento/informe-financiero`, dentro de estas cuentas se encuentran:

    **Activos:** Se refiere a los bienes de los que una empresa dispone y tiene derechos, sean tangibles o intangibles.

    **Pasivos:** Se refiere a los compromisos u obligaciones que la empresa contrae con una entidad.

    **Patrimonio:** Se refiere a los aportes realizados por accionistas de la empresa.

**Cuentas Nominales**: Son denominadas así las cuentas que son cerradas al finalizar el período contable, transfiriendo el saldo a las cuentas reales, y posteriormente iniciarán con saldo cero, con el objetivo de iniciar el balance con estas cuentas limpias, dentro de estas cuentas se encuentran:

    **Ingresos:** Se refiere a la ganancia o dinero que ingresa a la empresa.

    **Costos:** Se refiere al dinero que egresa de la empresa con la finalidad de generar un activo.

    **Gastos:** Se refiere al dinero que egresa de la empresa que no genera activos.

Estas cuentas han sido estandarizadas a nivel mundial de la siguiente forma:

+------------+------------+-----------+------------+------------+-----------+
| Activos    | Pasivos    | Patrimonio| Ingresos   |Costos      |Gastos     |
+============+============+===========+============+============+===========+
| 1          | 2          | 3         | 4          | 5          | 6         |
+------------+------------+-----------+------------+------------+-----------+

En Solop ERP los códigos de las cuentas son conformados con números con la siguiente estructura:

|Estructura de Cuentas|

Imagen 1. Estructura de Cuentas Contables

Para este ejemplo podríamos establecer la siguiente figura:

+------------+------------+-------------+--------+-----------------+
| Activos    |Corrientes  | Disponibles | Banco  |Cuenta Bancaria  |
+============+============+=============+========+=================+
| 1          | 1          | 1           | 0001   | 0001            |
+------------+------------+-------------+--------+-----------------+

El elemento contable es necesario para la definición del esquema contable, que a su vez define el óptimo funcionamiento de Solop ERP, esto es porque cada transacción administrativa generará un asiento contable y por ende son requeridas las cuentas contables.

En esta oportunidad se ha diseñado para usted un material en el cual se define detalladamente esta ventana que frecuentemente será visitada por usted, que ha decidido incursionar en el uso de Solop ERP.

.. toctree::
    :maxdepth: 2

    accounting-element