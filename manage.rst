Actualización de equipos del aula o centro
==========================================

Una vez tenga actualizado el repositorio del que depende su equipo, podrá utilizar LliureX-Up para mantenerlo al día.

.. important::
   El hecho de tener una réplica del repositorio actualizada no significa que el equipo esté actualizado. Para aplicar las novedades recibidas en dicha sincronización es necesario lanzar LliureX-Up.

Las posibilidades son varias:

* Si el equipo está fuera de las aulas de informática, y disponen de un servidor de centro, lo lógico es que dependa de éste para sus actualizaciones.
* En el caso de ser un equipo en una aula de informática, dependerá del servidor de dicha aula.

  * Si ha configurado el servidor del aula como se comentaba en la sección de `Réplicas internas (Modelo de Centro)`_, deberá actualizar primero el servidor de centro y, una vez finalizada su actualización, proceder con el servidor de aula (que se sincroniza con las novedades del de centro). Una vez acabado este último, podrá comenzar la actualización del equipo.
  * En caso contrario, cada servidor actúa de manera independiente y se sincroniza directamente con el repositorio central de LliureX. De la misma manera, debe refrescar el servidor del aula antes de proceder a la del equipo.

En todo caso, puede actualizar un conjunto de equipos simultáneamente mediante la herramienta de *Gestión remota de clientes* en el *Centro de Control de LliureX*. Esta herramienta establece (desde un servidor) una conexión con todos los equipos cliente que dependen de él. Aparecerá una línea de comandos desde la que podrá ejecutar una orden simultánea: *sudo lliurex-upgrade*. De esta manera, todos los clientes accedidos empezarán el proceso de actualización usando el repositorio (que debe estar recién sincronizado) del servidor local al que estan conectados (si llevan la configuración por defecto).

.. todo:: Procedimiento para la actualización de equipos aislados o con baja conectividad.
