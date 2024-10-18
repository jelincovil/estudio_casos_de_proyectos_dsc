# Estudio de casos en Data Science con aplicaciones a datos Industriales, Ciencias de la Salud, Medio Ambiente y Big-Data.

Este repositorio contiene casos de aplicaciones de Data Science para ser empleado en cursos de post-grado.
Son empleados los lenguajes R y Python.

## Aplicación de la Teoria de Ondaletas a la estimación y comparación de datos funcionales


## Modelos de ranking para datos industriales

### Caso de estudio: lealtad de clientes a las marcas

## Aprendizaje en linea
### Caso de estudio: Asesoría de experto

## Sistema de recomendaciones
### Caso de estudio: Analisis de semantica Latente.

## Clasificación

### Caso de estudio: Control de calidad

## Aplicaciones de Modelos Aditivos Generalizados a ensayos clinicos

# Ensayos Controlados Aleatorizados (Randomized Control Trials) 

Los **RCTs** son una técnica experimental que consiste en asignar aleatoriamente a los participantes de un estudio a dos grupos: **grupo de tratamiento** y **grupo de control**. La aleatorización asegura que, excepto por el tratamiento, ambos grupos sean comparables, lo que permite atribuir cualquier diferencia en el resultado observado a la intervención o tratamiento aplicado.

**Ejemplo**: Si una empresa quiere medir el efecto de una nueva campaña de marketing en las ventas, dividiría a sus clientes en dos grupos de manera aleatoria: un grupo que recibe la campaña (tratamiento) y otro que no (control). Luego, comparan las ventas entre ambos grupos para ver si la campaña tuvo un impacto significativo.

---

# Difference in Differences (Dif-in-Dif o DiD)

La técnica **Difference in Differences** se usa para evaluar el impacto de una intervención (tratamiento) en un grupo tratado comparándolo con un grupo no tratado. Lo que hace es medir la **diferencia en el resultado** entre ambos grupos antes y después de la intervención, y **resta** la diferencia que ya existía entre los dos grupos antes del tratamiento. Esto ayuda a aislar el efecto de la intervención.

**Ejemplo**: Un gobierno implementa un nuevo programa educativo en ciertas escuelas. Para evaluar el impacto, comparas las notas de los estudiantes **antes y después** de la implementación del programa tanto en las escuelas que participaron (tratadas) como en aquellas que no participaron (control). La técnica DiD mide cómo cambió el rendimiento de los estudiantes en las escuelas tratadas en comparación con las no tratadas, aislando el efecto del programa.

---

# Control Sintético (Synthetic Control)

El método de **control sintético** crea un grupo de control artificial o "sintético" a partir de una combinación ponderada de datos observacionales de otras unidades que no recibieron el tratamiento. Esta técnica es útil cuando solo una unidad (por ejemplo, un país o una empresa) recibe el tratamiento, y no hay un grupo de control natural.

**Ejemplo**: Imagina que un país cambia su política fiscal y quieres medir el impacto en el crecimiento económico. Dado que no hay otros países con políticas idénticas para comparar, el control sintético combina datos de varios países similares (en cuanto a crecimiento económico antes del cambio) para crear un "país sintético" contra el cual puedas comparar los efectos de la política.

---

# Variables Instrumentales (Instrumental Variables)

La técnica de **Variables Instrumentales** se usa cuando hay un problema de **endogeneidad** (es decir, cuando una variable explicativa está correlacionada con los errores del modelo o con variables omitidas, lo que sesga los resultados). Las **variables instrumentales** son variables que están correlacionadas con la variable independiente (la que queremos estudiar), pero no lo están con el error del modelo ni afectan directamente el resultado. Esto permite estimar el efecto causal de la variable de interés.

**Ejemplo**: Si quieres estudiar el efecto de la educación en los ingresos, pero crees que las personas con mayor habilidad innata (que no puedes medir directamente) tienden a estudiar más, la variable "educación" estaría sesgada. Podrías usar la **distancia a las escuelas** como una variable instrumental, asumiendo que las personas más cerca de escuelas tienen más años de educación, pero su proximidad a una escuela no afecta directamente sus ingresos, excepto a través de la educación.

---

# Propensity Score Matching (PSM)**

**Propensity Score Matching** es una técnica que se utiliza para **emparejar** unidades tratadas y no tratadas que tienen características similares, lo que reduce el sesgo de selección. Se calcula una **probabilidad de recibir el tratamiento** (propensity score) basada en las características observadas de cada individuo. Luego, se emparejan individuos tratados y no tratados con puntajes similares para comparar el impacto del tratamiento.

**Ejemplo**: Si estás evaluando el impacto de un programa de subsidios a empresas pequeñas, el propensity score matching encontraría empresas similares en cuanto a tamaño, sector, ingresos, etc., para que puedas comparar empresas que recibieron el subsidio con aquellas que no lo recibieron, y así medir el efecto del subsidio de manera más precisa.

---


## Referencias

- Introduction to Statistics and Data Analysis – A Case-Based Approach. (Link)[https://bookdown.org/conradziller/introstatistics/]
- The Big Book of Data Science Use Cases. (Link)[]
- Data Science in R. A Case Studies Approach to Computational Reasoning and Problem Solving. (Link)[https://www.routledge.com/Data-Science-in-R-A-Case-Studies-Approach-to-Computational-Reasoning-and-Problem-Solving/Nolan-Lang/p/book/9781482234817]
  
 
