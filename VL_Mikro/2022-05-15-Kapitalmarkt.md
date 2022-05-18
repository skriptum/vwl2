# 15.05.2022 Kapitalmarkt

*Was passiert, wenn Haushalte die Möglichkeit haben Geld anzulegen / zu leihen?*

=> Erfindung des Bankensystems!

## intertemporale Budgetbeschränkung

gegenwärtige Wert zukünftiger Auszahlungen $B = \frac{m}{(1+r)^t}$

- *m* = heutige Einzahlung
- *r* = Zins

Entscheidung eines Haushalts zwischen Gütern in zwei Perioden

- $x_{p2}, x_{p1}$ = Güter in Periode 1/2
- $m_1,m_2$ = Einkommen in Periode 1 / 2
- Preise der Güter sind konstant und gleich 1

Güterkonsum in Periode 2, wenn Haushalt in Periode 1 anlegen kann:
$$
x_{p2} = m_2 + (m_1 -x_{p1}) + r*(m_1 - x_{p1}) \\
= m_2 + (1+r) * (m_1 - x_{p1})
$$
alternativ: Haushalt kann in Periode 1 Geld leihen 
$$
x_{p2} = m_2 - (x_{p1} - m_1) - r*(x_{p1} - m_1) \\
= m_2 - (1+r)*(x_{p1} - m_1) \\
= m_2 + (1+r)*(m_1-x_{p1})
$$
= gleiche Mengenfunktion wie davor
$$
\text{B in Zukunftswerten:}\\
(1+r) * x_{p1} + x_{p2} = (1+r) * m_1 + m_2 \\
\text{B in Gegenwartswerten:}\\
x_{p1} + \frac{x_{p2}}{(1+r)} = m_1 + \frac{m_2}{(1+r)}
$$
![2022-05-05_20.45.42](../images/2022-05-05_20.45.42.jpg)

## intertemporale Konsumpräferenzen

wie lässt sich die Präferenz eines Haushalts zwischen zwei Zeitpunkten beschreiben?

Ziel: maximiere den Gesamtnutzen in beiden Perioden

Lagrange Funktion aufstellen: 
$$
\begin{aligned}
L = U(x_{p1}, x_{p2}) &+ \lambda \ [m_1 * (1+r) + m_2 - (1+r)x_{p1} - x_{p2}] \\
&\to \frac{\partial L}{\partial x_{p1}} = \frac{\partial U}{\partial x_{p1}} - \lambda * (1+r) = 0 \\
& \to \frac{\partial L}{\partial x_{p2}} = \frac{\partial U}{\partial x_{p2}} - \lambda  = 0 \\
&\to \frac{\partial L}{\partial \lambda} = m_1 * (1+r) + m_2 - (1+r)x_{p1} - x_{p2} = 0 \\
\end{aligned}
$$
Umstellen für die Zeitpräferenzrate
$$
\implies \frac{\frac{\partial L}{\partial x_{p1}}}{\frac{\partial L}{\partial x_{p2}}}  = 1+r \text{ oder } \frac{MU(x_{p1})}{MU(x_{p2})} = 1+r \\
r = \frac{MU(x_{p1})}{MU(x_{p2})} - 1 \\
r = \frac{MU(x_{p1})}{MU(x_{p2})}- \frac{MU(x_{p2})}{MU(x_{p2})} \\
r = \bold{\tau = \frac{MU(x_{p1})- MU(x_{p2})}{MU(x_{p2})}}
$$
Analogie Betrachtungen dieser Formeln

![2022-05-18_11.40.04](../images/2022-05-18_11.40.04.jpg)