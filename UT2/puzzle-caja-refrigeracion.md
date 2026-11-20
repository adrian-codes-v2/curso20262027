# Caja y refrigeración: cómo sacar el calor del PC

**Sistemas Informáticos · 1.º DAW · UT2 (puzzle)** · Autor: Adrián Gámez Espigares · Pareja: Alejandro Correa · Noviembre 2026

## 1. Resumen de una cara

**Para qué sirve.** Cuando un procesador trabaja, convierte la electricidad en calor. Si ese calor no sale, la CPU baja su velocidad para protegerse (*thermal throttling*), el equipo puede apagarse y los componentes se desgastan antes. Intel indica una temperatura máxima de unión de 100 °C para el Core i9-14900K y AMD de 95 °C para el Ryzen 9 7950X [1][3].

![Recorrido del calor: CPU, pasta térmica, disipador, ventilador y caja](img/recorrido-calor.png)

*Esquema de elaboración propia: el calor pasa por cinco piezas y, si una falla, se queda atascado.*

**Cómo funciona.** La CPU se calienta; la **pasta térmica** rellena los huecos microscópicos entre la CPU y el disipador; el **disipador** (metal con aletas y tubos de calor) reparte el calor; el **ventilador** lo arrastra con aire; y la **caja** lo expulsa. El aire fresco entra por delante y el caliente sale por detrás y por arriba.

**Tipos.** Refrigeración por **aire** (disipador + ventilador) o líquida **AIO** (bomba, tubos y radiador). Las dos enfrían bien; cambian el espacio que ocupan y el precio.

**Leer una ficha técnica.**

| Dato | Unidad | Qué significa |
|---|---|---|
| TDP | W | Calor que tiene que sacar el disipador |
| Velocidad | RPM | Vueltas por minuto del ventilador |
| Caudal | m³/h | Cuánto aire mueve |
| Presión estática | mmH₂O | Fuerza para empujar el aire a través de obstáculos |
| Ruido | dB(A) | Cuanto menor, más silencioso |
| Vida útil / MTTF | horas | Tiempo medio hasta el fallo, no una garantía |

**Ojo con el TDP.** La cifra anunciada no es el máximo. El i9-14900K tiene 125 W de potencia base y 253 W de potencia máxima en turbo [1]. El Ryzen 9 7950X tiene 170 W de TDP y 230 W de límite de potencia (PPT) [3][4]. El disipador se elige pensando en la cifra alta.

**Ventiladores.** Los de **caudal** mueven mucho aire si no hay obstáculos (frontal y trasero de la caja). Los de **presión estática** empujan aunque algo estorbe (radiadores y disipadores con muchas aletas). Con conector de **4 pines (PWM)** la placa sube y baja la velocidad sola.

**Ejemplo real: Noctua NH-D15** [2]. Doble torre con 6 tubos de calor y 2 ventiladores de 140 mm PWM. Altura de 168 mm con ventiladores y 1320 g de peso. Sus ventiladores dan como máximo 24,6 dB(A), 140,2 m³/h y 2,08 mmH₂O, con un MTTF de más de 150 000 h. Hay que comprobar que quepa en la caja.

**Montaje y errores típicos.** Basta un punto de pasta del tamaño de un guisante. Los fallos habituales: dejar el plástico protector del disipador, conectar mal el ventilador de la CPU (debe ir a `CPU_FAN`), poner ventiladores al revés (la flecha del marco indica el sentido del aire) y no limpiar el polvo ni renovar la pasta seca con los años.

**Fuentes**

1. Intel, [Core i9-14900K: especificaciones](https://www.intel.com/content/www/us/en/products/sku/236773/x/specifications.html) (potencia base 125 W, potencia máxima turbo 253 W) y [ficha del 14900KF](https://www.intel.com/content/www/us/en/products/sku/236787/x/specifications.html) (TJUNCTION 100 °C).
2. Noctua, [NH-D15: especificaciones](https://noctua.at/en/nh-d15/specification) y [hoja de datos](https://noctua.at/pub/media/blfa_files/infosheet/noctua_nh_d15_datasheet_en_web.pdf).
3. AMD, [Ryzen 9 7950X](https://www.amd.com/en/products/processors/desktops/ryzen/7000-series/amd-ryzen-9-7950x.html) (TDP 170 W, Tjmax 95 °C).
4. TechPowerUp, [AMD Ryzen 9 7950X Review](https://techpowerup.com/review/amd-ryzen-9-7950x) (PPT 230 W).
5. Esquemas: elaboración propia (presentación del Grupo 10, *Caja y refrigeración*).

## 2. Test (5 preguntas)

**1. ¿Qué hace la pasta térmica entre la CPU y el disipador?**

- [ ] a) Aísla eléctricamente la CPU del disipador
- [x] b) Rellena los huecos microscópicos para que el calor pase mejor al disipador
- [ ] c) Pega el disipador a la CPU
- [ ] d) Enfría la CPU por sí sola

