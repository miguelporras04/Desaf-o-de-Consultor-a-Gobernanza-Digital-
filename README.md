

# 

# 

# Desafío de Consultoría "Gobernanza Digital"

**Lenguaje de Marca**  
Miguel Porras González  
Javier Oliveros Lepe  
Jose Luis Contreras Brazo  
12/05/2026

[Bloque A: Análisis de Mercado y Selección (CE a, c)	3](#bloque-a:-análisis-de-mercado-y-selección-\(ce-a,-c\))

[Bloque B: Diseño de Seguridad RBAC (CE f)	3](#bloque-b:-diseño-de-seguridad-rbac-\(ce-f\))

[Bloque C: Documentación de Explotación (CE i)	3](#bloque-c:-documentación-de-explotación-\(ce-i\))

 Bloque A: Análisis de Mercado y Selección (CE a, c) {#bloque-a:-análisis-de-mercado-y-selección-(ce-a,-c)}

Debéis elegir entre **Odoo (SaaS o Community)**, **SAP S/4HANA** o **Zoho One**.

1. **Justifica la elección basándote en el perfil de la empresa (25 empleados, presupuesto ajustado, necesidad de personalización en el etiquetado).**

Hemos escogido Odoo por estas razones:  
**El costo** : al ser un código abierto , elimina el pago de licencias por el usuario , por lo que Odoo viene genial para este caso debido al presupuesto tan ajustado que tienen

**Personalización** : Permite modificar el código para necesidades un poco específicas como el etiquetado personalizado que han solicitado

Escalabilidad : Elimina el “Efecto Silo” que tenemos al integrar el inventario, clientes y facturación en una única plataforma

2. **Cálculo de TCO:** Realiza una estimación a 3 años. No olvidéis incluir:  
   * Coste de licencias/suscripción.  
   * Coste de implantación (vuestras horas de desarrollo: estima 100h a 40€/h).  
   * Coste operativo (Hosting en Google Cloud, AWS, Huawei Cloud o similar).

        

| Concepto | Detalle | Coste estimado |
| :---- | :---- | :---- |
| Licencias/Suscripción  | Odoo Community | 0€ |
| Implantación | 100 h de desarrollo x 40€/h | 4.000€ |
| Coste Operativo | Hosting (AWS/Google Cloud) 50€/mes | 1.800€ (36 meses) |
| Total ( 3 años ) |  | 5.800€ |

Bloque B: Diseño de Seguridad RBAC (CE f) {#bloque-b:-diseño-de-seguridad-rbac-(ce-f)}

Diseña la matriz de permisos para los siguientes roles, asegurando el **Principio de Mínimo Privilegio**:

* **Administrador:** Acceso total a todos los módulos y configuraciones

  **Restricciones**: Ninguna

* **Comercial:** Accesos a sus propios clientes y presupuestos

		**Restricciones**: No puede visualizar costes de producción ni datos contables globales

* **Operario de Almacén:** Acceso exclusivo a stock y albaranes de entrada/salida

  **Restricciones**: Sin acceso a facturación ni márgenes comerciales

* **Contable:** Lectura y gestión de facturas

  **Restricciones**: No puede modificar niveles de stock

Bloque C: Documentación de Explotación (CE i) {#bloque-c:-documentación-de-explotación-(ce-i)}

Siguiendo la norma **ISO/IEC 26514**, redacta un breve **Manual de Despliegue** para que el responsable de IT de la empresa pueda levantar el sistema en caso de caída. Debe incluir:

1. El fragmento de *docker-compose.yml* necesario.  
2. El comando para realizar un backup de la base de datos PostgreSQL.

BIBLIOGRAFIA

[https://blogempresas.masmovil.es/efecto-silo-en-los-negocios-un-mal-que-debes-evitar/\#:\~:text=evitar%20este%20mal.-,%C2%BFQu%C3%A9%20es%20el%20efecto%20silo%20en%20una%20empresa%3F,de%20manera%20efectiva%20entre%20ellos.](https://blogempresas.masmovil.es/efecto-silo-en-los-negocios-un-mal-que-debes-evitar/#:~:text=evitar%20este%20mal.-,%C2%BFQu%C3%A9%20es%20el%20efecto%20silo%20en%20una%20empresa%3F,de%20manera%20efectiva%20entre%20ellos.)

[https://trilio.io/es/digitales/Copia-de-seguridad-de-la-base-de-datos-de-Postgres/](https://trilio.io/es/digitales/Copia-de-seguridad-de-la-base-de-datos-de-Postgres/)
