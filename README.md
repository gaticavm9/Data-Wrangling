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

Análisis de Confort Térmico y Calidad del aire, mediante la definicion de confort térmico de la norma ISO 7730 y la norma ASHRAE 55-2013. El confort térmico es calculado mediante el Método Fanger.
 
**Atributos:**
|Atributo|Descripción|Indicador de Resultado|
|--------|--------|--------|
|Medición de confort térmico|Medición con nodo sensor de las variables que definen el confort térmico en un recinto: PMV: predicted mean vote y PPD: percentage persons dissastified|Presencia de medición de PMV y PPD en plataforma e interfaz de operación|
|Medición de calidad del aire interior|Medición con nodo sensor de las variables que determinan la calidad del aire interior: CO2, CO, NO2, COV (compuestos orgánicos volátiles); junto a mediciones de concentración de polvo grueso PM10 y polvo fino PM2.5|Presencia de medición de CO, CO2, NO2, COV, PM10, PM2.5 en plataforma e interfaz de operación|
|Registro historizado de mediciones|Mediciones almacenadas en base de datos con información asociada a tiempo en que la medición se ejecutó y ubicación en el recinto|Mediciones de las variables con formato {fecha-hora, valor}, factibles de ser analizadas con herramientas de series de tiempo|

**Índices:**
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

**Diccionario:**
|Unidad|Descripción|
|--------|--------|
|ppm|Particulas por Millón|
|%|Porcentaje|
|Time|Instante de tiempo|
|μg/m³|Microgramos por metro cúbico|
|°C|Grados Celsius|
|U.A.|Unidad Adimensional|


## Instalación
Es necesario tener instalado Jupyter Notebooks en Visual Studio Code. Luego en una terminal Powershell o CMD en Windows se debe instalar las librerías de Pandas y MatPlotLib.
- Pandas:
```bash
pip install pandas
```

- MatPlotLib:
```bash
py -m pip install matplotlib
```

Descomprimir la aplicacion y abrir una terminal cambiando el directorio de trabajo actual a la ubicación en donde se encuentra la aplicación.
```bash
cd Tarea2-TPCD
```

O clonar el repositorio a través del comando [git clone](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository).

```bash
git clone https://github.com/victorex/Tarea2-TPCD.git

cd Tarea2-TPCD
```

## Ejecución
Al abrir la carpeta contenedora en Visual Studio Code, abrir el archivo ```Main.ipynb```, seleccionandolo con doble clic en la vista de carpetas y archivos en el costado izquierdo. Luego en el panel superior, al centro, presionar en **Ejecutar todo**.

## Versión Python

    Python 3.8
