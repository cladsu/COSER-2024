---
language:
- es
---
# Dataset Card for Dataset Name

Este dataset es una parte del Corpus Oral y Sonoro del Español Rural (http://www.corpusrural.es/), en el cual se pueden encontrar las transcripciones de 230 entrevistas revisadas anotadas y segmentadas manualmente por expertos.

## Dataset Details

### Dataset Description

<!-- Provide a longer summary of what this dataset is. -->
El Corpus Oral y Sonoro del Español Rural - COSER (http://www.corpusrural.es/) consta de 1.772 entrevistas semidirigidas (1.910 horas grabadas) que datan de entre 1990 y 2022. Los individuos entrevistados provienen de zonas rurales y tienen una media de edad de 74 años, generalmente son personas que han recibido poca educación académica y han tenido poca movilidad geográfica. El porcentaje de hombres y mujeres entrevistados está equilibrado, siendo un 47'8% hombres y un 52'2% mujeres. Actualmente, se han registrado en el corpus 1.415 enclaves del territorio español (península y los dos archipiélagos).

En este corpus hemos recopilado 230 entrevistas semidirigidas anotadas, revisadas y segmentadas manualmente.
Enclaves de las 230 entrevistas:

Para un mejor entendimiento de los datos proporcionamos un esquema de las marcas que permanecen en este dataset y forman parte de los datos originales:

**Emisiones vocales**:
- Risa ([RISA]): se emplea cuando se ríe una sola persona, ya sea el encuestador o el informante.
- Risas ([RISAS]): sirve para señalar las risas de varias personas.
- Risa en habla ([Rndo: ]): el informante se ríe mientras está contando algo. Podemos incluir primero la marca, y escribir dentro el fragmento que corresponda, o seleccionarlo previamente y pinchar en esta herramienta.
- Llanto en habla ([Llndo: ]): el informante llora mientras está contando algo. Se utiliza igual que “risa en habla”.
- Otra lengua ([L-Otra: ]): para aquellos fragmentos en los que el informante utilice una lengua que no sea el español. Se selecciona la marca, y se escribe dentro el fragmento en la lengua original, o se selecciona el fragmento y, posteriormente, pinchamos en dicha marca. En estos casos, no se debe hacer la equivalencia en español.
- Exclamaciones ([EXCL]): es una marca que se recomienda no utilizar. Por ejemplo, si el informante dice algo como “ay”, o “ah”, en tono exclamativo, es preferible transcribirlo con signos exclamativos: “¡Ay!”, “¡Ah!”.
- Asentimiento ([Asent]): se utiliza para representar todas aquellas emisiones que utilizamos en la lengua oral para asentir algo. Si el informante o el encuestador dice algo del tipo “uhum”, “aham”, “hum”, etc., no se transcribe, sino que utilizamos esta marca. Si dice “sí”, no se utiliza esta marca, sino que se transcriben. Siempre que utilicemos esta marca, debe ponerse punto (“.”), pues cuenta como cualquier intervención: “I1: Mi hijo no vive aquí, por eso ya no hago matanza” / “E1: [Asent]. ¿Y desde cuándo?”.
- Tos ([TOS]).
- Carraspeo ([CARRASP]).
- Chasquido ([CHASQ]).
- Onomatopeya ([ONOMAT]): como se deduce por su nombre, sirve para marcar las onomatopeyas. En este caso, la onomatopeya no se incluye dentro de la marca: transcribimos la onomatopeya, y detrás, ponemos esta marca. Por ejemplo: “[…] y de repente, el libro hizo pum, [ONOMAT] y se cayó”.
- Respiración ([RESPIR]).
- Otras ([OTRAS-EM]): se utiliza para representar aquellas emisiones que sirven al informante para pensar lo que va a decir a continuación. Es muy frecuente en la lengua oral que hagamos cosas como: “Y mi hijo, pues, e…/a…/mm, estudió medicina”, etc. Esto no se transcribe, sino que se utiliza esta marca: “Y mi hijo, pues [OTRAS-EM] estudió medicina”. No hay que confundir “e” o “a” alargada, con las interjecciones “eh” y “ah”, pues estas últimas sí se transcriben, y no necesitan marca: “Mi hijo estudió medicina, eh”.

**Habla simultánea (HS:E/I:)**: Suele ser frecuente que los informantes y los encuestadores se “solapen”, hablando ambos a la vez. Para aquellos casos, recurrimos a esta marca. Con ella, señalamos quien es la persona que interrumpe (si el informante o el encuestador), en cierta forma, el discurso principal. 
Por ejemplo, el informante puede comenzar a contestar antes de que el encuestador termine de realizar la pregunta, como ocurre con [HS:I1: Sí, de… con tirantillos], en la siguiente imagen. En este caso, el encuestador deja que el informarte siga hablando, de ahí que el habla simultánea no se haya cerrado, y su siguiente intervención comience en minúscula, y no en mayúscula, ya que se considera que el inicio de su intervención empieza en el habla simultánea, y continúa. 
Otro ejemplo muy frecuente es que el encuestador asienta, afirme ([HS:E1 [Asent].]; [HS:E1: Ah.]; [HS:E1 Sí.]) o realice nuevas preguntas mientras que el informador está hablando. Si estas intervenciones no interrumpen el discurso principal y son autónomas, deben tener su propia puntuación final, sea punto, exclamación o interrogación.

**Habla cruzada (HCruz)**: En ocasiones, aparecen nuevos integrantes en la conversación. Pensemos en una entrevista con un informantes y dos encuestadores. Están hablando y, de repente, aparece un familiar del informante, y este deja de dirigirse a los encuestadores y se pone a hablar con él. Ahí tenemos una conversación cruzada. Para señalarlo, debemos seleccionar cada una de las intervenciones que conformen esa conversación cruzada, y pinchar en dicho icono. También podemos insertar la marca de “habla cruzada”, y escribir dentro de ella cada fragmento. 
Ejemplo: “en Pola_de_Siero y él es, el padre de este, en Gijón. Este vivió en Gijón y en Madrí=Madrid. En Madrí, [HCruz:¿cuántos años tuvo=estuvo? Unos cuantos, sí.]”

**Desambiguación:** Debe desambiguarse cualquier palabra que pueda confundirse con otra como resultado de la pronunciación dialectal. La variante dialectal se transcribe primero y la convencional después, de acuerdo con la convención (x=y), (forma dialectal= forma estándar). Cuando la forma dialectal implica una reducción puede usarse (0=y). Por ejemplo, canta(0=r)lo, pero debe prestarse atención por si la forma reducida implica un cambio de tilde. Por ejemplo, cárce(0=l) o cantá(0=r)lo, no son equivalencias correctas, ya que el resultado editado sería cárce o cantálo.
- Los participios en –ada y los infinitivos en –ar, que dan lugar a formas idénticas en –á (cantá=cantada o cantar).
- Los participios en –ida(s), que pueden confundirse con los imperfectos de indicativo (tenía(s)=tenida(s)).
- Los infinitivos seguidos de clítico que asimilan o pierden la –r final, para evitar que se confundan con formas de presente seguidas de pronombre enclítico (o de imperfecto de subjuntivo): canta(0=r)lo, toma(0=r)se, etc.
- Los infinitivos sé=ser, dá=dar o dada, vé=ver.
- El cuantificador to=todos, toda(s), cuando equivale a reducción de la forma plural o de las femeninas, no cuando es simplemente reducción de todo.
- El pronombre clítico los=os o nos, y tos=os, para evitar confundirlo con el sustantivo tos o (tos=todos).
- La primera persona analógica de los perfectos de la primera conjugación (cantemos=cantamos), para evitar que se confunda con el presente de subjuntivo.
- Las formas sincréticas de 1p y 3p del singular (ha=he, dijo=dije).
- Las desinencias dialectales de 2p del singular y del plural del perfecto (cantastes=cantaste o cantasteis).
- Los imperativos (ves, oyes=ve, oye), que pueden confundirse con el presente de indicativo.
- Las formas del verbo ser, sos=eres, seis=sois,
- Los imperativos con pronombre os enclítico, que pueden confundirse con los participios en –ados, -idos. En este caso, se desambigua la forma menos frecuente, el imperativo, con punto alto: compra·os, salí·os.
- Las palabras: ca=casa o cada, ma=mal o mar, pa=pan (puede confundirse con el ubícuo pa=para, que no se desambigua), so=sol (puede confundirse con la preposición so), ande=adonde (puede confundirse con el presente de subjuntivo del verbo andar), mía=mira (puede confundirse con el posesivo femenino), vía(s)=veía(s) o vida(s), ara=ahora o ara, etc.
- La forma l’ o ‘l puede ser artículo o pronombre clítico.
  - Como artículo. En amalgamas muy frecuentes como to’l o pa’l no es necesario desambiguar el artículo. En otras menos frecuentes sí sería necesario. En los casos en que la palabra comience por vocal a- hay que atender a si existe o no cambio de género. Por ejemplo, l’aceite puede equivaler a el aceite o la aceite y la equivalencia debería hacerse en consecuencia: (l’=el)aceite.
  - Como pronombre. Si el clítico se apoya en una forma verbal comenzada por vocal, es muy frecuente que pierda su vocal. Por ejemplo, L’he hecho por Lo he hecho. Solo debe desambiguarse cuanto exista seguridad sobre el clítico. Por ejemplo, l’echamos arroz > (l’=le), ejemplo donde sería también posible transcribir, dadas las vocales iguales, le echamos.
- La variación de otras vocales átonas, como a-e, a-o, e-o deben desambiguarse, y marcarse siempre: (halecho=helecho). Lo mismo ocurre con la vacilación entre a-o, a-e tónicas. 
- Pérdida de [d] intervocálica en:
  -  -ado(s), -ada(s): (cansaos=cansados), (cansá=cansada)
  -  -ido(s), -ida(s): (salíos=salidos), (vía=vida)
  -  -udo, -uda: (púo=pudo)
  -  entre vocales iguales: (pue=puede), (to=todo), (ca=cada)
  -  ante vocal tónica: (cazaor=cazador), (roílla=rodilla)
  -  otros contextos. (píe=pide), (aonde=adonde), (ande=adonde)
- Pérdida de otras consonantes intervocálicas (ɾ, n, χ, etc.): (quie=quiere), (mía=mira), (tie=tiene).
- Pérdida de –d final: (necesidá=necesidad)
- Pérdida de – ɾ final: (salí=salir)
- Pérdida de –l final: (so=sol)
- Pérdida de –χ final u otras consonantes (-k, -t, -p, etc.): (reló=reloj), (coñá=coñac)

**Nombres**: Los nombres de las personas participantes están anonimizados para proteger su identidad, dado que se hablan de datos personales en las entrevistas. En la base de datos los nombres propios no aparecen, pero sí se pueden encontrar los nombres de celebridades o referentes culturales.

**Números**: Se transcribe en letra los números (cincuenta_y_tres). Excepciones:
Los años de nacimiento, evento, etc: “tengo ochenta_y_seis años y nací en el 34”, “en el año 1945 estaba en Salamanca”.
Expresiones como “treinta y pico”, “cuarenta y tantos”...




- **Curated by:** [More Information Needed]
- **Funded by [optional]:** Inés Fernández-Ordoñez
- **Shared by [optional]:** [More Information Needed]
- **Language(s) (NLP):** [More Information Needed]
- **License:** [More Information Needed]

### Dataset Sources [optional]

<!-- Provide the basic links for the dataset. -->

Las 230 entrevistas revisadas se pueden descargar de la página web de COSER (https://corpusrural.fe.uam.es/coser/descargas.php) pinchando en el enlace de la Versión 3.0 (Mayo 2022) - Pueyo Mena, F. Javier: Corpus oral y sonoro del español rural etiquetado. Versión 3.0 [mayo 2022].
Los archivos están en extensión XML, que distingue entre dos parents: cabecera y entrevista. En cabecera tenemos los datos sobre la entrevista: provincia, enclave, fecha de la entrevista, duración de la entrevista, los datos de los informantes (sin nombre), nombre de los encuestadores, personas que han llevado a cabo la transcripción y temas que se han tratado en la entrevista.
En el apartado de entrevista tenemos los turnos con los atributos de id (marca el número de turno) y mp3 (duración del turno). El primer children de turno siempre es la referencia de la persona que habla en ese turno, puede ser informante (I) o entrevistador (E). El resto de children de turno son las palabras (w), signos de puntuación (punct), nombres propios (NP - que salen anonimizados), marcas lingüísticas como emisiones, ininteligible o "lit" (que puede ser la reproducción de un refrán, dicho popular, versos de un poema, etc).

- **Repository:** http://www.corpusrural.es/index.php
- **Paper [optional]:** https://raco.cat/index.php/Dialectologia/article/view/198820/266019
- **Demo [optional]:** [More Information Needed]

## Uses

<!-- Address questions around how the dataset is intended to be used. -->

### Direct Use

<!-- This section describes suitable use cases for the dataset. -->

[More Information Needed]

### Out-of-Scope Use

<!-- This section addresses misuse, malicious use, and uses that the dataset will not work well for. -->

[More Information Needed]

## Dataset Structure

<!-- This section provides a description of the dataset fields, and additional information about the dataset structure such as criteria used to create the splits, relationships between data points, etc. -->

[More Information Needed]

## Dataset Creation

### Curation Rationale

<!-- Motivation for the creation of this dataset. -->

[More Information Needed]

### Source Data

<!-- This section describes the source data (e.g. news text and headlines, social media posts, translated sentences, ...). -->

#### Data Collection and Processing

<!-- This section describes the data collection and processing process such as data selection criteria, filtering and normalization methods, tools and libraries used, etc. -->
A fin de generar una base de datos manipulable y accesible para tareas de NLP, los archivos obtenidos en extensión XML se han convertido en un csv que recoja toda la información. Para ello se han usado las librerías de xml.etree, pandas, BeautifulSoup4 y RegEx. Con xml.etree se ha accedido a las rutas de los archivos y se han parseado para conseguir acceso a los datos. Después, se han leido los contenidos de los archivos xml con BeautifulSoup para extraer los atributos de turno y el texto contenido en cada turno. Con pandas se ha generado un dataframe en el cual se iban añadiendo los datos.
Dado que el texto mostraba caracteres especiales y saltos de línea, tabulaciones o espacios fuera de lugar; se ha limpiado el archivo accediendo al csv y aplicando las expresiones regulares correspondientes para obtener un dataset accesible.



[More Information Needed]

#### Who are the source data producers?

<!-- This section describes the people or systems who originally created the data. It should also include self-reported demographic or identity information for the source data creators if this information is available. -->
El COSER es un proyecto colectivo en el que han colaborado, a lo largo de los años, un sinfín de estudiantes, licenciados y profesores. Puede verse una lista pormenorizada de aquellos que participaron en la recolección de los datos en Campañas (http://www.corpusrural.es/participantes.php). Los autores de las transcripciones y los responsables de su revisión se mencionan, en orden cronológico de intervención, en la ficha de cada uno de los Archivos disponibles. Nos limitamos aquí a citar a aquellos investigadores y colaboradores que han participado de forma más estrecha y directa en el proyecto.



[More Information Needed]

### Annotations [optional]

<!-- If the dataset contains annotations which are not part of the initial data collection, use this section to describe them. -->

#### Annotation process

<!-- This section describes the annotation process such as annotation tools used in the process, the amount of data annotated, annotation guidelines provided to the annotators, interannotator statistics, annotation validation, etc. -->

[More Information Needed]

#### Who are the annotators?

<!-- This section describes the people or systems who created the annotations. -->

[More Information Needed]

#### Personal and Sensitive Information

<!-- State whether the dataset contains data that might be considered personal, sensitive, or private (e.g., data that reveals addresses, uniquely identifiable names or aliases, racial or ethnic origins, sexual orientations, religious beliefs, political opinions, financial or health data, etc.). If efforts were made to anonymize the data, describe the anonymization process. -->

[More Information Needed]

## Bias, Risks, and Limitations

<!-- This section is meant to convey both technical and sociotechnical limitations. -->

[More Information Needed]

### Recommendations

<!-- This section is meant to convey recommendations with respect to the bias, risk, and technical limitations. -->

Users should be made aware of the risks, biases and limitations of the dataset. More information needed for further recommendations.

## Citation [optional]

<!-- If there is a paper or blog post introducing the dataset, the APA and Bibtex information for that should go in this section. -->

**BibTeX:**

@article{Fernández-Ordóñez_2010, title={Dialect grammar of spanish from the perspective of the audible corpus of spoken rural spanish (or corpus oral y sonoro del español rural, coser)}, url={https://raco.cat/index.php/Dialectologia/article/view/198820}, number={3}, journal={Dialectologia: revista electrònica}, author={Fernández-Ordóñez, Inés}, year={2010}, month={ago.}, pages={23-51} }

**MLA:**

Fernández-Ordóñez, I. «Dialect Grammar of Spanish from the Perspective of the Audible Corpus of Spoken Rural Spanish (or Corpus Oral Y Sonoro Del español Rural, Coser)». Dialectologia: Revista electrònica, Núm. 3, agosto de 2010, p. 23-51, https://raco.cat/index.php/Dialectologia/article/view/198820.

## Glossary [optional]

<!-- If relevant, include terms and calculations in this section that can help readers understand the dataset or dataset card. -->

[More Information Needed]

## More Information [optional]

[More Information Needed]

## Dataset Card Authors [optional]

[More Information Needed]

## Dataset Card Contact

[More Information Needed]