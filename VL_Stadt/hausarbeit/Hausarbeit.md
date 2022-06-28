## Einleitung

Afrika ist einer der Regionen, die global gesehen vor den größten Herausforderungen im 21. Jahrhundert stehen. Bis 2050 wird die derzeitige Bevölkerung von 1.1 Milliarden Menschen auf das Doppelte anwachsen, wobei 80% dieses Wachstums in Städten stattfinden wird. Diese zusätzlichen Stadtbewohner treffen jedoch auf geringe Beschäftigungsmöglichkeiten und wenig wirtschaftlichen Aufschwung, gepaart mit einer zunehmenden Bedrohung durch den Klimawandel. Die Implikationen, die sich daraus für politische, ökonomische und gesellschaftliche Handlungen ergeben, sind zahlreich, und ein großer Teil hängt von der Möglichkeit ab, die Urbanisierung in wohlstandssteigernde Bahnen zu lenken.

Mit diesen Themen beschäftigen sich Vernon Henderson, Adam Storeygard und Uwe Deichmann in ihrer wissenschaftlichen Arbeit mit dem Titel "Has climate change driven urbanization in Africa?". Der Artikel wurde 2016 im renommierten Journal of Development Economics veröffentlicht und untersucht die Zusammenhänge zwischen Urbanisierung und Klimawandel in Subsahara-Afrika (vgl. @hendersonHasClimateChange2017)

Die beiden Fragen, die die Autoren zu beantworten versuchen, sind einerseits, ob ungünstige Klimaveränderungen dazu führen, dass die Menschen aus den ländlichen Gebieten in die Städte ziehen und andererseits, ob dieser Zuzug dass Gesamteinkommen der Städte erhöht. Die Motivation hinter der Fragestellung ist also, ob die Urbanisierung in Afrika ein Ausweg aus den sich verändernden klimatischen Bedigungen sein kann.

### Forschungsstand

Die Frage, was das Stadtwachstum antreibt, wird in der stadtökonomischen Forschung weit diskutiert. Unterschieden wird dabei im Wesentlichen zwischen Pull-Faktoren wie bspw. Wirtschaftliche Aussichten und Push-Faktoren wie beispielsweise Konflikte. 

Zur Frage des Klimawandels als Push-Faktor der Urbanisierung, die die Autoren untersuchen, ist die nächstverwandte Arbeit von @barriosClimaticChangeRural2006a . Sie untersuchten die Fragestellung anhand eines Paneldatensatzes von 36 Ländern aus Subsahara-Afrika und verglichen ihre Ergebnisse mit Entwicklungsländern aus anderen Regionen. Ähnlich geht @brucknerEconomicGrowthSize2012 vor, der den Zusammenhang zwischen dem Anteil der Landwirtschaft am BIP und Niederschlag untersucht. Auch @hendersonUrbanizationSubSaharanAfrica2013 untersuchten diese Frage bereits für die Weltbank.

Die Autoren des aktuellen Papers erweitern diese Forschung, indem sie zwei Probleme angehen, die die genannten Arbeiten nicht adressieren konnten. Einerseits die beträchtliche inländische Heterogenität durch die Konstruktion eines regionalen und subnationalen Datensatzes. Andererseits die auf Interpolation beruhenden Bevölkerungsdaten durch Nutzen der originalen Zensusdaten. Wir gehen auf diese Daten näher Absatz 2.1 in ein.

Ein weiteres Alleinstellungsmerkmal der Forschungsarbeit ist, dass die Autoren den Einfluss des Klimawandels auf Urbanisierung und Einkommensveränderungen ausdifferenzieren nach dem Industrialisierungsgrad der Stadt. Dieser Ansatz wurde so in noch keinem Artikel verfolgt.

------------------------------------------------------------------------

-   Zu Effekt von Klimawandel auf Afrika

    -   Afrika diverses Klima

-   Effekt von klimawandel auf Landwirtschaft

------------------------------------------------------------------------

## Vorgehensweise

Um die empirischen Untersuchungen zu unterstüzen, konstruieren die Autoren ein mathematisches Modell, auf das im ersten Abschnitt kurz eingegangen wird. Anschließend analysieren wir die Vorgehensweise für beide Forschungsfragen aufgrund der unterschiedlichen Datensätze und Modelle in getrennten Abschnitten

### Mathematisches Modell

Die Autoren modellieren die Bewegungen zwischen dem städtischen Sektor und dem ländlichen Sektor in einem Distrikt

### Klimaveränderung und Urbanisierung

