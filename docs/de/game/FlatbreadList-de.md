# The Native Pond Feature-Roadmap

![flatbreadlist_background](/background/de/FBL-docs-bg-de.png)

> [!WARNING]
> 1. Alle Inhalte dieser Liste sind Zukunftsmusik – sie stellen weder die finale Darstellung noch die tatsächliche Umsetzung dar.
> 2. Ein Teil der Inhalte dieser Liste wurde in den Sitzungen der Entwicklungsgruppe nicht besprochen.
> 3. Ein Teil der Inhalte dieser Liste wurde keiner Machbarkeitsstudie unterzogen.
> 4. Diese Liste kann als Leitfaden für Fanwerke und abgeleitete Projekte dienen.
> 5. Die Entwicklungsgruppe behält sich alle weiteren Maßnahmen in Bezug auf diese Liste sowie die endgültige Auslegung dieser Liste vor.

---

## 🎮 Steuerungssystem

Eine flüssige Bewegung und eine gute Kameraperspektive sind ein wichtiger Bestandteil, damit ein Spiel wirklich Spielgefühl hat. **Der Charakter muss sich auf jeden Fall bewegen können!**

### Fortbewegung

- Der Spieler steuert den Charakter durch die **Karte** und **aktiviert** an besonderen Orten (wie der Angelplattform) durch Tastendruck oder das Betreten des kleinen Koordinatenbereichs des Ortes die Animation, die in diesen **besonderen Ort** hineinführt.
- Die Interaktion mit dem Spiel erfolgt über Touch-Buttons (mobil), Tastatur (Desktop) und Gamepad; die Tastenbelegung kann frei angepasst werden.

### Kameraperspektive

- Auf nicht-besonderen Bereichen der Karte wird die **Dritte-Person-Perspektive** verwendet.
- Auf besonderen Bereichen der Karte (wie der Angelplattform) wird die **Erste-Person-Perspektive** verwendet und die Innenausstattung dieses besonderen Bereichs (falls vorhanden) gezeigt.
- Die Karte **bewegt** sich mit der Kamera.

---

## 🗺️ Kartensystem

Leg dich auf den Tisch und baue eine **Karte** – in dieser Karte gibt es wirklich alles!

### Zoom und Richtung

- Die Karte **rotiert** nicht mit der Kamera.
- Die Karte kann **gezoomt** werden.
- Die Karte folgt der Richtungslogik „**Norden oben, Süden unten, Westen links, Osten rechts**“.

### Grenzen

- Die Spielkarte besitzt **Grenzen**, das heißt, der Spieler kann die **Kartenränder** nicht durchqueren.
- Wenn der Spieler versucht, die Grenze zu durchqueren, wird er vom Spiel **gewaltsam zurückgeholt**, und es erscheint der Splash-Text „* Ein vertrautes Gefühl steigt auf – du scheinst zu hören: ‚Erkunden wir das Gebiet vor uns später!‘ Auch wenn du weißt, dass du es später nie erkunden kannst, willst du es trotzdem versuchen.“
- Die Grenzen können offensichtliche **natürliche Hindernisse** (wie große Berge) oder **menschengemachte Zäune** (wie die Mauern der Architektur im Huizhou-Stil) sein.

### Wetter

- Die **Arten** des Wetters sind wie folgt:
	- Sonnig.
	- Regen.
	- Gewitter.
	- Schnee.
- Wetter**wechsel** können bestimmt werden durch:
	1. Manuelle Einstellung durch den Spieler.
	2. Ähnlichkeit mit den klimatischen Besonderheiten eines Ortes.
	3. Vollkommen zufällige Wahrscheinlichkeit.

### Jahreszeiten

- Die Jahreszeit wechselt alle **90 Stunden**.
- Die **Arten** der Jahreszeiten sind wie folgt:
	- Frühling.
	- Sommer.
	- Herbst.
	- Winter.

### Kamera

- Der Spieler kann an beliebiger Stelle (außer in GUI-Oberflächen) durch Drücken einer Tastaturtaste, eines Buttons oder einer Controller-Taste **fotografieren**.
- Beim **Fotografieren** überzieht das Spiel den Bildschirm mit einem **weißen Licht**, um das Fotografieren darzustellen. Möglicherweise muss auf dem Startbildschirm des Spiels ein Warnhinweis für **fotosensible Epilepsie** eingeblendet werden.
- Beim **Fotografieren** erfasst das Spiel automatisch alle Elemente des Bildschirms (außer GUI-Elementen) und fügt einen **Bilderrahmen** hinzu.
- Das Spiel **speichert** die Fotos in einem **festgelegten Ordner**, damit sie geteilt werden können.

