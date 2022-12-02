# conversionesLoopsDictSeriesDfs
Busco y descargo datos que necesiten ser tratados para formar un dataset.
https://www.worldbank.org/en/home
El fichero excel descargado, se pasa primero a un dataset que contiene una sola columa y 266 filas

## NOTA IMPORTANTE:
En realidad, bastaría con separar las columnas, como en el típico ejemplo, así:
df[['apellido','nombre']] = df['apellido;nombre'].str.split(";",expand=True)
Pero el objeto de este notebook es coger mucha destreza en la manipulación de datos, bucles...

El nombre de la columna es (es una sola columna):
'Country Name;Country Code;1960;1961;1962;1963;1964;1965;1966;1967;1968;1969;1970;1971;1972;1973;1974;1975;1976;1977;1978;1979;1980;1981;1982;1983;1984;1985;1986;1987;1988;1989;1990;1991;1992;1993;1994;1995;1996;1997;1998;1999;2000;2001;2002;2003;2004;2005;2006;2007;2008;2009;2010;2011;2012;2013;2014;2015;2016;2017;2018;2019;2020;2021'

Las filas son del tipo:
'Aruba;ABW;54208;55434;56234;56699;57029;57357;57702;58044;58377;58734;59070;59442;59849;60236;60527;60653;60586;60366;60102;59972;60097;60561;61341;62213;62826;63024;62645;61838;61072;61033;62152;64623;68240;72495;76705;80324;83211;85450;87280;89009;90866;92892;94992;97016;98744;100028;100830;101226;101362;101452;101665;102050;102565;103165;103776;104339;104865;105361;105846;106310;106766;107195'

Se realizan operaciones para aprender a tener soltura en la union de dataframes, bucles for con range, creacion de listas, series, diccionarios, dataframes (cada tipo en función del anterior...)