Um die erste Forschungsfrage zu beantworten, ob Klimaveränderungen zu einem verstärkten zuzug in die Städte führen, kombinieren die Forscher verschiedene Datensätze zu Bevölkerung, Klimaveränderungen und Industrie und konstruieren anschließend ein Regressionsmodell.

Für Bevölkerungsdaten nutzen die Autoren Zensusdaten von Ländern in Subsahara-Afrika, die in einem Zeitraum von 1960 bis 2010 mindestens 2 Zensus in einem Abstand von weniger als 20 Jahren durchgeführt haben. Daraus entsteht ein Paneldatensatz mit 29 Ländern, unter anderem nicht Teil ist aber Nigeria aufgrund von Bedenken über die Qualität der Zensusdaten. Das Panel beruht somit nicht auf Interpolation, sondern den reinen Daten. Grundlage sind Publikationen des US. Census Bureau, der U.S. Library of Congress, die Bibliothek der LSE und die British Library. Daraus extrahieren sie daraufhin Daten zu 369 subnationalen Distrikten mit einer durchschnittlichen Fläche von 41.100 Quadratkilometern. Diese Distrikte werden in Abbildung 1 dargestellt.

Zur Untersuchung der klimatischen Bedingungen nutzen die Autoren das University of Delaware Climate Data Set von @WillmottMatsuuraCollaborators und konstruieren aus den Daten zu Niederschlag und potentieller Evapotranspiration ein Index für die Feuchtigkeit. Der Vorteil dieses Indizes ist, dass er ein besserer Indikator für landwirtschaftliches ist, als es reine Niederschlagsdaten könnten, die in anderen Forschungsarbeiten genutzt werden.

Das Ziel der Autoren, die Effekte auf Städte nach dem Industrialisierungsgrad auszudifferenzieren, wird durch die dürftige Datenlage zu Industriestandorten erschwert, insbesondere für den untersuchten Zeitraum ab 1960. Nach einem Hinweis von Alexander Moradi stoßen sie auf den *Oxford Regional Economic Atlas* (OREA) von\@adyAfricaOxfordRegional1965 , der 26 unterschiedliche produzierende Gewerbe nach Stadt und Typ kartographiert. Von diesen 26 Industrien kategoriesieren die Autoren 16 der Industrien als nicht landwirtschaftliche Produkte verarbeitend und somit modern. Diese Unterscheidung wird in der Regressionsanalyse noch bedeutend. Die Standorte der Industrien in den Zensusdistrikten ist in Abbildung 2 dargestellt. Insgesamt haben 25% der Distrikte eine Industrie und 16% eine moderne.

Für die empirische Analyse schätzen die Autoren den Effekt des Wachstums der Feuchtigkeit auf das Stadtwachstum im Distrikt i, im Land j, im Jahr t mit folgendem Regressionsmodell $$
u_{ijt} = \beta_0 w_{ijt} + \beta_1 X_{ij} + \beta_2 X_{ij} \ w_{ijt} + \alpha_{jt}+ \varepsilon _{ijt}
$$ wobei die Variablen wie folgt definiert sind:

-   $u_{ijt}$ ist das Wachstum des Anteils der Stadtbevölkerung an der Gesamtberölkerung,
-   $w_{ijt}$ die Feuchtigkeit über 3 Jahre gemittelt,
-   $X_{ij}$ zeit-invariante Kontrollen,
-   $a_{jt}$ sind Fixed Effects
-   und $e_{ijt}$ der Fehler Term

Die Ergebnisse sind in Tabelle \ref{tbl1} dargestellt, wobei die erste Zeile von Interesse ist. Dort wird in der ersten Spalte der Einfluss auf alle Städte dargestellt. Wie sichtbar ist, gibt es einen generellen negativen Zusammenhang zwischen Wachstum der Feuchtigkeit und der Stadtbevölkerung. Aufgrund der heterogenität der Distrikte ist dieser Effekt aber nicht statistisch signifikant, der Effekt ist also nicht generalisierbar .

In der zweiten Spalte wird der Einfluss auf Distrikte mit moderner Industrie untersucht und hier findet sich ein statistisch signifikanter negativer Zusammenhang. Sinkt also in einem Distrikt mit modernen Industrien die Feuchtigkeit, steigt die Stadtbevölkerung. Ähnliche Effekte auf Distrikte mit irgendeiner Art von Industrie werden in Spalte 3 dargestellt.