### Angelgewässer

- Das Angelgewässer ist der wichtigste besondere Bereich des Spiels und umfasst **Angelplattform**, **Teich** und **Boot**.

#### Angelplattform

- Liegt am südlichsten **Ende** des Teichs.
- Wenn der Spieler diesen besonderen Bereich **betritt**, zoomt die Kamera automatisch hinein und wechselt in die Erste-Person-Perspektive; der Charakter nimmt eine sitzende Haltung ein, und die visuelle Oberfläche dieses besonderen Bereichs wird angezeigt.
- Die Angelplattform dient zum **Angeln**.

#### Teich

- Liegt am nördlichsten **Ende** der Karte.
- Wenn der Spieler diesen besonderen Bereich **betritt**, wechselt der Charakter in den **Schwimmzustand**.

#### Boot

- Liegt an **beliebiger Stelle** des Teichs (dies hängt davon ab, wo der Spieler das Boot zuletzt geparkt hat).
- Wenn der Spieler diesen besonderen Bereich **betritt**, wechselt der Charakter in den **Steuerzustand**, und die visuelle Oberfläche dieses besonderen Bereichs wird angezeigt.
- Der Spieler kann das Boot über den **Teich** steuern.

### Zelt

- Liegt im mittleren, leicht **südwestlichen** Teil der Karte.
- Wenn der Spieler diesen besonderen Bereich **betritt**, zoomt die Kamera automatisch hinein und wechselt in die Erste-Person-Perspektive, und die visuelle Oberfläche dieses besonderen Bereichs wird angezeigt.
- Das Zelt ist das **Herzstück des Lagers**.
- Die **Innenausstattung** und **Größe** des Zelts können sich am Zeltdesign aus „Robinson Crusoe“ orientieren.

### Ackerland

- Das Ackerland liegt auf der **Südostseite** des Zelts.
- Wenn der Spieler diesen besonderen Bereich **betritt**, zoomt die Kamera automatisch hinein und wechselt in die Erste-Person-Perspektive, und die visuelle Oberfläche dieses besonderen Bereichs wird angezeigt.
- Das Ackerland dient zum **Pflanzen**.

### Markt

- Der Markt liegt im **Osten** der Karte.
- Wenn der Spieler diesen besonderen Bereich **betritt**, zoomt die Kamera automatisch hinein und wechselt in die Erste-Person-Perspektive, und die visuelle Oberfläche dieses besonderen Bereichs wird angezeigt.
- Der Markt dient zum **Handeln**.

### Baum

- Liegt **südöstlich** des Zelts.
- Wenn der Spieler diesen besonderen Bereich **betritt**, zoomt die Kamera automatisch hinein und wechselt in die Erste-Person-Perspektive; der Charakter nimmt eine sitzende Haltung ein.
- Auf dem Baum erscheinen manchmal (zum Beispiel im Herbst) **Äpfel**. Die Äpfel kann der Spieler mit einem **langen Holzstab** herunterschlagen und **einsammeln**.
- Wenn der Spieler eine Weile (etwa 1 Minute) unter dem **Baum** bleibt, blendet das Spiel den schwebenden Button „Halte [W] gedrückt, um zu meditieren“ ein. Wenn der Spieler W drückt, den Button klickt oder die Controller-Taste betätigt, beginnt die **Meditation**. Während der **Meditation** zeigt das Spiel einen vollflächigen **visuellen Effekt** (verschiedene physikalische Formeln), und es besteht eine gewisse Wahrscheinlichkeit, von einem **Apfel** getroffen zu werden.

### Lagerfeuer

- Liegt nicht weit **östlich** des Zelts.
- Wenn der Spieler diesen besonderen Bereich **betritt**, zoomt die Kamera automatisch hinein und wechselt in die Erste-Person-Perspektive, und die visuelle Oberfläche dieses besonderen Bereichs wird angezeigt.
- Das Lagerfeuer kann **entzündet** werden und spendet Licht.
- Das Lagerfeuer kann zum **Kochen** genutzt werden.

### Wunderbare Meeresschnecke

