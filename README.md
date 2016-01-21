# fastd-peers-clients
Fastd Whitelists für die Segmente

Im ersten Schritt ist Segment 02 für Aachen Stadt und Segment 03 für die Regio. Eine weitere Aufteilung in 10 Segmente ist in der Firmware vorbereitet, aber für die Testphase nicht praktikabel.

Pro FastdD Key eine Datei, der Dateiname soll mit der NodeID wie sie in MeshVierwer zu finden ist beginnen und nach einem - zur Trennung als zweiten Teil den Nodenamen enthalten.

Ob dies praktikabel ist wird sich zeigen. Möglicherweise sollte auf den Nodenamen verzichtet werden.

Inhalt der Datei ist nur eine Zeile:
> key "\<public-fastd-key\>";
zu ermitteln z.B. über SSH auf dem Router mit:
    # /etc/init.d/fastd show_key mesh_vpn
    18fa75d1808692f04770bedf30c42dac24585d331560c545d70dd27f22a05648

Es könnten auch Kommentarzeilen beginnen mit # eingefügt werden, z.B. für den Nodenamen, meshpartner oder die Koordinaten.

Zusätzlich existiert ein Ordner blacklist, wie der Name vermuten lässt schaltet er nicht für ein bestimmtes Segment frei, sonder dient lediglich dazu Knoten fürs default Segment zu sperren.
