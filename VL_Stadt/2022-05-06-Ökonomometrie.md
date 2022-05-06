# 06.05.2022 Ökonomometrische Methoden


## Querschnittsregression

eine Beobachtung pro Obversationseinheit

**Beispiel:** 
Regression der Wohnungspreise $y_i$ verschiedener Wohnungen $i$ mit verschiedenen Charakteristika $x_{1,i}, x_{2,i},...$
$$
y_i = \beta_0 + \beta_1 * x_{i,1} + ... + u_i
$$
*u* = Fehlerterm


### Annahmen des Linearen Regressionsmodells

1. **lineare Parameter**: ökonomischer Sachverhalt kann durch lineares Modell ausgedrückt werden
2. **zufällige Stichproben:** repräsentative Stichprobe
3. **keine perfekte Kolinearität**: Regressionsmodell spielt sonst verrückt
    - keine Regressoren mit Korrelation über 0.7
4. **Exogenität der Regressoren**: Erwartungswert des Fehlerterms *u* = 0
    - keine Korrelation von unabhängigen Variablen mit Fehlerterm
5. **Homoskedastizität:** Fehlerterm hat für alle Obversationseinheiten gleiche Varianz
    - häufig nicht => kann behoben werden (*heteroskedastizitäts-robusten Standardfehlern*)

### OLS-Schätzer

Miminierung der quadratischen Abweichungen 
$$
\sum_{i=1}^N (y_i - \beta_0 - \beta_1*x_{i1} - ...- \beta_k*x_{ik})
$$
erhält Regressionskoeffizienten $\beta_1, \beta_2,...,\beta_k$

#### Interpretation

$\hat\beta_j$ = erwartete Veränderung von *y* , aus einer **ceteribus paribus** Veränderung von $x_j$
$$
\Delta \hat{y} = \hat\beta_j * \Delta x_j
$$

- Beispiel: 
    - *y* = Wohnungsmiete in Euro
    - *x* =  Entfernung vom Stadtzentrum
    - $\beta_j$ = -0,9
- 1km mehr Entfernung senkt Miete um 0,90 Euro

#### Dummy Variablen

auch Binäre Variablen, können nur 0 oder 1 annehmen

bspw. "Garten" oder "kein Garten"



## Instrumentvariablenschätzung

falls Annahme 4 des LRM (Endogenität eines Regressors) verletz => verzerrte Ergebnisse

Stattdessen: Schätzung mit **Instrument-Variablen**

- suche außerhalb des Modells nach Instrument-Variable *z*
    - nicht mit Fehlerterm korreliert (**Exogenität**)
    - mit *x* korreliert ist (**Relevanz**)

Beispiel: Untersuchung ob Wohnungsviertel mit höherer Eigentumsquote bessere Luft haben

- Problem: bessere Luft kann auch zu mehr Wohnungskauf führen (Rückkopplung)
- alternative Variable für Eigentumsquote gesucht: *Zerstörungsgrad der Stadt im 2 WK.*
    - stark zerbombte Städte = mehr Mietwohnungen wieder aufgebaut (niedriger Eigentumsquote)
    - wird nicht durch heutige Luftqualität beinflusst
    - korreliert mit Eigentumsquote



## Paneldatenregression

gleiche Obversationseinheiten über *T* Zeitperioden

**Beispiel:**
Regression der jährlichen Durschnittseinkommen $y_{it}$ der Städte $i$ auf verschiedene Charakteristika $x_{1,it}, x_{2,it}$ der Stadt zu Zeitpunkten *t*
$$
y_{it} = \alpha_i+ \alpha_t+\beta_1 * x_{1,it} + ... + \beta_K * x_{K,it} + u_{it}
$$

- Vorteil: jede Einheit wird zu mehreren Zeitpunkten beobachtet
- Variation über Stadt und Zeit: erkenntnis über
    - stadtpezifische, zeitinvariate Effekte $a_i$
    - periodenspezifische Effekte $a_t$ 
- Meist gilt $N >> T$ (mehr Einheiten als Beobachtungseinheiten)

### statische Paneldatenmodelle

#### Fixed Effects Schätzer

von allen Variablen den Mittelwert über Zeit $\bar{y_i}$ ab und dann OLS

- Vorteil: erlaubt Korrelation von $a_i$ mit x-Regressoren
- Nachteil: keine Koeff. von zeitinvaritan Regressoren schätzbar

meistgenutzter Schätzer in Stadtökonomie und Paneldaten

#### Random Effects Schätzer

$a_i$ wird in Fehlerterm gezogen

- Vorteil: kann auch Koeff. von zeitinvariaten Regressoren schätzbar
- Nachteil: Bedingung von $Cov(x_{i,t},a_i)=0$ (selten)

### dynamische Paneldatemodelle

mega kompliziert!

nutze **GMM-Schätzer** von Arrellano und Bond

meist trechenintensiver

### natürliches Experiment