- Der Spieler kann am **Sandstrand** am Wasser die **wunderbare Meeresschnecke** aufheben.
- Wenn der Spieler die **wunderbare Meeresschnecke** **aufhebt**, wechselt der Charakter in den Blaszustand und die Kamera zoomt automatisch hinein. Der Spieler kann sich dann nicht mehr bewegen. Gleichzeitig wird die visuelle Oberfläche dieses besonderen Gegenstands angezeigt.
- Die wunderbare Meeresschnecke besitzt insgesamt 7 **Töne**, die der Spieler spielen kann.
- Die wunderbare Meeresschnecke hat mehrere **Varianten**, deren **Klangfarben** sich unterscheiden.

### Briefkasten

- Liegt auf der **Südseite** des Zelts.
- Wenn der Spieler diesen besonderen Bereich **betritt**, zoomt die Kamera automatisch hinein und wechselt in die Erste-Person-Perspektive, und die visuelle Oberfläche dieses besonderen Bereichs wird angezeigt.
- Der Briefkasten dient zum **Empfangen und Versenden von Post**.

---

## 🎣 Angelsystem

An der **Angelplattform** kann der Spieler mit einer **Angelrute** angeln.

### Fischarten

- Im **Angelgewässer** des Spiels können sowohl **Salzwasserfische** als auch **Süßwasserfische** gefangen werden. Neben Fischen können auch **Sammelstücke** geangelt werden.
	1. Dies kann anhand der vom Spieler gewählten **Angelplattform** bestimmt werden (zum Beispiel können an einer Angelplattform am Meer nur Salzwasserfische, an einer Angelplattform am See nur Süßwasserfische gefangen werden).
	2. Dies kann anhand der **Wahrscheinlichkeiten** der einzelnen Fischarten bestimmt werden (das heißt, an derselben Angelplattform am Meer können je nach Wahrscheinlichkeit sowohl Salzwasser- als auch Süßwasserfische gefangen werden).
- Die **Wahrscheinlichkeit**, die einzelnen Fischarten zu fangen, richtet sich nach:
	1. Der **realen** Wahrscheinlichkeit, die jeweiligen Fischarten zu fangen. Dies kann ein Wertebereich sein, der anhand verschiedener Faktoren (wie Wetter, Jahreszeit usw.) angepasst wird, statt starr zu bleiben.
	2. Einer vollkommen **zufälligen** Wahrscheinlichkeit.
- Die **Wahrscheinlichkeit**, Sammelstücke zu fangen, richtet sich nach:
	1. Der historischen **Bissrate** des Spielers.
	2. Einer zufälligen **Wahrscheinlichkeit** innerhalb eines festen Bereichs.
	3. Einer vollkommen **zufälligen** Wahrscheinlichkeit.

### Bissrate

Erwähnenswert ist: Die Bissrate bezeichnet die Wahrscheinlichkeit, dass ein Fisch **anbeißt**, nicht die Wahrscheinlichkeit, den Fisch am Ende zu fangen.

- Die **Bissrate** des Spiels wird gemeinsam durch folgende Faktoren bestimmt:
	- Ob sich Köder am Angelhaken des Spielers befindet.
	- Ob der Spieler einen Anfütterungsplatz angelegt hat.
	- Die Art des Köders am Angelhaken.
	- Die Spielzeit (zum Beispiel Tag, Nacht).
	- Ob nachts die Stirnlampe eingeschaltet ist.
	- Das Spielwetter.
	- Die Spieljahreszeit.
- Die Bissrate im Spiel kann sich außerdem richten nach:
	1. Der historischen Bissrate des Spielers.
	2. Einer vollkommen zufälligen Wahrscheinlichkeit.

### Fangrate

Wie der Name schon sagt: Die Fangrate bezeichnet die Wahrscheinlichkeit, den Fisch am Ende tatsächlich zu fangen.

- Die **Fangrate** des Spiels wird gemeinsam durch folgende Faktoren bestimmt:
	- Ob der Fisch angebissen hat.
	- Der Zeitpunkt des Anhebels (nicht zu früh, nicht zu spät).
	- Die Reißfestigkeit der Angelschnur.
	- Die Größe des Angelhakens.

### Angelrute