*Explicación:* las superficies parecen lisas pero tienen irregularidades; la pasta sustituye el aire atrapado, que conduce muy mal el calor. No pega ni enfría por sí misma.

**2. Un procesador anuncia 125 W de potencia base y 253 W de potencia máxima en turbo (como el i9-14900K). ¿Qué cifra conviene tener en cuenta al elegir el disipador?**

- [ ] a) La de 125 W, porque es la oficial
- [ ] b) La media de las dos
- [x] c) La de 253 W, porque en turbo puede llegar a gastarla y generar ese calor
- [ ] d) Ninguna, el disipador no depende del consumo

*Explicación:* el TDP o la potencia base no es el máximo. Si el disipador solo cubre la cifra baja, en carga alta la CPU se calienta y baja su velocidad.

**3. ¿Para qué ponemos un ventilador de presión estática?**

- [ ] a) Para la parte frontal de la caja, sin nada delante
- [x] b) Para radiadores y disipadores con muchas aletas, que ofrecen resistencia al aire
- [ ] c) Para sustituir al disipador
- [ ] d) Para que el PC haga menos ruido siempre

*Explicación:* los de caudal mueven mucho aire con poca resistencia; los de presión estática lo empujan aunque haya obstáculos, como las aletas de un radiador.

**4. ¿Qué ventaja tiene un ventilador con conector de 4 pines (PWM)?**

- [ ] a) Gira siempre al máximo
- [ ] b) No necesita alimentación
- [x] c) La placa base puede subir y bajar su velocidad automáticamente según la temperatura
- [ ] d) Solo sirve para refrigeración líquida

*Explicación:* el cuarto pin lleva la señal de control (PWM). Con 3 pines solo se puede regular variando el voltaje, y no todas las placas lo permiten.

**5. Al montar un equipo aparece «CPU Fan Error» en el arranque. ¿Cuál es la causa más probable?**

- [ ] a) La pasta térmica es de mala calidad
- [ ] b) La RAM está mal encajada
- [x] c) El ventilador de la CPU no está conectado al conector `CPU_FAN` de la placa
- [ ] d) La fuente tiene poca potencia

*Explicación:* la placa vigila las RPM del ventilador desde `CPU_FAN`. Si no detecta señal, avisa de error. Es una observación habitual, pero no demuestra por sí sola la causa: hay que comprobar la conexión.

## 3. Uso de IA

- **Herramienta y fecha:** Claude (Anthropic), 20/11/2026.
- **Para qué la usé:** para montar la estructura de este fichero a partir de mi presentación, proponer las preguntas del test y buscar fuentes técnicas.
- **Afirmación que decidí comprobar:** los datos del Noctua NH-D15 y de las CPU de la diapositiva 6.
- **Resultado:**
  - *Confirmadas:* 125 W de potencia base y 253 W de potencia máxima del i9-14900K (Intel); 170 W de TDP y 230 W de PPT del Ryzen 9 7950X; 6 tubos de calor, 1320 g, 24,6 dB(A) y MTTF de más de 150 000 h (Noctua).
  - *Corregida:* la presentación decía que el NH-D15 mide 165 mm; la ficha actual de Noctua indica **168 mm** con ventiladores (160 mm sin ellos).
  - *Matizada:* «más de 150 000 h» es el MTTF de los ventiladores (tiempo medio hasta el fallo), no la vida garantizada de todo el disipador. Pasarlo a «unos 17 años» es una cuenta, no un dato del fabricante.
- **No verificado con fuente técnica:** la cantidad de pasta («tamaño de un guisante») y los pasos de montaje, que se basan en lo que hicimos en el taller.
- **Datos personales:** no compartí datos personales ni información privada del centro.
