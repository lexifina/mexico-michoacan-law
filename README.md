# Michoacán: law history in git

The law of the State of Michoacán (Estado Libre y Soberano de Michoacán de Ocampo, Mexico) as a git history: one file per article, one commit per publication that changed it, dated the day it took effect, with the decree as the commit's author. `git blame` names the decree behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `mx-mic/`. Mexico's federal law is in [lexifina/mexico-law](https://github.com/lexifina/mexico-law).

The text is in Spanish, exactly as the source prints it.

## What this repository holds

174 ordenamientos with 1030 versions so far: the constitution first, then the codes and laws in force, added in parts. Regulations, decrees and repealed laws are not included yet.

| Folder | Ordenamiento | Versions | History |
| --- | --- | ---: | --- |
| `constitucion-politica/` | CONSTITUCION POLITICA DEL ESTADO LIBRE Y SOBERANO DE MICHOACAN DE OCAMPO | 134 | as first published, then each reform: 10 February 1918 to 26 March 2026 |
| `codigo-civil/` | CODIGO CIVIL PARA EL ESTADO DE MICHOACAN DE OCAMPO | 18 | as first published, then each reform: 8 September 2008 to 28 April 2026 |
| `codigo-de-desarrollo-urbano/` | CODIGO DE DESARROLLO URBANO DEL ESTADO DE MICHOACAN DE OCAMPO | 26 | as first published, then each reform: 27 December 2007 to 11 August 2026 |
| `codigo-de-justicia-administrativa/` | CODIGO DE JUSTICIA ADMINISTRATIVA DEL ESTADO DE MICHOACAN DE OCAMPO | 14 | as first published, then each reform: 2 January 2008 to 15 February 2025 |
| `codigo-de-procedimientos-civiles/` | CODIGO DE PROCEDIMIENTOS CIVILES PARA EL ESTADO DE MICHOACAN DE OCAMPO | 11 | as first published, then each reform: 8 September 2008 to 27 September 2022 |
| `codigo-electoral/` | CODIGO ELECTORAL DEL ESTADO DE MICHOACAN DE OCAMPO | 37 | as first published, then each reform: 30 June 2014 to 30 May 2026 |
| `codigo-familiar/` | CODIGO FAMILIAR PARA EL ESTADO DE MICHOACAN DE OCAMPO | 22 | as first published, then each reform: 3 October 2015 to 5 May 2026 |
| `codigo-fiscal/` | CODIGO FISCAL DEL ESTADO DE MICHOACAN DE OCAMPO | 23 | as first published, then each reform: 28 February 1992 to 1 January 2025 |
| `codigo-fiscal-municipal/` | CODIGO FISCAL MUNICIPAL DEL ESTADO DE MICHOACAN DE OCAMPO | 7 | as first published, then each reform: 26 August 1997 to 27 May 2026 |
| `codigo-penal/` | CODIGO PENAL PARA EL ESTADO DE MICHOACAN DE OCAMPO | 69 | as first published, then each reform: 20 December 2014 to 19 August 2026 |
| `ley-contra-las-adicciones-en-el-estado-de-michoacan/` | LEY CONTRA LAS ADICCIONES EN EL ESTADO DE MICHOACAN | 3 | as first published, then each reform: 12 July 2022 to 25 July 2026 |
| `ley-de-adopcion-y-acogimiento-familiar/` | LEY DE ADOPCION Y ACOGIMIENTO FAMILIAR DEL ESTADO DE MICHOACAN DE OCAMPO (ANTES: LEY DE ADOPCION DEL ESTADO DE MICHOACAN DE OCAMPO) | 7 | as first published, then each reform: 2 July 2013 to 4 March 2023 |
| `ley-de-adquisiciones-arrendamientos-y-prestacion-de-servicio/` | LEY DE ADQUISICIONES, ARRENDAMIENTOS Y PRESTACION DE SERVICIOS RELACIONADOS CON BIENES MUEBLES E INMUEBLES DEL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 12 June 1998 to 6 November 2020 |
| `ley-de-agricultura-urbana-y-periurbana/` | LEY DE AGRICULTURA URBANA Y PERIURBANA DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 14 December 2017 to 8 December 2023 |
| `ley-de-amnistia/` | LEY DE AMNISTIA DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 17 May 1981 to 29 August 2019 |
| `ley-de-arancel-de-abogados-en-el-estado-de-michoacan-de-ocam/` | LEY DE ARANCEL DE ABOGADOS EN EL ESTADO DE MICHOACAN DE OCAMPO | 1 | as first published: 28 August 1953 |
| `ley-de-arancel-de-notarios/` | LEY DE ARANCEL DE NOTARIOS | 1 | as first published: 20 August 1974 |
| `ley-de-archivos-administrativos-e-historicos/` | LEY DE ARCHIVOS ADMINISTRATIVOS E HISTORICOS DEL ESTADO DE MICHOACAN DE OCAMPO Y SUS MUNICIPIOS | 1 | as first published: 4 March 2004 |
| `ley-de-asistencia-social/` | LEY DE ASISTENCIA SOCIAL DEL ESTADO DE MICHOACAN DE OCAMPO | 18 | as first published, then each reform: 15 May 1987 to 5 June 2026 |
| `ley-de-asociaciones-publico-privadas/` | LEY DE ASOCIACIONES PUBLICO PRIVADAS PARA EL ESTADO DE MICHOACAN DE OCAMPO | 3 | as first published, then each reform: 1 October 2015 to 30 December 2016 |
| `ley-de-atencion-a-victimas/` | LEY DE ATENCION A VICTIMAS PARA EL ESTADO DE MICHOACAN DE OCAMPO | 9 | as first published, then each reform: 21 May 2015 to 27 July 2024 |
| `ley-de-bibliotecas/` | LEY DE BIBLIOTECAS PARA EL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 20 July 2018 to 27 May 2026 |
| `ley-de-cambio-climatico/` | LEY DE CAMBIO CLIMATICO DEL ESTADO DE MICHOACAN DE OCAMPO | 8 | as first published, then each reform: 22 January 2014 to 3 September 2025 |
| `ley-de-caminos-y-puentes/` | LEY DE CAMINOS Y PUENTES DEL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 15 June 2004 to 11 August 2026 |
| `ley-de-ciencia-tecnologia-e-innovacion/` | LEY DE CIENCIA, TECNOLOGIA E INNOVACION DEL ESTADO DE MICHOACAN | 6 | as first published, then each reform: 8 February 2012 to 26 September 2023 |
| `ley-de-comunicaciones-y-transportes/` | LEY DE COMUNICACIONES Y TRANSPORTES DEL ESTADO DE MICHOACAN | 5 | as first published, then each reform: 22 July 1982 to 3 June 2023 |
| `ley-de-cooperacion-de-los-productores-de-limon/` | LEY DE COOPERACION DE LOS PRODUCTORES DE LIMON DEL ESTADO DE MICHOACAN PARA EL FIDEICOMISO PARA REALIZAR ESTUDIOS E INVESTIGACIONES DE CARACTER TECNICO | 1 | as first published: 13 August 1974 |
| `ley-de-coordinacion-fiscal/` | LEY DE COORDINACION FISCAL DEL ESTADO DE MICHOACAN DE OCAMPO | 15 | as first published, then each reform: 1 January 2009 to 1 January 2025 |
| `ley-de-cultura-fisica-y-deporte/` | LEY DE CULTURA FISICA Y DEPORTE DEL ESTADO DE MICHOACAN DE OCAMPO | 12 | as first published, then each reform: 17 February 2004 to 19 August 2026 |
| `ley-de-derechos-el-bienestar-y-proteccion-de-los-animales-en/` | LEY DE DERECHOS, EL BIENESTAR Y PROTECCION DE LOS ANIMALES EN EL ESTADO DE MICHOACAN DE OCAMPO -- ANTES LEY DE DERECHOS Y PROTECCION PARA LOS ANIMALES EN EL ESTADO DE MICHOACAN DE OCAMPO -- | 12 | as first published, then each reform: 3 April 2018 to 13 August 2026 |
| `ley-de-desarrollo-cultural/` | LEY DE DESARROLLO CULTURAL PARA EL ESTADO DE MICHOACAN DE OCAMPO | 4 | as first published, then each reform: 27 September 2007 to 19 February 2022 |
| `ley-de-desarrollo-economico/` | LEY DE DESARROLLO ECONOMICO DEL ESTADO DE MICHOACAN DE OCAMPO | 7 | as first published, then each reform: 4 December 2014 to 11 August 2026 |
| `ley-de-desarrollo-forestal-sustentable/` | LEY DE DESARROLLO FORESTAL SUSTENTABLE DEL ESTADO DE MICHOACAN | 9 | as first published, then each reform: 25 November 2004 to 1 February 2025 |
| `ley-de-desarrollo-rural-integral-sustentable/` | LEY DE DESARROLLO RURAL INTEGRAL SUSTENTABLE DEL ESTADO DE MICHOACAN DE OCAMPO | 14 | as first published, then each reform: 19 January 2006 to 26 September 2023 |
| `ley-de-deuda-publica/` | LEY DE DEUDA PUBLICA PARA EL ESTADO DE MICHOACAN DE OCAMPO Y SUS MUNICIPIOS | 2 | as first published, then each reform: 6 August 2016 to 29 December 2017 |
| `ley-de-educacion/` | LEY DE EDUCACION DEL ESTADO DE MICHOACAN DE OCAMPO | 25 | as first published, then each reform: 30 May 2020 to 19 August 2026 |
| `ley-de-ejecucion-de-sanciones-penales/` | LEY DE EJECUCION DE SANCIONES PENALES DEL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 15 June 2011 to 29 August 2019 |
| `ley-de-entidades-paraestatales/` | LEY DE ENTIDADES PARAESTATALES DEL ESTADO DE MICHOACAN | 5 | oldest version available, then each reform: 31 March 1992 to 12 August 2025 |
| `ley-de-expropiacion/` | LEY DE EXPROPIACION DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 1 September 2007 to 22 April 2015 |
| `ley-de-financiamiento-rural/` | LEY DE FINANCIAMIENTO RURAL PARA EL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 13 February 2008 to 27 June 2023 |
| `ley-de-firma-electronica-certificada/` | LEY DE FIRMA ELECTRONICA CERTIFICADA DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 1 October 2015 to 30 December 2016 |
| `ley-de-fiscalizacion-superior-y-rendicion-de-cuentas/` | LEY DE FISCALIZACION SUPERIOR Y RENDICION DE CUENTAS DEL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 1 April 2019 to 16 November 2023 |
| `ley-de-fomento-a-la-lectura-y-el-libro/` | LEY DE FOMENTO A LA LECTURA Y EL LIBRO DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 23 January 2008 to 24 March 2026 |
| `ley-de-fomento-al-primer-empleo-y-a-la-primera-empresa/` | LEY DE FOMENTO AL PRIMER EMPLEO Y A LA PRIMERA EMPRESA PARA EL ESTADO DE MICHOACAN DE OCAMPO Y SUS MUNICIPIOS | 3 | as first published, then each reform: 12 November 2017 to 24 December 2020 |
| `ley-de-fomento-apicola/` | LEY DE FOMENTO APICOLA DEL ESTADO DE MICHOACAN DE OCAMPO | 4 | as first published, then each reform: 15 May 2004 to 19 November 2022 |
| `ley-de-fomento-y-desarrollo-artesanal/` | LEY DE FOMENTO Y DESARROLLO ARTESANAL DEL ESTADO DE MICHOACAN DE OCAMPO | 4 | as first published, then each reform: 22 May 2015 to 8 May 2024 |
| `ley-de-fomento-y-fortalecimiento-a-las-actividades-realizada/` | LEY DE FOMENTO Y FORTALECIMIENTO A LAS ACTIVIDADES REALIZADAS POR ORGANIZACIONES DE LA SOCIEDAD CIVIL EN EL ESTADO DE MICHOACAN DE OCAMPO | 3 | as first published, then each reform: 30 September 2015 to 5 December 2020 |
| `ley-de-fomento-y-proteccion-del-maiz-criollo-como-patrimonio/` | LEY DE FOMENTO Y PROTECCION DEL MAIZ CRIOLLO COMO PATRIMONIO ALIMENTARIO DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 2 March 2011 to 8 December 2023 |
| `ley-de-fondos-de-aseguramiento-agropecuario-y-rural/` | LEY DE FONDOS DE ASEGURAMIENTO AGROPECUARIO Y RURAL PARA EL ESTADO DE MICHOACAN DE OCAMPO | 1 | as first published: 23 April 2015 |
| `ley-de-ganaderia/` | LEY DE GANADERIA DEL ESTADO DE MICHOACAN DE OCAMPO | 7 | as first published, then each reform: 3 March 2007 to 23 May 2024 |
| `ley-de-gobierno-digital/` | LEY DE GOBIERNO DIGITAL DEL ESTADO DE MICHOACAN DE OCAMPO | 1 | as first published: 5 October 2021 |
| `ley-de-hacienda/` | LEY DE HACIENDA DEL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 1 January 2022 to 26 March 2026 |
| `ley-de-hacienda-municipal/` | LEY DE HACIENDA MUNICIPAL DEL ESTADO DE MICHOACAN DE OCAMPO | 10 | as first published, then each reform: 1 January 2015 to 11 August 2026 |
| `ley-de-indulto/` | LEY DE INDULTO PARA EL ESTADO DE MICHOACAN | 1 | as first published: 14 April 1989 |
| `ley-de-ingresos/` | LEY DE INGRESOS DEL ESTADO DE MICHOACAN DE OCAMPO PARA EL EJERCICIO FISCAL 2026 | 2 | as first published, then each reform: 1 January 2026 to 2 February 2026 |
| `ley-de-ingresos-del-municipio-de-acuitzio-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE ACUITZIO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-aguililla-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE AGUILILLA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-angangueo-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE ANGANGUEO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-apatzingan-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE APATZINGAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-aquila-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE AQUILA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-arteaga-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE ARTEAGA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-brisenas-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE BRISEÑAS, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-buenavista-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE BUENAVISTA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-caracuaro-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE CARACUARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-charo-michoacan-para-el-eje/` | LEY DE INGRESOS DEL MUNICIPIO DE CHARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-chavinda-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE CHAVINDA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-cheran-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE CHERAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-chilchota-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE CHILCHOTA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-chinicuila-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE CHINICUILA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-chucandiro-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE CHUCANDIRO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-churintzio-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE CHURINTZIO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-coahuayana-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE COAHUAYANA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-coalcoman-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE COALCOMAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-cojumatlan-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE COJUMATLAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-contepec-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE CONTEPEC, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-copandaro-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE COPANDARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-cotija-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE COTIJA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-cuitzeo-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE CUITZEO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-ecuandureo-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE ECUANDUREO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-epitacio-huerta-michoacan-p/` | LEY DE INGRESOS DEL MUNICIPIO DE EPITACIO HUERTA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-gabriel-zamora-michoacan-pa/` | LEY DE INGRESOS DEL MUNICIPIO DE GABRIEL ZAMORA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-hidalgo-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE HIDALGO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-huaniqueo-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE HUANIQUEO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2025 | 1 | as first published: 1 January 2025 |
| `ley-de-ingresos-del-municipio-de-huaniqueo-michoacan-para-el-2/` | LEY DE INGRESOS DEL MUNICIPIO DE HUANIQUEO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-huetamo-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE HUETAMO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-huiramba-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE HUIRAMBA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-indaparapeo-michoacan-para/` | LEY DE INGRESOS DEL MUNICIPIO DE INDAPARAPEO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-irimbo-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE IRIMBO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-ixtlan-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE IXTLAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-jacona-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE JACONA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-jimenez-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE JIMENEZ, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-jiquilpan-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE JIQUILPAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-jose-sixto-verduzco-michoac/` | LEY DE INGRESOS DEL MUNICIPIO DE JOSE SIXTO VERDUZCO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-juarez-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE JUAREZ, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-la-huacana-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE LA HUACANA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-la-piedad-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE LA PIEDAD, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-lagunillas-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE LAGUNILLAS, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-lazaro-cardenas-michoacan-p/` | LEY DE INGRESOS DEL MUNICIPIO DE LAZARO CARDENAS, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 2 | as first published, then each reform: 1 January 2026 to 21 January 2026 |
| `ley-de-ingresos-del-municipio-de-los-reyes-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE LOS REYES, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-madero-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE MADERO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-maravatio-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE MARAVATIO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-marcos-castellanos-michoaca/` | LEY DE INGRESOS DEL MUNICIPIO DE MARCOS CASTELLANOS, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-morelia-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE MORELIA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-morelos-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE MORELOS, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-mugica-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE MUGICA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-nahuatzen-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE NAHUATZEN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-nocupetaro-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE NOCUPETARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-nuevo-parangaricutiro-micho/` | LEY DE INGRESOS DEL MUNICIPIO DE NUEVO PARANGARICUTIRO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-nuevo-urecho-michoacan-para/` | LEY DE INGRESOS DEL MUNICIPIO DE NUEVO URECHO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-numaran-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE NUMARAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-pajacuaran-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE PAJACUARAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-panindicuaro-michoacan-para/` | LEY DE INGRESOS DEL MUNICIPIO DE PANINDICUARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-paracho-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE PARACHO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-patzcuaro-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE PATZCUARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-penjamillo-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE PENJAMILLO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-periban-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE PERIBAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-purepero-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE PUREPERO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-puruandiro-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE PURUANDIRO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-querendaro-michoacan-para-e/` | LEY DE INGRESOS DEL MUNICIPIO DE QUERENDARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-quiroga-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE QUIROGA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-sahuayo-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE SAHUAYO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-salvador-escalante-michoaca/` | LEY DE INGRESOS DEL MUNICIPIO DE SALVADOR ESCALANTE, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 2 | as first published, then each reform: 1 January 2026 to 21 January 2026 |
| `ley-de-ingresos-del-municipio-de-santa-ana-maya-michoacan-pa/` | LEY DE INGRESOS DEL MUNICIPIO DE SANTA ANA MAYA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-tancitaro-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE TANCITARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-tlalpujahua-michoacan-para/` | LEY DE INGRESOS DEL MUNICIPIO DE TLALPUJAHUA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-tocumbo-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE TOCUMBO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-turicato-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE TURICATO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 2 | as first published, then each reform: 1 January 2026 to 21 January 2026 |
| `ley-de-ingresos-del-municipio-de-tuxpan-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE TUXPAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-tzintzuntzan-michoacan-para/` | LEY DE INGRESOS DEL MUNICIPIO DE TZINTZUNTZAN, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-tzitzio-michoacan-para-el-e/` | LEY DE INGRESOS DEL MUNICIPIO DE TZITZIO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-venustiano-carranza-michoac/` | LEY DE INGRESOS DEL MUNICIPIO DE VENUSTIANO CARRANZA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-yurecuaro-michoacan-para-el/` | LEY DE INGRESOS DEL MUNICIPIO DE YURECUARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-zacapu-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE ZACAPU, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-zamora-michoacan-para-el-ej/` | LEY DE INGRESOS DEL MUNICIPIO DE ZAMORA, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos-del-municipio-de-zinapecuaro-michoacan-para/` | LEY DE INGRESOS DEL MUNICIPIO DE ZINAPECUARO, MICHOACAN, PARA EL EJERCICIO FISCAL DEL AÑO 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-instituciones-de-asistencia-privada/` | LEY DE INSTITUCIONES DE ASISTENCIA PRIVADA DEL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 10 June 2004 to 29 August 2019 |
| `ley-de-justicia-alternativa-y-restaurativa/` | LEY DE JUSTICIA ALTERNATIVA Y RESTAURATIVA DEL ESTADO DE MICHOACAN | 5 | as first published, then each reform: 22 January 2014 to 1 July 2020 |
| `ley-de-justicia-civica/` | LEY DE JUSTICIA CIVICA DEL ESTADO DE MICHOACAN DE OCAMPO | 1 | as first published: 28 February 2024 |
| `ley-de-justicia-comunal/` | LEY DE JUSTICIA COMUNAL DEL ESTADO DE MICHOACAN DE OCAMPO | 3 | as first published, then each reform: 9 May 2007 to 29 August 2019 |
| `ley-de-justicia-en-materia-electoral-y-de-participacion-ciud/` | LEY DE JUSTICIA EN MATERIA ELECTORAL Y DE PARTICIPACION CIUDADANA DEL ESTADO DE MICHOACAN DE OCAMPO | 7 | as first published, then each reform: 30 June 2014 to 28 May 2026 |
| `ley-de-la-atencion-y-proteccion-a-personas-con-la-condicion/` | LEY DE LA ATENCION Y PROTECCION A PERSONAS CON LA CONDICION DEL ESPECTRO AUTISTA PARA EL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 21 July 2017 to 5 December 2020 |
| `ley-de-la-comision-estatal-de-los-derechos-humanos-de-michoa/` | LEY DE LA COMISION ESTATAL DE LOS DERECHOS HUMANOS DE MICHOACAN DE OCAMPO | 13 | as first published, then each reform: 22 November 2014 to 19 August 2026 |
| `ley-de-la-comision-estatal-para-la-proteccion-contra-riesgos/` | LEY DE LA COMISION ESTATAL PARA LA PROTECCION CONTRA RIESGOS SANITARIOS DE MICHOACAN | 2 | as first published, then each reform: 31 May 2014 to 31 March 2023 |
| `ley-de-la-defensoria-publica/` | LEY DE LA DEFENSORIA PUBLICA DEL ESTADO DE MICHOACAN | 3 | as first published, then each reform: 1 December 2013 to 29 August 2019 |
| `ley-de-la-funcion-registral-y-catastral/` | LEY DE LA FUNCION REGISTRAL Y CATASTRAL DEL ESTADO DE MICHOACAN DE OCAMPO | 3 | as first published, then each reform: 29 January 2021 to 10 January 2026 |
| `ley-de-los-derechos-de-ninas-ninos-y-adolescentes/` | LEY DE LOS DERECHOS DE NIÑAS, NIÑOS Y ADOLESCENTES DEL ESTADO DE MICHOACAN DE OCAMPO | 43 | as first published, then each reform: 31 August 2015 to 19 August 2026 |
| `ley-de-los-jovenes/` | LEY DE LOS JOVENES DEL ESTADO DE MICHOACAN DE OCAMPO | 8 | as first published, then each reform: 25 May 2011 to 16 June 2026 |
| `ley-de-los-trabajadores-al-servicio/` | LEY DE LOS TRABAJADORES AL SERVICIO DEL ESTADO DE MICHOACAN DE OCAMPO Y DE SUS MUNICIPIOS | 25 | as first published, then each reform: 9 August 1983 to 13 February 2026 |
| `ley-de-mecanismos-de-participacion-ciudadana/` | LEY DE MECANISMOS DE PARTICIPACION CIUDADANA DEL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 9 September 2015 to 3 June 2023 |
| `ley-de-mejora-regulatoria/` | LEY DE MEJORA REGULATORIA DEL ESTADO DE MICHOACAN DE OCAMPO Y SUS MUNICIPIOS | 2 | as first published, then each reform: 20 February 2018 to 7 September 2023 |
| `ley-de-movilidad-y-seguridad-vial/` | LEY DE MOVILIDAD Y SEGURIDAD VIAL DEL ESTADO DE MICHOACAN DE OCAMPO | 13 | as first published, then each reform: 3 June 2023 to 19 August 2026 |
| `ley-de-obra-publica-y-servicios-relacionados-con-la-misma/` | LEY DE OBRA PUBLICA Y SERVICIOS RELACIONADOS CON LA MISMA PARA EL ESTADO DE MICHOACAN DE OCAMPO Y SUS MUNICIPIOS -ANTES LEY DE OBRAS PUBLICAS DEL ESTADO DE MICHOACAN DE OCAMPO Y DE SUS MUNICIPIOS- | 11 | as first published, then each reform: 8 December 1998 to 23 December 2022 |
| `ley-de-organizaciones-agricolas/` | LEY DE ORGANIZACIONES AGRICOLAS DEL ESTADO DE MICHOACAN | 4 | as first published, then each reform: 27 March 1997 to 5 July 2022 |
| `ley-de-pensiones-civiles/` | LEY DE PENSIONES CIVILES PARA EL ESTADO DE MICHOACAN | 7 | as first published, then each reform: 11 May 1980 to 6 October 2018 |
| `ley-de-pesca-y-acuacultura-sustentables/` | LEY DE PESCA Y ACUACULTURA SUSTENTABLES PARA EL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 24 June 2015 to 30 December 2016 |
| `ley-de-planeacion/` | LEY DE PLANEACION DEL ESTADO DE MICHOACAN DE OCAMPO | 4 | as first published, then each reform: 18 April 1989 to 28 June 2014 |
| `ley-de-planeacion-hacendaria-presupuesto-gasto-publico-y-con/` | LEY DE PLANEACION HACENDARIA, PRESUPUESTO, GASTO PUBLICO Y CONTABILIDAD GUBERNAMENTAL DEL ESTADO DE MICHOACAN DE OCAMPO | 12 | as first published, then each reform: 21 March 2014 to 19 August 2026 |
| `ley-de-productos-organicos/` | LEY DE PRODUCTOS ORGANICOS PARA EL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 4 December 2014 to 30 December 2016 |
| `ley-de-profesiones/` | LEY DE PROFESIONES DEL ESTADO DE MICHOACAN DE OCAMPO | 3 | as first published, then each reform: 21 January 2020 to 15 August 2026 |
| `ley-de-proteccion-civil/` | LEY DE PROTECCION CIVIL DEL ESTADO DE MICHOACAN DE OCAMPO | 7 | as first published, then each reform: 26 November 2014 to 3 September 2025 |
| `ley-de-proteccion-de-datos-personales-en-posesion-de-sujetos/` | LEY DE PROTECCION DE DATOS PERSONALES EN POSESION DE SUJETOS OBLIGADOS DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 14 November 2017 to 27 May 2026 |
| `ley-de-proteccion-de-los-no-fumadores/` | LEY DE PROTECCION DE LOS NO FUMADORES DEL ESTADO DE MICHOACAN DE OCAMPO | 3 | as first published, then each reform: 8 November 2008 to 12 May 2018 |
| `ley-de-proteccion-integral-a-las-personas-adultas-mayores/` | LEY DE PROTECCION INTEGRAL A LAS PERSONAS ADULTAS MAYORES DEL ESTADO DE MICHOACAN DE OCAMPO | 9 | as first published, then each reform: 25 January 2013 to 19 August 2026 |
| `ley-de-remuneraciones-de-los-servidores-publicos/` | LEY DE REMUNERACIONES DE LOS SERVIDORES PUBLICOS DEL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 22 November 2007 to 23 August 2019 |
| `ley-de-responsabilidad-ambiental/` | LEY DE RESPONSABILIDAD AMBIENTAL PARA EL ESTADO DE MICHOACAN DE OCAMPO | 5 | as first published, then each reform: 10 January 2014 to 19 February 2022 |
| `ley-de-responsabilidad-patrimonial/` | LEY DE RESPONSABILIDAD PATRIMONIAL DEL ESTADO DE MICHOACAN Y SUS MUNICIPIOS | 1 | as first published: 2 September 2017 |
| `ley-de-responsabilidades-administrativas/` | LEY DE RESPONSABILIDADES ADMINISTRATIVAS PARA EL ESTADO DE MICHOACAN DE OCAMPO | 13 | as first published, then each reform: 19 July 2017 to 27 June 2025 |
| `ley-de-responsabilidades-y-registro-patrimonial-de-los-servi/` | LEY DE RESPONSABILIDADES Y REGISTRO PATRIMONIAL DE LOS SERVIDORES PUBLICOS DEL ESTADO DE MICHOACAN Y SUS MUNICIPIOS | 8 | as first published, then each reform: 15 October 2014 to 17 February 2018 |
| `ley-de-salud/` | LEY DE SALUD DEL ESTADO DE MICHOACAN DE OCAMPO | 62 | as first published, then each reform: 9 December 2007 to 19 August 2026 |
| `ley-de-salud-mental/` | LEY DE SALUD MENTAL DEL ESTADO DE MICHOACAN DE OCAMPO | 8 | as first published, then each reform: 13 September 2014 to 6 August 2026 |
| `ley-de-seguridad-privada/` | LEY DE SEGURIDAD PRIVADA DEL ESTADO DE MICHOACAN DE OCAMPO | 3 | oldest version available, then each reform: 4 January 2011 to 29 August 2019 |
| `ley-de-transparencia-acceso-a-la-informacion-publica-y-prote/` | LEY DE TRANSPARENCIA, ACCESO A LA INFORMACION PUBLICA Y PROTECCION DE DATOS PERSONALES DEL ESTADO DE MICHOACAN DE OCAMPO | 11 | as first published, then each reform: 19 May 2016 to 27 May 2026 |
| `ley-de-trasplantes-y-donacion-de-organos-tejidos-y-celulas-e/` | LEY DE TRASPLANTES Y DONACION DE ORGANOS, TEJIDOS Y CELULAS EN EL ESTADO DE MICHOACAN DE OCAMPO | 2 | as first published, then each reform: 9 June 2021 to 27 July 2024 |
| `ley-de-turismo/` | LEY DE TURISMO DEL ESTADO DE MICHOACAN DE OCAMPO | 17 | as first published, then each reform: 4 May 2011 to 9 August 2026 |

## Source

The legislation compilation of Mexico's Supreme Court, the Suprema Corte de Justicia de la Nación (SCJN), at <https://legislacion.scjn.gob.mx/>. For each ordenamiento it lists every publication in the state's official gazette (Periódico Oficial) that changed it (decree, erratum, ruling), with the date of publication, the decree's extract and the whole consolidated text as it stood after that publication. Each version here is one of those texts.

## Dates

- Each commit is dated at **noon, America/Mexico_City, on the day the publication took effect**: the day its own transitorios name, as SCJN's extract quotes them (most often the day after publication). When a decree names none, 3 days after publication.
- A consolidated text holds every change published before it, so it is never dated before the latest of their in-force days. Different in-force days for parts of one decree are not split.
- An act's first commit is its first publication when SCJN holds the original text; otherwise it is the oldest version SCJN holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 Bis; `encabezado.md` holds the title, the promulgation and preamble; `transitorios-original.md` the original transitory articles and `transitorios-<date>.md` those of the reform published that day. Section headings and editor's notes such as "(REFORMADO, P.O. ...)" stay in the file of the article they stand before. One paragraph per line.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of SCJN's own text of that version (read independently of the parser), and every unit's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the publication that changed the text (a decree, an erratum or a ruling), named by its category, gazette date and issue, with an e-mail address that cannot exist (`<key>@legislacion.scjn.gob.mx.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one published in the state's official gazette (Periódico Oficial). The history starts with the oldest text SCJN holds for each ordenamiento, which for many is later than its enactment. Only the ordenamientos listed above are included.
