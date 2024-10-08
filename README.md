# EquipoExpo
Aqui mostramos la informacion de la exposicion 
```
source("https://raw.githubusercontent.com/GaliSuarez/EquipoExpo/refs/heads/main/Exposicion.qmd")

```
---
Title: "Exposición"
Author: "Angel Sinai Reyes Ferreyra <br>
         Yoselin Castañeda Ayllon <br>
         Dana Yuval Reyes González <br>
         Stephani Olvera Chávez <br>
         Guadalupe Montserrat Ramirez Mendoza <br>
         Oscar  Arciniega Patricio <br>
         Karla Galilea Suárez Esquivel <br>
         Sergio Díaz González <br><br>"
format: revealjs
editor: visual
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)

```

<style>
 p {
 text-align: justify;
}
</style>

## Certificados de depósito e inversiones a plazo en los bancos: conceptos, funcionamiento y tasas de interés

En el mundo financiero, existen múltiples opciones para hacer crecer nuestros ahorros de manera segura. Dos de las más comunes son los Certificados de Depósito (CD) y las Inversiones a Plazo. Ambas herramientas permiten obtener rendimientos a partir de nuestros depósitos en el banco, generando intereses que se acumulan con el tiempo. Sin embargo, para comprender su funcionamiento y evaluar cuál opción es la más adecuada para nuestras necesidades, es fundamental entender los conceptos básicos de tasas de interés y su aplicación en distintos contextos.

A continuación, se explica detalladamente qué son los Certificados de Depósito (CD) y las Inversiones a Plazo, cómo funcionan y cómo se aplican las tasas de interés activa y pasiva, utilizando la fórmula del interés simple para realizar cálculos.

## ¿Qué es un Certificado de Depósito (CD)?

Un Certificado de Depósito (CD) es un producto financiero ofrecido por los bancos que permite a los clientes depositar una cantidad de dinero por un periodo de tiempo determinado a cambio de un interés fijo. Los CD son considerados inversiones de bajo riesgo, ya que el capital está protegido y el retorno está asegurado por la entidad bancaria (Banco Central del país, 2020).

El inversor deposita una cantidad de dinero en el banco (valor actual, VA) por un periodo de tiempo específico (t), y el banco se compromete a devolver el valor del depósito más los intereses generados al finalizar el plazo (valor futuro, VF). La tasa de interés que el banco paga al inversor es conocida como la tasa pasiva, y se aplica utilizando la fórmula del interés simple.

## Inversiones a Plazo Fijo

Las Inversiones a Plazo Fijo son muy similares a los Certificados de Depósito. Implican el depósito de una cantidad de dinero por un tiempo específico a cambio de una tasa de interés. La principal diferencia radica en la flexibilidad que ofrecen algunos plazos fijos en cuanto a la posibilidad de renovación automática o retiro anticipado en ciertos casos, aunque esto puede implicar penalidades (Santander, 2023).

## Fórmula del Interés Simple

Para comprender el cálculo de los rendimientos generados por los Certificados de Depósito y las Inversiones a Plazo, se utiliza la fórmula del interés simple, que es:

Formula: $VF=VA\cdot[1+(r\cdot t)]$

Donde:

**VF**: es el valor futuro (lo que se recibirá al final del plazo).

**VA:** es el valor actual o principal (la cantidad que se deposita inicialmente).

**r:** es la tasa de interés (en forma decimal).

**t:** es el tiempo, expresado en años.

Esta fórmula nos permite calcular el valor futuro de una inversión cuando se aplica una tasa de interés simple, que es el tipo de interés más común en este tipo de productos financieros de corto plazo.

## **Ejemplo Práctico**

Imaginemos que invertimos \$10,000 en un CD a 1 año, con una tasa de interés anual del 5%.

**VA** = 10,000

**r** = 0.05 (5%)

**t** = 1 año

```{r}
library(htmltools)
library(ggplot2)
library(knitr)