- Die Angelrute besteht aus **Rutenschaft**, **Schwimmer**, **Angelhaken** und **Angelschnur**.
- Jedes Teil der Angelrute hat eine **Haltbarkeit**; je niedriger die Haltbarkeit, desto höher die Wahrscheinlichkeit, dass die Rute beschädigt wird. Ist die Rute beschädigt, muss das beschädigte **Teil ausgetauscht** werden.

#### Rutenschaft

- Der **Rutenschaft** ist ein Bestandteil der **Angelrute**.
- Der Spieler kann über das **Handelssystem** Angelruten kaufen, zum Beispiel eine 2,7-Meter-Rute und eine 3,6-Meter-Rute.
- Angelruten unterschiedlicher Länge haben unterschiedliche Auswurf- und Anhebezeiten.

#### Schwimmer

- Der **Schwimmer** ist ein Bestandteil der **Angelrute**; der Spieler kann anhand der **Schwimmbewegungen** des Schwimmers entscheiden, ob er die Rute anhebt.
- Der Spieler kann über das **Handelssystem** Schwimmer kaufen, zum Beispiel einen gewöhnlichen Schwimmer und einen Leucht-Schwimmer.
- Bei unterschiedlichen Fischarten bewegt sich der Schwimmer beim Anbeißen unterschiedlich; dies orientiert sich an den realen Schwimmbewegungen beim Anbeißen.
- Der Schwimmer kann in seiner **Tauchtiefe** verstellt werden (das heißt, das Gewicht des Bleis wird angepasst), damit der Spieler ihn besser beobachten kann.

#### Angelhaken

- Der **Angelhaken** ist ein Bestandteil der **Angelrute** und die Grundlage dafür, dass der Spieler Fische fängt.
- Der Spieler kann über das **Handelssystem** Angelhaken kaufen, zum Beispiel kleine und große Angelhaken.
- Die Größe des Angelhakens ist entscheidend dafür, ob der Spieler große oder kleine Fische fangen kann.
- Am Angelhaken kann **Köder** befestigt werden.

#### Angelschnur

- Die **Angelschnur** ist ein Bestandteil der **Angelrute**.
- Der Spieler kann über das **Handelssystem** Angelschnüre kaufen, zum Beispiel eine gewöhnliche 0,8er-Schnur und eine hochwertige 2,0er-Schnur.
- Verschiedene Angelschnüre haben unterschiedliche **Reißfestigkeiten**; diese kann gemeinsam durch folgende Faktoren bestimmt werden:
	- Die Qualität der Angelschnur.
	- Die Nutzungsdauer oder Haltbarkeit der Angelschnur.

### Köder

- Der Spieler kann über das **Handelssystem** Köder kaufen, zum Beispiel gewöhnlichen Köder und rote Regenwürmer.
- Wird ein pulverförmiger Köder gekauft, muss er erst durch Schritte wie Wasserzugabe und Kneten zu einem Köder verarbeitet werden.
- Verschiedene Köder haben unterschiedliche **Bissraten**.
- Als Verbrauchsmaterial gilt: Wenn der Spieler keinen Köder mehr besitzt und die Anzahl der Muscheln (einschließlich der Muscheln aus dem Fischverkauf) nicht ausreicht, um eine Packung Köder zu kaufen, erhält der Spieler am nächsten Tag eine kostenlose Nachlieferung im **Briefkasten**.

### Anfütterung

- Der Spieler kann über das **Handelssystem** Anfütterung kaufen, zum Beispiel fermentierten Tofutrester und alten Mais in Schnaps eingelegt.
- Verschiedene Anfütterungen haben unterschiedliche **Bissraten**.
- Anfütterung kann die Bissrate enorm erhöhen.

### Stirnlampe

- Der Spieler kann über das **Handelssystem** Stirnlampen kaufen, zum Beispiel eine gewöhnliche Stirnlampe und eine blaue Nachtangel-Lampe.
- Verschiedene Stirnlampen haben unterschiedliche **Bissraten** und unterschiedliche visuelle Effekte.
- Nachts ermöglicht die Stirnlampe dem Spieler, die Wasserfläche und den Schwimmer zu sehen.
- Nachts kann die Stirnlampe den Fischschwarm aufschrecken und die Bissrate senken.

### Sammelstücke

- Sammelstücke lassen sich hauptsächlich in **Flaschenpost**, **Souvenirs** und **Handlungsfragmente** unterteilen.
- Der Spieler kann Sammelstücke auf folgende Wegen **erhalten**:
	- Angeln.
	- Geschenke von Cat.

