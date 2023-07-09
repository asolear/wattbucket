---
title: 
    Distancia mínima entre filas de módulos
campos: ['Tecnico']
abstract: 
    Enlaces de interes
author: Q.Roman
header-includes: |
    \usepackage{multicol}
    \usepackage{fancyhdr}
    \pagestyle{fancy}
    \fancyhead{}
    \fancyhead[R]{1}
    \fancyfoot{}
    \fancyfoot[R]{Página \thepage}
...


<a href="../Distancia mínima entre filas de módulos.pdf" style="font-size: 40px;">   :fontawesome-solid-file-pdf:</a>,
<a href="../Distancia mínima entre filas de módulos.html" style="font-size: 40px;">    :fontawesome-solid-file-pen:</a>


ddd

## Disposicion de los modulos FV.

### Distancia mínima entre filas de módulos

Se utiliza el metodo del IDAE [^111] para la determinar la distancia mínima entre filas de módulos, tales que se garanticen al menos 4 horas de sol en torno al mediodía del solsticio de invierno.

$$
d_{min}=h \cdot 1/tan(61^o - \phi)
$$

donde:

- $d_{min}$: distancia mínima entre filas de módulos
- $h$: altura del obstáculo.
- $\phi$: latitud.
 


Para la Ubicacion en la latitud ($\phi$) de 40$^o$ representada en la figura

![Ubicacion Lat.:40 $^o$ ](assets/_mapa_pais.png)

se representan las medidas a tener en cuenta para determinar la separacion entre filas en la figura.


![Distancia mínima entre filas de módulos para $\alpha = 30 ^o$](assets/_fig_distanciaentrefilas_30.png)


En la tabla se muestan los distancias para las posibles inclinaciones, $\beta$,  con  modulos de 1m x 2m dispuestos horizontalmente.


Table: Distancia mínima entre filas de módulos

<!-- {pd.read_json(dddd.distanciaentrefilas).to_markdown()} -->

### Inclinación óptima. 

Se han calculado las medidas para inclinacion de la estructura comercial de $30^o$ mas cercana  a la inclinación óptimas  $\beta_{opt}$=30$^o$,  segun el metodo del IDAE [^2]  con el objetivo de  maximizar la producción anual.


## Sombras

## Generacion (PVGis)

![Distribucion de paneles FV](assets/_fig_generacioxincliancion.png)


## Estimacion del consumo

Se utiliza el metodo del IDAE [^3] para justificar la previsión, en cómputo anual, de la suma de la energía eléctrica consumida por parte del consumidor o consumidores asociados a la instalación de autoconsumo.


## Coste de la estructura. Estudio de cargas. (material y mano de obra).


Segun IDAE [^4],y basándonos en los criterios descritos en el CTE, no será necesario realizar estudios de carga, ya que los tejados y  cubiertas están obligados a soportar cargar mayores de las que implica una instalación de
autoconsumo,

se utilizarán contrapesos sobre la estructura soporte de
los módulos, para poder contrarrestar la acción del viento. Basándonos en el Código Técnico de la
Edificación para un viento de 130 km/h se establece como necesario un contrapeso a una
inclinación de 35º de 100 kg/m2.

### Coeficientes de presión externa en cubiertas con pendiente no superior a 5º
<!-- folleto de Sunfer -->
Según EUROCÓDIGO 1, en las zonas del extremo de la cubierta se
generan turbulencias y efectos adversos que amplifican el efecto del
viento.
<!-- recomentdaciones del idae a los ayuntamientos -->

<!-- contrapesos de primer curso de fotovoltaicas  y da las recomendaciones a los ayuntamientos -->

## Optimizacion


Luego, la función objetivo se ha modificado para incluir tanto la generación de energía como el costo del lastre. Los pesos generation_weight y cost_weight se utilizan para ajustar la importancia relativa de cada factor. Puedes ajustar estos pesos según tus necesidades y prioridades.





![Vista Satelite](assets/_satelite.png)



![Distribucion de paneles FV](assets/_geopandas_bg_map.png)


## Referencias

[^111]:[IDAE. Pliego de Condiciones Técnicas de Instalaciones Conectadas a Red. 5 Distancia mínima entre filas de módulos](https://www.idae.es/uploads/documentos/documentos_5654_FV_pliego_condiciones_tecnicas_instalaciones_conectadas_a_red_C20_Julio_2011_3498eaaf.pdf)

[^2]:[IDAE. Pliego de Condiciones Técnicas de Instalaciones Aisladas de Red. 3.2 Orientación e inclinación óptimas. Pérdidas por orientación e inclinación](https://www.idae.es/uploads/documentos/documentos_5654_FV_Pliego_aisladas_de_red_09_d5e0a327.pdf)

[^3]:[Justificacion de la energía eléctrica consumida.](https://www.idae.es/sites/default/files/documentos/ayudas_y_financiacion/RD477-2021_Autoconsumo_y_almacenamiento/2022_02_08-Informe_80%25_Consumo_RD477.pdf)

[^4]:[Guía de orientaciones a los municipios para el fomento del autoconsumo](https://www.idae.es/sites/default/files/documentos/publicaciones_idae/2022-12-02_Guia_Autoconsumo_Ayuntamientos_v.3.pdf)


[^5]:[IDAE. Oficina de Autoconsumo](https://www.idae.es/tecnologias/energias-renovables/oficina-de-autoconsumo)

