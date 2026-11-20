# SI · UT2 — Ficha de taller: montaje y revisión de un ordenador

## 1. Orden de trabajo

**Fecha:** 17/11/2026  **Puesto:** ____________________  **Equipo / etiqueta:** Sobremesa slim, caja Dominion (etiqueta en la parte trasera)

**Integrantes del grupo (2 o 3):**

1. Nombre y apellidos: Adrián Gámez Espigares
2. Nombre y apellidos: Alejandro Correa
3. Nombre y apellidos (si procede): __________________________________

> **Equipo A:** ordenador de prácticas utilizado para el montaje o la revisión. Puede estar averiado; no se exige que arranque.
>
> **Equipo B:** vuestro propio ordenador funcional. Se utiliza a partir del apartado 9 para analizar el arranque y el hardware desde Linux.

## 2. Recepción e inspección visual · Equipo A

**Trabajo previsto:**

- [x] Desmontaje y montaje
- [ ] Revisión / diagnóstico
- [ ] Otro: ___________________________________

**Estado al recibirlo:**

- [x] Completo
- [ ] Faltan piezas
- [ ] Sucio
- [ ] Daños visibles

**Síntomas conocidos, piezas ausentes o daños observados:**

No se observan piezas ausentes ni daños visibles. No se indicaron síntomas de avería (práctica de mantenimiento preventivo).

## 3. Seguridad y preparación · Equipo A

- [x] Equipo desconectado de la corriente y de los periféricos.
- [x] Botón de encendido pulsado tras desconectar.
- [x] Superficie despejada y piezas organizadas.
- [x] Estado inicial y conexiones fotografiados.

**Herramientas utilizadas:** Destornillador de estrella (Phillips), caja transparente para organizar los tornillos y papel para limpiar la pasta térmica antigua.

**No abráis la fuente ni forcéis piezas.** Ante daños o baterías, avisad al profesor.

## 4. Componentes identificados · Equipo A

Anotad lo que podáis verificar. Si no se distingue, escribid «no identificado».

| Componente | Marca / modelo | Dato observado |
|---|---|---|
| Placa base | Gigabyte GA-B85M-DS3H (rev. 3.0) | Socket LGA1150, micro-ATX, UEFI DualBIOS, salidas VGA / DVI / HDMI, 4 ranuras DIMM, pila de botón CMOS |
| Procesador | Intel Celeron G1840 (SR1VK) | 2,80 GHz, socket LGA1150 |
| RAM | Crucial (módulo DIMM) | Capacidad no legible en las fotos: no identificado |
| Almacenamiento | WD Blue WD5000AAKX-00ERMA0 | 500 GB, SATA, 16 MB de caché, 3,5", fabricado el 07/12/2014 |
| Fuente | Modelo IP-S300EF7-2 H (marca no identificada) | 300 W; +3,3 V/18 A, +5 V/18 A, +12 V/18 A, –12 V/0,3 A, +5 VSB/2 A |
| Disipador / ventilador | Intel original, ref. E97379-001 (CNFN4344V2), Foxconn | 12 V, 0,17 A, conector de 4 pines |
| Tarjetas / otros | Tarjeta WiFi PCIe (marca no identificada) | WLAN PCI-E 300 Mbps, 2,4 GHz 802.11 b/g/n, 2 conectores de antena |

## 5. Conexiones y observaciones · Equipo A

Identificad y marcad las conexiones presentes y comprobadas:

- [x] Alimentación de la placa
- [x] Alimentación de la CPU
- [x] Ventilador de la CPU
- [x] Datos de almacenamiento
- [x] Alimentación del disco
- [x] Panel frontal

**¿Hay algún cable suelto, conector dañado o conexión que no sepáis identificar?**

No había cables sueltos ni conectores dañados. El conector del panel frontal se identificó con el serigrafiado de la placa (F_PANEL).

**Fotografías de referencia (nombre de archivo o ubicación):**

Todas están en la carpeta `img/` de este repositorio (`Curso_26_27-SI/UT2/img/`).

*Estado inicial*

![montaje-01-caja-trasera.jpg: parte trasera de la caja Dominion](img/montaje-01-caja-trasera.jpg)

![montaje-02-interior-inicial.jpg: interior al abrir el equipo](img/montaje-02-interior-inicial.jpg)

*Conexiones del panel frontal*

![montaje-03-panel-frontal.jpg: cables del panel frontal en F_PANEL](img/montaje-03-panel-frontal.jpg)

*Piezas desmontadas*

![montaje-04-piezas-desmontadas.jpg: piezas organizadas sobre la mesa](img/montaje-04-piezas-desmontadas.jpg)