Die Autoren testen ihre Ergebnisse auf Robustheit gegenüber anderen Effekten, exemplarisch werden hier Konflikte und Entfernung zur Küste genannt. Erstere, da eine Verschlechterung der landwirtschaftlichen Situation aufgrund von Klimaveränderung Konflikte entstehen lassen könnte, wie bei @burkeClimateConflict2015 argumentiert wurde. Es könnte also sein, dass die Urbanisierung nur aufgrund der Schutzsuche in den Städten geschieht. Die Autoren finden nach einem Abgleich ihrer Daten mit der Social Conflict Analysis Database von @salehyanSocialConflictAfrica2012 keine signifikanten Zusammenhänge. Die Überprüfung des Zusammenhangs mit Hinblick auf die Entfernung zur Küste findet statt, da sie eine Korrelation mit der Feuchtigkeit hat. Doch nach dem Einfügen eines Interaktionsterms zwischen beiden Variablen kristallisieren sich keine signifikanten Effekte heraus.

Zusammenfassend kann man sagen, dass je mehr Industrien ein Distrikt hat, desto stärker wirkt eine Feuchtigkeitsveränderung auf das Wachstum der Stadtbevölkerung. Zusätzliche Arbeitskräfte aus der ländlichen Bevölkerung, die davor in der Landwirtschaft arbeiteten, ziehen also stärker in industrialisierte Städte. Bei einem historischen durchschnittlichen Sinken der Feuchtigkeit um 0.44% pro Jahr würden die am stärksten industrialisierten Städte um 0.51% schneller wachsen als Städte in nicht industrialisierten Distrikten . Das mag erstmal wenig klingen, über einen Zeitraum von Jahrzehnten kumuliert sich dieser Effekt jedoch und hat eine starke Auswirkung auf den Urbanisierungsgrad.

### Klimaveränderung und Einkommenssteigerung

In der zweiten Forschungsfrage untersuchen die Autoren, ob dieser Zuzug in Städte aufgrund von Klimaveränderungen eine Auswirkung auf das Gesamteinkommen der Stadt hat. Dafür konstruieren sie einen neuen Datensatz von Lichtdaten aus dem *U.S. Defence Meteorological Satellite Program* (DSMP) als Indikator für Einkommen, ähnlich zu einer früheren Arbeit von @hendersonMeasuringEconomicGrowth2012. Diese Lichtdaten werden bereinigt um temporäre Lichtquellen und Gasflammen und ein Index für die Lichtintensität von 0 bis 63 für die Emission von 8:30 bis 10:00 morgens extrahiert. Kombiniert werden diese Daten mit Niederschlagsdaten der *Africa Rainfall Climatology Version 2* (ARC2) von @novellaAfricanRainfallClimatology2013a .

Aufgrund der kürzeren Zeitspanne (1992 - 2008), für die Satellitendaten des DMSP zur Verfügung stehen, aber höheren Auflösung ändern die Autoren ihr Modell und untersuchen nun einen Paneldatensatz von 1158 Städten und ihrem jeweiligen Umkreis von 30km (*outer envelope*), die mit den Niederschlagsdaten von ARC2 kombiniert werden. Auch hier werden die Städte wieder mit der Anzahl der (modernen) Industrien aus dem OREA in Verbindung gebracht.

Das Regressionsmodell für Stadt i im Land j ist wie folgt spezifiziert: $$
\ln(light_{it}) = \sum_{j=0}^k \beta_j \ln(rain_{i,t-j}) + \sum_{j=0}^k \gamma_j X_i \ln(rain_{i,t-j}) + \phi_i + \lambda_t + a_{it} + \epsilon_{it}
$$ Die Variablen sind dabei wie folgt definiert:

-   $\ln (light_{it})$ ist der logarithmierte Lichtindex,
-   $\ln (rain_{i,t-j})$ der Niederschlag über 3 Jahre geglättet,
-   $X_i$ zeitinvariante Kontrollen,
-   $\phi_i$ und $\lambda_t$ Fixed Effects der Stadt bzw. des Jahres
-   $a_{it}$ ein stadtspezifischer linearer Trend und
-   $e_{it}$ der Fehlerterm

Die Ergebnisse der Regression sind in Tabelle \ref{tbl2} zu sehen, wobei auch hier wieder die erste Zeile von besonderem Interesse ist. In der ersten Spalte ist der Zusammenhang zwischen dem Niederschlag und den Lichtemissionen auf alle Städte angegeben. Ähnlich zu den Ergebnissen aus Tabelle 1 gibt es hier einen generell negativen Trend, der jedoch nicht statistisch signifikant ist.

