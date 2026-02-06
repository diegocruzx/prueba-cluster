===================================
Infraestructura del Leviatán
===================================


----

Especificaciones del Nodo Maestro
===================================


------------------------

:CPU: Intel(R) Xeon(R) E5-2680 v3 @ 2.50GHz
   - 24 hilos de procesamiento
   - Arquitectura Haswell

:Memoria RAM: 125 GiB

:Interfaz de Red: InfiniBand Mellanox ConnectX-3

:Sistema Operativo: Rocky Linux 9.6
   - Distribución empresarial compatible con RHEL
   - Optimizado para HPC

----

Particiones del Cluster
===================================


.. list-table:: 
   :widths: 15 10 45 15 15
   :header-rows: 1
   :align: center

   * - Partición
     - Nodos
     - Descripción
     - Características
     - Estado
   * - **normal**
     - 35
     - Cómputo general de propósito múltiple
     - Nodos C01-C38
     - Activo
   * - **fatcpu**
     - 40
     - Procesamiento con alta demanda de memoria
     - RAM extendida
     - Activo
   * - **gpu**
     - 2
     - Cómputo acelerado por GPU
     - Ampere/L402
     - Activo


----

Almacenamiento Global
===================================



**Directorio /home**
   :Capacidad: 111 TB
   :Tipo: Almacenamiento persistente compartido
   :Uso: Datos de usuario, scripts, resultados de larga duración
   :Respaldo: Incluido en respaldos periódicos

**Directorio local (scratch)**
   :Capacidad: 4.6 TB por nodo
   :Tipo: Almacenamiento temporal de alto rendimiento
   :Uso: Datos temporales durante la ejecución de trabajos
   :Respaldo: **No incluido** - los datos pueden eliminarse automáticamente


----

Contacto
========

LNS-BUAP
* Contacto: soporte-lns@cs.buap.mx