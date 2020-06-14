## Sistema de préstamos

Sistema de préstamos con roles de usuarios, desarrollado en Laravel + Blade. Puede administrar bóvedas, rutas, agente, supervisores, cierres de ruta, histórico de pagos, estadística de agente, reporte de gastos, perfil de cliente, entre otras cosas.

#### ¿Que puedo hacer con este sistema?

Gestionar roles de usuarios:
- Usuario
- Agente
- Supervisor
- Admin

#### Usuario
Hace referencia de una persona a quien se presta el dinero esta persona puede elegir entre N número de cuotas a pagar su préstamo con un % de interés.

#### Agente
Será el encargado de buscar nuevos clientes, registrar pagos, realizar la ruta de cobro siempre bajo el mando de un supervisor

![](https://i.imgur.com/kbvwudQ.gif)

#### Supervisor
Tiene bajo su control una bóveda de cual posee un historial de transacciones con un monto base y a su vez puede asignar sub montos a los agentes los cuales deben realizar préstamos y cobros.

![](https://i.imgur.com/DdkdJds.gif)

#### Admin
Encargado de crear las bóvedas, supervisor y agente. Siempre tiene el control de todos los otros módulos

![](https://i.imgur.com/KAX76ui.gif)

### Requerimientos
```
 "php": ">=5.6.4"
```

### Instalación
Ejecutar los siguientes comandos en orden
```cmd
git clone https://github.com/leifermendez/sistema-prestamos.git
```
```cmd
cd sistema-prestamos
```
```cmd
composer install
```
```cmd
php artisan key:generate
```
```cmd
php artisan migrate && php artisan db:seed
```