Erst in der zweiten Spalte lässt sich ein negativer Zusammenhang in Städten mit einer höheren Anzahl an modernen Industrien erkennen, der auch statistisch signifikant ist. Eine Senkung der Niederschlagsmenge führt in diesen Städten zu höheren Lichtemissionen. Ähnlich verhält es sich in Städten, die irgendeine der 26 Industrien haben.

In der vierten Spalte nutzen die Autoren ein anderes Maß für die Industrialisierung, den Anteil der Landwirtschaft an dem nationalen Bruttoinlandsprodukt (BIP). Dieser bestätigt die Effekte von Spalte 2 und 3. Jedoch ist die Stärke des Zusammenhangs unterschiedlich, was darauf zurückzuführen sein könnte, dass nicht der stadtspezifische Anteil untersucht wird, sondern nur der Anteil auf nationaler Ebene.

Auch für diese Untersuchung führen die Autoren Robustheitsprüfungen durch, einerseits gegen Überschwemmungen, da bei ihnen eine sprunghafte Erhöhung der Niederschlagsmenge und eine Reduktion des Einkommens stattfindet. Des Weiteren überprüfen sie die Effekte, die eine Versorgung mit Energie auf Wasserkraft hat, da diese zu preiswertem Strom bei größeren Wassermassen führen könnte. Für beide Einflüsse finden sie keine signifikanten Effekte, da beide meistens nicht nur auf individueller Stadtebene wirken, sondern auch auf die ländliche Region und die nationale Ebene.

Aus Spalte 3 der Tabelle 2 folgt, dass die Elastizität zwischen Niederschlag und Lichtemissionen für die am stärksten industrialisierten Städte -0.017 beträgt. Nach @hendersonMeasuringEconomicGrowth2012 , die für die Elastizität von Licht und Einkommen einen Faktor von 0.3 bestimmten, folgt daraus eine Elastizität zwischen Niederschlag und Stadteinkommen von -0.051. In verständlicheren Dimensionen ausgedrückt, führt eine Senkung der Niederschlagsmenge um eine Standardabweichung zu einer Steigerung der Lichtemissionen um 11% und ein Wachstum des Einkommens von 3.5%, aber nur in den am stärksten industrialisierten Städten.

## Diskussion

### Bewertung und Schlussfolgerungen

-   Paper stellt erweitert den Forschungsstand auf jedenfall

-   hochrelevant für aktuelle Zeit

-   leider Verbindung beider Fragen nicht so gut geklappt, aufgrund komplett unterschiedlicher Daten und Zeiträume

-   sehr interessante Quelle für Stand der Industrialisierung

    -   leider etwas veraltet, es hat sich seit den 60ern dann doch etwas getan
    -   betont auch in Einleitung, dass es ein Tip eines guten Kollegen war

-   Afrika wird von Klimawandel hart getroffen

-   bereits jetzt nur marginal geeignet für landwirtschaftliche Produktion

-   industrialisierte Distrikte können Klimawandelfolgen entgehen

    -   Jedoch: Afrika wenig strukturelle Transformation
    -   und einhergehend mit intensiver Industrie ist Verschmutzung, die damit nicht übersprungen werden kann (Leapfrogging)

-   Folgen für landwirtschaftliche Produktion können mithilfe von verstärkter Adaption von Dünger und Bewässerung aufgefangen werden

    -   sehr geringe Verbreitung und quasi kein Wachstum seit 80ern

### Forschungsansatz

[Artiikel dazu](https://qz.com/1895253/climate-change-in-india-is-fueling-unchecked-urbanization/)

Erweiterung der Fragen auf den indischen Subkontinent

-   wird von Klimawandel hart getroffen
-   in starkem Wachstum, insbesondere die Industrie

Forschungsfragen

-   wie schwächt der Klimawandel das Wachstum?
-   bietet die Industrie hier den Ausweg für überschüssige Arbeitskräfte?

Daten:

-   indischer Zensus [Web](https://censusindia.gov.in)
-   und auch noch [Weltbank](https://data.worldbank.org/indicator/SP.URB.GROW?locations=IN)

Forschungstand

-   Übersichtspaper: nicht gelesen! [DOI](https://doi.org/10.1002/wcc.560)
-   

Vorteile:

-   konsistente Datenbasis des Zensus
-   bessere Quellen zur Industrialisierung

## Appendix {.unnumbered}

### Abkürzungen {.unnumbered}

-   ARC2: Africa Rainfall Climatology Version 2
-   DSMP: Defence Meteorological Satellite Program
-   OREA: Oxford Regional Economic Atlas
-   BIP: Bruttoinlandsprodukt

### Literaturverzeichnis
