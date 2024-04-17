# Mathematisches Pläuschchen – Wie kommt man von der Hälfte zum Drittel?
Vom 4\. July 2021

<div align=center style="text-align: center;">
    <img width="850" src="./Media/haelfte-zu-drittel.png"/>
</div>

Eine Idee die mir schon seit Anfang meines Physikstudiums im Kopfe herumkreist. Ich hatte einen Dozenten, der verzweifelt versuchte in seiner Vorlesung die Tafel in drei gleich große Stücke aufzuteilen. Wer es schon einmal selbst probiert hat, ohne ein Lineal zu benutzen, stellt schnell fest, dass das überhaupt nicht einfach ist. Was man mit dem Auge gut hinbekommt ist die Hälfte eine Länge, weil wir hierbei einfach uns auf die Symmetrie des Problems verlassen können. Wenn beide Teile gleich groß sind, dann hat man die Hälfte, aber wie ist es bei einem Drittel einer Länge? Hierbei ist das Problem nicht mehr symmetrisch, man müsste ständig nachjustieren und bleibt manchmal frustriert zurück. Dann bekam ich bei einem Spieleabend vor gut 3 Jahren die Idee. Wenn ich nur die Methode der Hälfte verstehe, dann teile ich ein Kartenstapel in zwei Hälften auf und diese Hälften teile ich nochmal in zwei Hälften auf. Ich habe 4 Stapel keine 3. Jetzt nimmt man den restlichen Stapel und macht dasselbe nochmal. Man macht diesen Algorithmus so lange bis alle Karten verteilt sind oder noch ein Rest von 1 oder 2 Karten übrig bleibt.

Diesen Algorithmus habe ich mal versucht mathematisch zu formulieren und kam dann darauf, dass ich auch einfach 4 Stapel machen kann und den letzten Stapel wieder auf 4 Stapel verteile bis alles verteilt ist. Dabei kommt man auf folgende Summenformel:

$$
 {\color{cyan}\sum} ^{\color{cyan}\infty\color{black}} _{{\color{Orchid}k}=1} \frac{1}{4^{\color{VioletRed}k\color{black}}}=\frac{1}{4}+\frac{1}{4^2}+\frac{1}{4^3}+...=\frac{1}{3}
$$

<!-- $$ \colorbox{white}{${\color{cyan}\sum} ^{\color{cyan}\infty\color{black}} _{{\color{pink}k}=1} \frac{1}{4^{\color{pink}k\color{black}}}=\frac{1}{4}+\frac{1}{4^2}+\frac{1}{4^3}+...=\frac{1}{3}$} $$ -->


<!-- <div align=center style="text-align: center;"> <img width="550" src="./Media/formula-1-4-3.png"/> </div> -->

Diese Summenformel ist nicht neu, diese hat auch schon der gute [Archimedes](https://en.wikipedia.org/wiki/1/4_%2B_1/16_%2B_1/64_%2B_1/256_%2B_%E2%8B%AF) gefunden und auch schon eindrucksvoll geometrisch [bewiesen](https://en.wikipedia.org/wiki/1/4_%2B_1/16_%2B_1/64_%2B_1/256_%2B_%E2%8B%AF#Proof_by_Archimedes). Meine Idee war es diese Formel zu verallgemeinern. Wenn man nun in der Summenformel statt %% 1/4 %% mit %% 1/5 %% ersetzt bekommt man %% 1/4 %% als Ergebnis der Summe. Hierbei lässt sich ein Muster erkennen. Das Ergebnis unterscheidet sich immer nur um Eins von dem Nenner in der Summe, was sich so schreiben lässt:

$$
 {\color{cyan}\sum}^{\color{cyan}\infty\color{black}}_{{\color{pink}k}=1} \frac{1}{(n+1)^{\color{pink}k\color{black}}}=\frac{1}{n}
$$

<!-- <div align=center style="text-align: center;">    <img width="550" src="./Media/formula-1-n-2.png"/> </div> -->

Wir können sogar beliebige Werte für %% n %% einsetzen. Diese Formel konnte ich so in der Form im Internet noch nicht finden, aber sie ist verwandt mit der geometrischen [Reihe](https://de.wikipedia.org/wiki/Geometrische_Reihe), welche auch schon bewiesen wurde.


$$
 {\color{cyan}\sum}^{\color{cyan}\infty\color{black}}_{{\color{pink}k}=0} {q^{\color{pink}k}}=\frac{1}{1-q}
$$

<!-- <div align=center style="text-align: center;">     <img width="550" src="./Media/formula-q.png"/> </div> -->

Der Unterschied ist, dass diese Reihe bei null anfängt zu zählen, die Eins im Nenner bei dem Ergebnis steht und unsere Reihe eine Art Spezialfall dieser Reihe ist. Für den Wert von
$$
q = \frac{1}{1+n}
$$
bekommen wir fast das gleiche Ergebnis nur mit einer Eins dazu addiert. Dadurch können wir unsere Reihe in Form der geometrischen Reihe schreiben und den Beweis für die Reihe benutzen, damit unsere Summe immer konvergiert, egal welchen Wert wir für %% n %% einsetzen.

Dass eigentlich faszinierende an einer unendlichen Reihe ist, dass der unendliche Prozess zu einem endlichen Ergebnis führt. Diese Unendlichkeit bespreche ich in einem weiteren Artikel, also seit gespannt auf das nächste mathematische Pläuschchen. Und wem die Farben in den Formeln aufgefallen sind, wird auch noch mit einem [Artikel](Blog/Mathematisches_Pläuschchen_-_Farbige_Formeln.md) belohnt werden.