#### Flaschenpost

- In der Flaschenpost befinden sich **Briefe**.
- Die meisten Briefe sind **Ermutigungen für die Seele**, um den Spieler zu motivieren.

#### Souvenirs

- Ein Teil der Souvenirs kann im **Zelt** **aufgestellt** werden.

#### Handlungsfragmente

- Handlungsfragmente können genutzt werden, um den Spieler zu den Geschichten der **Dorfbewohner** zu führen.
- Wenn alle Handlungsfragmente gesammelt sind, kann der Spieler eine lange Handlung freischalten, um die Geschichten der **Dorfbewohner** vollständig und detailliert kennenzulernen.

---

## 🍳 Kochsystem

Stelle **Speisen** her und versuch, sie zu essen!

### Kochgeräte

- Die Kochgeräte bestehen aus drei Teilen: **Herd**, **Schneidebrett** und **Kochutensilien**.

#### Herd

- Der Herd dient zum **Erhitzen** von Speisen.
- Der Herd kann sich **befinden**:
	1. Im Zelt.
	2. Außerhalb des Zelts, aber in der Nähe des Zelts.
- Der Herd bietet Platz für einen Teil der **Kochutensilien** (wie eine Pfanne).
- Vor der Benutzung des Herds muss **Brennstoff** in den Herd gegeben werden.
- Der Spieler muss die **Hitze kontrollieren**, um sicherzustellen, dass die zubereiteten Speisen genießbar sind.

#### Schneidebrett

- Das Schneidebrett dient zum **Zerkleinern** von Speisen.
- Auf dem Schneidebrett können ein Teil der **Zutaten** (wie Chinakohl) und **halbfeite Speisen** abgelegt werden.
- Der Spieler kann mit einem Teil der **Kochutensilien** (wie einem Küchenmesser) auf dem Schneidebrett schneiden.

#### Kochutensilien

- Kochutensilien ermöglichen dem Spieler, Zutaten bequem zu **verarbeiten**.
- Zu den Kochutensilien gehören:
	- Großer Topf.
	- Pfanne.
	- Dampfeinsatz.
	- Porzellanschüssel.
	- Küchenmesser.
	- Nudelholz.

### Rezepte

- Der Spieler kann Speisen nach **Rezept** zubereiten. In der Regel gelingt die Zubereitung, wenn man sich an das Rezept hält.
- Der Spieler kann auch **vom Rezept abweichen** und frei improvisieren.

### Speisen

- Wenn der Spieler den gesamten **Zubereitungsablauf** abgeschlossen hat, erhält er die **Speise**.
- Der Spieler kann folgende Speisen herstellen:
	- Nackte Nudeln (erhältlich über den gesamten Ablauf vom Mehl über das Kneten und Schneiden der Streifen bis zum Kochen im Topf).
	- Dampfbrötchen (erhältlich über den gesamten Ablauf vom Mehl über das Kneten, Ausrollen der Hüllen, Herstellen der Füllung, Formen der Brötchen bis zum Dämpfen).
	- Spiegelei (erhältlich über den gesamten Ablauf vom Aufschlagen des Eis über das Anzünden des Feuers bis zum Wenden).
	- Gegrillter Fisch (erhältlich durch das Grillen von Fisch am Lagerfeuer).
	- Unbeschreibliches Ding (erhältlich, wenn die Zubereitung einer Speise fehlschlägt).
	- Holzkohle (erhältlich, wenn man nicht nach Rezept kocht und die Zubereitung fehlschlägt).

### Verzehr

- Wenn der Spieler eine **Speise** zubereitet hat, kann er versuchen, sie zu essen.
- Beim Essen kann der Spieler auf das entsprechende **Lebensmittel** oder **Bestandteil des Lebensmittels** klicken, um es zu essen.
- Wenn der Spieler eine **Speise** isst, ertönt ein wohliger **Soundeffekt**, es erscheint ein heilsamer **Text**, und das Lebensmittel oder sein Bestandteil **verschwindet** per Animation, um den Verzehr darzustellen.
- Besonderes: Wenn der Spieler das **Unbeschreibliche Ding** isst, kann mit einer gewissen Wahrscheinlichkeit Folgendes eintreten:
	1. Der Charakter fällt in Ohnmacht und erwacht nach einer Weile wieder.
	2. Der Charakter hat eine Weile lang einen visuellen Übelkeitseffekt.
	3. Es passiert gar nichts.