# Definimos datos de entrada
VP=10000 # Valor presente
r=0.05  # Tasa de interes
t=1  # Tiempo

VF=VP*(1+(r*t)) # Calculamos el valor futuro conforme ecuación


HTML(paste("<span style='font-weight:bold; font-size:16px;'> El valor futuro del prestamo es:$", VF, "</span><br><br>"))
```

## Tasa Activa y Tasa Pasiva

### Tasa Activa

La tasa activa es el tipo de interés que los bancos cobran a sus clientes por los préstamos o créditos. Este interés es más alto que la tasa pasiva porque es una fuente de ingresos para los bancos. La tasa activa incluye, además de los costos operativos del banco, el riesgo de impago que el banco asume al prestar dinero (Banco Central del país, 2020).

### Tasa Pasiva

La tasa pasiva es la que los bancos pagan a los ahorradores o inversionistas por mantener su dinero depositado en la institución. Este es el tipo de interés que se aplica a los productos de inversión como los Certificados de Depósito o las cuentas de ahorro. Generalmente, la tasa pasiva es menor que la tasa activa, ya que el banco obtiene un margen de ganancia a partir de esta diferencia (Banco Central del país, 2020).

## **Aplicación de la Fórmula de Interés Simple Para el Certificado de Depósito:**

Supongamos que tienes un Certificado de Depósito de \$20,000 con una tasa pasiva anual del 4% y un plazo de 2 años. Usamos la fórmula del interés simple para calcular cuánto recibirás al final del plazo:

**VA** 20,000

**r** = 0.04

**t** = 2 añoร

```{r}
# Definimos datos de entrada
VP=20000 # Valor presente
r=0.04  # Tasa de interes
t=2  # Tiempo

VF=VP*(1+(r*t)) # Calculamos el valor futuro conforme ecuación

HTML(paste("<span style='font-weight:bold; font-size:16px;'> El valor futuro del prestamo es:$", VF, "</span><br><br>"))
```

En este caso, al cabo de dos años, recibirías \$21,600. Esto significa que habrías ganado \$1,600 en intereses por tu inversión.

## **Para un Préstamo:**

Ahora consideremos un préstamo de \$15,000 con una tasa activa del 7% anual, y un plazo de 3 años. Aquí, la fórmula de interés simple también es útil para calcular cuánto se deberá pagar al final del plazo.

**VA** = 15,000

**r** = 0.07

**t** = 3 años

```{r}
# Definimos datos de entrada
VP=15000 # Valor presente
r=0.07  # Tasa de interes
t=3  # Tiempo

VF=VP*(1+(r*t)) # Calculamos el valor futuro conforme ecuación

HTML(paste("<span style='font-weight:bold; font-size:16px;'> El valor futuro del prestamo es:$", VF, "</span><br><br>"))
```

Al final del plazo, el monto total a devolver sería de \$18,150, lo que incluye los intereses generados por el préstamo.

## Conclusión

Tanto los Certificados de Depósito como las Inversiones a Plazo son opciones seguras y predecibles para hacer crecer nuestro dinero, con la ventaja de que los rendimientos están garantizados. La diferencia entre la tasa activa y la tasa pasiva permite a los bancos generar ingresos, mientras que los ahorradores e inversionistas reciben un retorno por su dinero(Banco Central del país, 2020).

La fórmula de interés simple es una herramienta valiosa para calcular el rendimiento de estas inversiones y conocer el valor futuro de los fondos invertidos. Al analizar diferentes opciones, es importante tener en cuenta tanto las tasas de interés como los plazos, ya que estos factores impactarán directamente en los rendimientos obtenidos.

## Referencias

Banco Central del país. (2020). Informe de tasas de interés y condiciones financieras. Recuperado de http://www.bancocentral.org

Santander. (2023). Qué es una inversión a plazo fijo y cómo funciona. https://www.santander.com/finanzas/inversion-a- plazo