![montaje-16-placa-base.jpg: placa base Gigabyte GA-B85M-DS3H fuera de la caja](img/montaje-16-placa-base.jpg)

*Componentes (etiquetas)*

![montaje-12-disco-etiqueta.jpg: etiqueta del disco WD Blue 500 GB](img/montaje-12-disco-etiqueta.jpg)

![montaje-13-disco-reverso.jpg: cara inferior del disco con su placa](img/montaje-13-disco-reverso.jpg)

![montaje-14-fuente-etiqueta.jpg: etiqueta de la fuente IP-S300EF7-2 H](img/montaje-14-fuente-etiqueta.jpg)

![montaje-15-tarjeta-wifi.jpg: tarjeta WiFi PCIe de 300 Mbps](img/montaje-15-tarjeta-wifi.jpg)

*Procesador y disipador*

![montaje-05-cpu-g1840.jpg: procesador Intel Celeron G1840](img/montaje-05-cpu-g1840.jpg)

![montaje-06-socket-vacio.jpg: socket LGA1150 vacío](img/montaje-06-socket-vacio.jpg)

![montaje-07-disipador-intel.jpg: disipador Intel con ventilador de 4 pines](img/montaje-07-disipador-intel.jpg)

![montaje-08-placa-con-disipador.jpg: disipador montado de nuevo con pasta térmica renovada](img/montaje-08-placa-con-disipador.jpg)

*Remontaje y cierre*

![montaje-09-remontaje-con-fuente.jpg: placa y fuente montadas en la caja](img/montaje-09-remontaje-con-fuente.jpg)

![montaje-10-disco-reinstalado.jpg: disco reinstalado en su bandeja](img/montaje-10-disco-reinstalado.jpg)

![montaje-11-equipo-cerrado.jpg: equipo cerrado al terminar](img/montaje-11-equipo-cerrado.jpg)

No retiréis la CPU ni el disipador sin indicación del profesor. Si se retira el disipador, consultad sobre limpieza y pasta térmica antes de volver a instalarlo.

## 6. Registro del trabajo · Equipo A

Registrad únicamente lo que hayáis hecho; marcad **N/P** si no procede.

| Operación | Hecho | N/P | Foto / observaciones |
|---|:---:|:---:|---|
| Apertura y fotos iniciales | ☒ | ☐ | `montaje-01-caja-trasera.jpg`, `montaje-02-interior-inicial.jpg` |
| Desconexión y organización de cables | ☒ | ☐ | `montaje-03-panel-frontal.jpg`, `montaje-04-piezas-desmontadas.jpg` |
| Desmontaje / montaje de memoria | ☒ | ☐ | `montaje-16-placa-base.jpg` (ranuras DIMM sin el módulo) |
| Revisión / montaje de almacenamiento | ☒ | ☐ | `montaje-12-disco-etiqueta.jpg`, `montaje-13-disco-reverso.jpg`, `montaje-10-disco-reinstalado.jpg` |
| CPU y disipador, si se autoriza | ☒ | ☐ | `montaje-05-cpu-g1840.jpg`, `montaje-06-socket-vacio.jpg`, `montaje-07-disipador-intel.jpg`, `montaje-08-placa-con-disipador.jpg`. Se renovó la pasta térmica con un punto en el centro |
| Tarjetas de expansión | ☒ | ☐ | `montaje-15-tarjeta-wifi.jpg` |
| Reconexión y orden de cables | ☒ | ☐ | `montaje-09-remontaje-con-fuente.jpg` |
| Cierre y limpieza del puesto | ☒ | ☐ | `montaje-11-equipo-cerrado.jpg` |

## 7. Incidencia o reparación · Equipo A

**Problema encontrado / hipótesis** (si no hay, indicadlo):

No se encontró ningún problema. La práctica fue de mantenimiento preventivo.

**Acción realizada y resultado observado:**

Se desmontó el equipo completo, se retiró el disipador y se limpió la pasta térmica antigua. Se aplicó un punto de pasta térmica nueva sobre la CPU, se volvió a colocar el disipador y se reconectó todo. Resultado: equipo montado de nuevo con los cables ordenados (`montaje-09-remontaje-con-fuente.jpg`).

## 8. Comprobación final · Equipo A

- [x] Piezas sujetas.
- [x] RAM encajada.
- [x] Cables revisados.
- [x] Sin tornillos sueltos.
- [x] Ventilador de CPU conectado.
- [x] Puesto recogido.

**¿Encendido autorizado?** ☐ Sí  ☐ No

**Resultado / motivo:** ___________________________________________________

Una observación no demuestra por sí sola la causa de una avería.

---

## 9. Identificación y arranque · Equipo B