---

## ⛺️ Lagersystem

Nur das **Zelt** kann Geborgenheit schenken!

### Lagerung

- Im **Zelt** kann der Spieler die eigenen **Gegenstände** einsehen.
- Zu den **eigenen** Gegenständen des Spielers gehören:
	- Fische.
	- Sammelstücke.
	- Angelausrüstung.
	- Feldfrüchte.
- Ein Teil der Gegenstände (wie ein Teil der Sammelstücke) kann **aufgestellt** werden.

### Errungenschaften

- Im **Zelt** kann der Spieler die errungenen **Errungenschaften** einsehen.

### Bett

- Bei **Sonnenuntergang** und **nachts** kann der Spieler durch Klicken auf das Bett **schlafen**, um die Nacht zu überspringen.
- Der Spieler wacht am nächsten Tag beim **Sonnenaufgang** oder am **Vormittag** auf; er kann auch wählen, „**noch ein wenig zu schlafen**“ und weiterzuschlafen.

### Emotions-Recycling-Behälter

- Dieser Behälter, der wie ein Recyclingbehälter aussieht, ermöglicht es dem Spieler, die im **realen Leben** erlebten unschönen Dinge aufzuschreiben, sie zu einem Knäuel zu formen und in den Emotions-Recycling-Behälter zu werfen!

### Tagebuch

- Der Spieler kann im **Tagebuch** die Erlebnisse jedes Tages aufschreiben (ob aus dem Spiel oder aus dem realen Leben).
- Das Spiel erlaubt es dem Spieler, bestimmte Seiten des **Tagebuchs** in einen **festgelegten Ordner** zu exportieren, um sie zu teilen.

### Album

- Das Album zeigt alle **Werke**, die der Spieler auf dem **Zeichenpapier** angefertigt hat.
- Das Album kann als einzelne Datei in einen **festgelegten Ordner** exportiert werden, um sie zu teilen.

---

## 🐚 Handelssystem

Ist diese Melone reif?

### Kaufen

- Der Spieler kann auf dem **Markt** Waren kaufen.
- Auf dem Markt kann der Spieler mit **Dorfbewohnern** verschiedener Berufe sprechen.
- Beim **Sprechen** mit den Dorfbewohnern kann mit einer gewissen Wahrscheinlichkeit eine **Sonderhandlung** ausgelöst werden; ist diese Sonderhandlung abgeschlossen, kann der Preis **gesenkt** werden.
- Der Spieler kann auf dem Markt folgende **Arten** von Waren kaufen:
	- Angelausrüstung (wie Angelruten).
	- Pflanzensamen (wie Weizensamen).
	- Verarbeitete Feldfrüchte (wie Mehl).
	- Gemüse (wie Chinakohl).
	- Brennstoffe (wie Holzkohle).
	- Speisewürzen (wie Salz).
	- Zeichenpapier (wie 1:1-Zeichenpapier).
	- Briefmarken.

### Verkaufen

- Der Spieler kann auf dem **Markt** Waren verkaufen.
- Der Spieler kann auf dem Markt folgende **Arten** von Waren verkaufen:
	- Fische.
	- Einen Teil der Sammelstücke.
- Beim Verkauf von Fischen gilt der **Tagesfischpreis** als Preisgrundlage.
- Der **Tagesfischpreis** unterscheidet zwischen **frischem Fisch** und **Lagerbestand**; keine der beiden Preisarten bleibt unverändert. Der Tagesfischpreis kann gemeinsam durch folgende Faktoren bestimmt werden:
	- Das Spielwetter.
	- Die Spieljahreszeit.
	- Ein Zufallswert innerhalb eines festen Wertebereichs.

### Währung

- Das Spiel verwendet **Muscheln** als Währung.
- Der Spieler kann Muscheln auf folgende Wegen **erhalten**:
	- Handel.
	- Angeln.
	- Geschenke von Cat.

---

## 🌽 Pflanzensystem

**Pflanzen anbauen**, **gießen und düngen** und **ernten**.

### Pflanzen

