# Tarea 2 - Taller de Python para Ciencia de Datos

Aplicación en Jupyter Notebook que muestre una historia del proceso de preparación de datos para su posterior análisis, utilizando las herramientas que provee el lenguaje de programación Python.

## Propiedad de los datos
**Proyecto:** Plataforma de diagnóstico e historización del confort térmico, consumo de energía y calidad de aire en hospitales públicos.

**Director Proyecto:** Dr. Hugo Garcés H.

**ID Proyecto:** 18IIP-BB-99513.

**Instituciones Ejecutoras:**
- Universidad Católica de la Santísima Concepción (Campus San Andrés, Concepción)
- Universidad Técnica Federico Santa María (Sede Concepción)

**Datos:** Nodo (MAC FD:BA:37) Pasillo 5to Piso - Sector Neonatología del Hospital Regional Guillermo Grant Benavente.

## Variables

**Atributos:**
|Atributo|Descripción|Indicador de Resultado|
|--------|--------|--------|
|Medición de confort térmico|Medición con nodo sensor de las variables que definen el confort térmico en un recinto: PMV: predicted mean vote y PPD: percentage persons dissastified|Presencia de medición de PMV y PPD en plataforma e interfaz de operación|
|Medición de calidad del aire interior|Medición con nodo sensor de las variables que determinan la calidad del aire interior: CO2, CO, NO2, COV (compuestos orgánicos volátiles); junto a mediciones de concentración de polvo grueso PM10 y polvo fino PM2.5|Presencia de medición de CO, CO2, NO2, COV, PM10, PM2.5 en plataforma e interfaz de operación|
|Registro historizado de mediciones|Mediciones almacenadas en base de datos con información asociada a tiempo en que la medición se ejecutó y ubicación en el recinto|Mediciones de las variables con formato {fecha-hora, valor}, factibles de ser analizadas con herramientas de series de tiempo|

**Diccionario:**
|Dato|Info|Unidad de medida|
|--------|--------|--------|
|id|ID del dato en la BD|U.A.|
|timestamp|Fecha y hora del dato capturado|Time|
|pmv|Voto Medio Previsto, estima la sensación térmica|U.A.|
|ppd|Porcentaje de Personas Insatisfechas|%|
|co2|Dioxido de Carbono|ppm|
|pm25|Material Particulado Fino|μg/m³|
|pm10|Material Particulado Grueso|μg/m³|
|temp|Temperatura|°C|
|hr|Humedad Relativa|%|
|voc|Compuestos Orgánicos Volatiles|ppm|
|co|Monoxido de Carbono|ppm|
|no2|Dioxido de Nitrogeno|ppm|
|c2h5ch|Etanol C2H5OH|ppm|
|idnodo|ID del nodo, correspondiente a su dirección MAC del dispositivo|U.A.|

|Unidad|Descripción|
|--------|--------|
|ppm|Particulas por Millón|
|%|Porcentaje|
|Time|Instante de tiempo|
|μg/m³|Microgramos por metro cúbico|
|°C|Grados Celsius|
|U.A.|Unidad Adimensional|


## Instalación
Descomprimir la aplicacion y abrir una terminal cambiando el directorio de trabajo actual a la ubicación en donde se encuentra la aplicación.
```bash
cd Tarea2-TPCD
```

O clonar el repositorio a través del comando [git clone](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository).

```bash
git clone https://github.com/victorex/Tarea2-TPCD.git

cd Tarea2-TPCD
```

## Importante
Al momento de ejecutar la aplicación se deben ingresar el siguiente parámetro necesario para el funcionamiento de esta:
- Nombre del libro a trabajar (éste debe estar almacenado en el directorio ```"../Libros_txt_utf-8"```).

## Ejemplos de ejecución

```properties
 python Main.py El_Arbol_De_La_Colina
 python Main.py El_Caos_Reptante
 python Main.py En_El_Mar_Remoto
```

## Versión python

    Python 3.8