> ⚠️ **PENDIENTE (borrar este aviso al completar los apartados 9 a 13 y 15):** hay que rellenarlos con vuestro propio ordenador con Linux.

Utilizad vuestro propio ordenador funcional para los siguientes apartados.

**Equipo:** ☐ Portátil  ☐ Sobremesa  ☐ Otro: ___________________________

**Linux:** ☐ Instalado directamente  ☐ Máquina virtual

**Sistema operativo y versión:** __________________________________________

**Si es virtual: sistema anfitrión y programa de virtualización:** ______________

**¿Arranca con normalidad? ¿Qué observáis desde el encendido hasta el inicio?**

________________________________________________________________________

**¿Qué es el POST y en qué se diferencia de la UEFI y del sistema operativo?**

________________________________________________________________________

**¿Habéis accedido a la UEFI o consultado información de ella? ¿Qué dato habéis visto?**

________________________________________________________________________

No cambiéis ajustes de UEFI sin indicación del profesor. Si no podéis acceder, indicadlo.

## 10. Linux: procesador · `lscpu`

Ejecutad `lscpu`. Adjuntad la salida revisada o indicad si el comando falla.

```text
(pega aquí la salida de lscpu)
```

**Modelo / CPU presentada a Linux:** _______________________________________

**Arquitectura:** ____________________  **CPU lógicas visibles:** ______________

**¿Qué diferencia hay entre núcleo e hilo? ¿Qué podéis concluir de la salida?**

________________________________________________________________________

## 11. Linux: memoria · `free -h`

Adjuntad las salidas de los comandos. Si alguno falla o no está disponible, anotadlo. Antes de entregarlas, ocultad usuarios, nombres de equipo, números de serie y UUID. En una máquina virtual pueden mostrarse recursos virtuales, no el hardware físico completo.

```text
(pega aquí la salida de free -h)
```

**Memoria total:** ____________________  **Memoria disponible:** ______________

**¿Qué significa «disponible» y por qué puede diferir de «libre»?**

________________________________________________________________________

## 12. Linux: almacenamiento · `lsblk`

```text
(pega aquí la salida de lsblk)
```

**Disco identificado:** ___________________________________________________

**Partición y punto de montaje, si aparecen:** ________________________________

**Explicad la diferencia entre disco, partición y punto de montaje:**

________________________________________________________________________

## 13. Linux: dispositivos · `lspci` y `lsusb`

```text
(pega aquí la salida de lspci)
```

```text
(pega aquí la salida de lsusb)
```

**Dispositivo 1 y función:** ________________________________________________

**Dispositivo 2 y función:** ________________________________________________

**¿Por qué podría no aparecer un componente físico o mostrarse de otra forma en una máquina virtual?**

________________________________________________________________________

## 14. Duda técnica y uso crítico de IA

Podéis usar una IA de Internet. No compartáis datos personales ni información privada del centro. Sin acceso a IA, resolved la duda con una fuente técnica.

**Herramienta utilizada y fecha:** Claude (Anthropic), 20/11/2026

**Pregunta planteada:**

Cómo rellenar esta ficha (apartados 1 a 8) a partir de las fotos que hicimos del montaje, y cómo ordenar los apartados y las fotos en este fichero.

**Respuesta resumida y afirmación concreta que decidisteis comprobar:**

La IA identificó los componentes (placa Gigabyte GA-B85M-DS3H, Intel Celeron G1840, disco WD Blue de 500 GB, fuente IP-S300EF7-2 H, disipador Intel y tarjeta WiFi PCIe) a partir de las etiquetas que se ven en las fotos. Decidimos comprobar esa identificación.

**Fuente técnica o prueba utilizada y resultado:** confirmada / corregida / no verificada.

Confirmada con las etiquetas visibles en las fotos (`montaje-05-cpu-g1840.jpg`, `montaje-12-disco-etiqueta.jpg`, `montaje-14-fuente-etiqueta.jpg`, `montaje-16-placa-base.jpg`). La capacidad de la RAM y la marca de la fuente no se leen en las fotos, por eso figuran como «no identificado». No se comprobó con ningún programa porque el equipo A no se arrancó con Linux.

## 15. Valoración y entrega

**¿Qué paso fue más difícil y cómo lo resolvisteis?**

________________________________________________________________________

**¿Qué relación existe entre el montaje y la información de Linux? Recordad que son equipos distintos.**

________________________________________________________________________

**¿Qué haríais de otra manera en un próximo montaje?**

________________________________________________________________________

Antes de entregar:

- [ ] Ficha completa.
- [ ] Fotos identificadas.
- [ ] Salidas de Linux revisadas.