- Zum Anpflanzen von Feldfrüchten muss man **Pflanzensamen** besitzen.
- Der **Ablauf** des Pflanzens ist wie folgt: Boden glätten, Samen ausstreuen, mit Erde bedecken, gießen, düngen.
- Bedingungen für das Keimen der Samen: **ausreichende Feuchtigkeit**, **geeignete Temperatur** und **genügend Sauerstoff**.
- Beim Pflanzen muss der Spieler **beachten**:
	- Das Spielwetter.
	- Die Spieljahreszeit.

### Wachstum

- Während des Wachstums der Feldfrüchte muss der Spieler ununterbrochen **gießen** und **düngen**.
- Die Feldfrüchte wechseln nach einer gewissen Zeit (etwa 90 Stunden) ihren **Wachstumszustand**.

### Ernte

- Wenn die Feldfrüchte **vollständig ausgereift** sind, kann der Spieler die **Feldfrüchte** und die **Pflanzensamen** ernten.

---

## 🐱 CatGPT

Plausch ein wenig mit dem Kätzchen oder **kraule die Katze** ฅ՞•ﻌ•՞ฅ.

### Chatten

- Der Spieler kann Cat **Nachrichten** schicken.
- Cat wird dem Spieler anhand bestimmter Gewichtungen **antworten**; die Gewichtungen können sich richten nach:
	1. Der Anzahl der vom Spieler gesendeten Zeichen.
	2. Einer vollkommen zufälligen Wahrscheinlichkeit.
- Cat antwortet mit „**Meow**“ in verschiedenen Tonlagen und Klangfarben, um dem Spieler emotionale Wärme zu schenken.

### Katze kraueln

- Der Spieler kann Cat am **Kopf** leicht berühren, um sie zu kraueln.
- Beim Kraueln fliegen „**Meow**“-Schriftzüge wie Kommentare von Cat weg, begleitet von „**Meow**“-Lauten in verschiedenen Tonlagen und Klangfarben, die dem Spieler emotionale Wärme schenken.

### Geschenke

- Cat kann dem Spieler am nächsten Morgen beim Aufwachen ein **Geschenk** überreichen.
- Ob Cat dem Spieler ein **Geschenk** überreicht, kann sich richten nach:
	1. Der Anzahl der Gespräche mit Cat oder des Krauelns am Vortag.
	2. Der Gesamtzahl der bisherigen Gespräche mit Cat oder des Krauelns.
	3. Einer vollkommen zufälligen Wahrscheinlichkeit.
- Die **Arten** der Geschenke können umfassen:
	- Fische.
	- Muscheln.
	- Einen Teil der Sammelstücke (sehr geringe Wahrscheinlichkeit).

### Es könnte auch …

- Neben Cat kann der Spieler auch **andere Objekte** zum Sprechen oder Kraueln wählen. Diese **anderen Objekte** könnten **Mitglieder der Entwicklungsgruppe** sein, die in der **Handlung zur Einführung** auftauchen.

---

## 🖌️ Zeichensystem

Male mit wahrhaftigem Papier und Farben und speichere deine Werke.

### Zeichenpapier

- Das Zeichenpapier verhält sich wie echtes Papier: Es erlaubt **Verlaufen**, **mehrfaches Übermalen** und **Farbmischen**.
- Der Spieler kann über das **Handelssystem** Zeichenpapier kaufen, zum Beispiel 1:1-Zeichenpapier und 3:4-Zeichenpapier.

### Farbpalette

- Standardmäßig werden 8 Grundfarben bereitgestellt; der Spieler kann mit dem **Pinsel** Farbe aufnehmen und auf der **Farbpalette** mischen.
- Das Mischverfahren kann **Aquarell** oder **Gouache** sein.
- Beim Mischen werden zwei Farben mit dem **Pinsel** vermengt; nicht gemischte Farben behalten ihre Ursprungsfarbe, und der Mischton hängt vom Grad der Vermischung durch den Spieler ab.

### Pinsel

- Der Pinsel kann Farbe oder Wasser auf das Zeichenpapier **auftragen**.

### Speichern

- Die Werke des Spielers werden im **Album** **gespeichert**.
- Der Spieler kann Werke in einen **festgelegten Ordner** **exportieren**, um sie zu teilen.

---

## 📬 Briefkastensystem

**Post** empfangen und versenden.

### Post empfangen

- Der Spieler kann folgende E-Mails **erhalten**:
	- Briefe, die der Spieler an sich selbst geschickt hat.
	- Kostenlose Köder-Nachlieferungen.
	- Festtagsgrüße.
	- Geburtstagsgrüße.

### Post versenden

- Der Spieler kann folgende E-Mails **versenden**:
	- Briefe an das eigene zukünftige Ich.
- Beim Versenden muss auf der E-Mail eine **Briefmarke** angebracht sein.

---

## 📺 Visuelle Oberfläche

Flüssige **nichtlineare Animationen** schenken dem Spieler stets ein angenehmes visuelles Erlebnis.

### Bedienelemente

- Bedienelemente können **Interaktionshandlungen und Ereignisse auslösen**.
- Die Bedienelemente sollten dem Designstil von „Today@PolarBay“ entsprechen.
- Beim **Drücken** sollten die Bedienelemente sofort schrumpfen und dann nichtlinear zurückfedern.
- Die **Position** und **Größe** der Bedienelemente kann angepasst werden.

### Karten

- Karten können nicht **interagiert** werden.
- Die Karten sollten dem Designstil von „Today@PolarBay“ entsprechen.
- Karten dienen zur Darstellung relativ **aufgeräumter** Hintergründe, zum Beispiel der Inventaroberfläche.

### Augenschonender grüner Bildschirm

- Da der Spieler beim **Angeln** über **lange Zeit** auf den **Schwimmer** starren muss, wurde eigens der **augenschonende grüne Bildschirm** entworfen.
- Der augenschonende grüne Bildschirm überzieht in regelmäßigen Abständen den **gesamten Bildschirm**, um den Spieler zur **erzwungenen Pause** zu bringen.
- Die **Intervalldauer** und die **Überlagerungsdauer** des augenschonenden grünen Bildschirms können in den Einstellungen angepasst oder ein- und ausgeschaltet werden.
- Der augenschonende grüne Bildschirm zeigt den Inhalt der **Briefe** aus den **Flaschenposten**, die der Spieler gesammelt hat.

### Farbkonzepte

- Das Spiel kann **zwei** Farbkonzepte enthalten: ein weißes und ein schwarzes.
- Der Wechsel zwischen weißem und schwarzem Konzept kann sich richten nach:
	1. Der Tages- und Nachtzeit in der Realität.
	2. Der Tages- und Nachtzeit im Spiel.
	3. Der manuellen Anpassung durch den Spieler in den Einstellungen.

### Partikeleffekte

- Partikeleffekte werden von **besonderen Ereignissen** erzeugt, zum Beispiel wenn ein Boot über die Wasserfläche fährt.
- Partikeleffekte können in den **Einstellungen** in Anzahl und Ein-/Aus-Zustand angepasst werden, um Leistungsprobleme zu vermeiden.

### Hochwertiges Material

- Das hochwertige Material ist das **Acryl-Material**.
- Der Spieler kann das hochwertige Material in den **Einstellungen** ein- oder ausschalten.
- Ist das hochwertige Material aktiviert, werden die **leeren Bereiche** der GUI wie Bedienelemente und Karten zu halbtransparenten, unscharfen Flächen.

---

## 🕒 Zeitsystem

Die **Zeit** vergeht immer so schnell, dass wir vieles verpassen.

### Zeitumrechnung

- Ein **Tag** im Spiel entspricht einer **Stunde** in der Realität.
- Das Umrechnungsverhältnis zwischen Spielzeit und Realzeit beträgt **1:24**.

### Zeitabschnitte

- **Tag** und **Nacht** im Spiel dauern jeweils **30 Minuten**.
- Innerhalb eines **Tages** (60 Minuten) ist das Spiel in folgende Zeitabschnitte unterteilt:
	- Sonnenaufgang: Minute 1–2.
	- Vormittag: Minute 2–10.
	- Mittag: Minute 11–20.
	- Nachmittag: Minute 21–28.
	- Sonnenuntergang: Minute 29–30.
	- Nacht: Minute 31–60.

---

## 💾 Speichersystem

**Speichere** den aktuellen **Spielstand**, damit unsere Fische und unser Salz sicher sind.

### Speichern

- Auf der **Speichern**-Seite kann der Spieler auf die Schaltfläche **Speicherstand holen** klicken, um den aktuellen Stand zu **speichern**.
- Auf der **Speichern**-Seite kann der Spieler auf die Schaltfläche **Speicherstand laden** klicken, um einen gespeicherten Stand zu **laden**.
