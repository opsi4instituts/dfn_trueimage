Die initiale Version dieses Pakets wurde von Eric Esser, Wissenschaftszentrum Berlin für Sozialforschung, erstellt und auf dem DFN-Repository der Initiative OPSI4instituts veröffentlicht: https://opsi.wzb.eu
Kontakt, sowie Fragen und Anregungen: eric.esser@wzb.eu / opsi@wzb.eu

VORAUSSETZUNGEN:
- Besitz einer TrueImage Lizenz

HOWTO
1. Im True Image einen Rettungsstick erstellen.

Variante A: Ins Paket packen, z.B. bei verteilter Infrastruktur mit mehreren OPSI-Servern
  1. Entpacken des Pakets: am Besten in der Workbench (standardmäßig unter /home/opsiproducts/) das Paket hinterlegen und dann in der Kommandozeile "opsi-package-manager -x desinfect_2015-1.opsi" ausführen"
  2. In den dadurch erstellten Ordner /home/opsiproducts/dfn_trueimage/SERVER_DATA/tftpboot/linux/trueimage die Dateien dat2.dat und dat3.dat aus dem Wurzelverzeichnis des TrueImage-Rettungssticks kopieren.
  3. Die Datei dat2.dat in ramdisk.dat und die Datei dat3.dat in kernel.dat umbenennen.
  4. Wieder verpacken des Pakets: in /home/opsiproducts/dfn_desinfect/ "opsi-makeproductfile" auf der Kommandozeile ausführen. Dabei die Version beibehalten und "O" wählen. 
  5. Installieren des Pakets durch Ausführen von "opsi-package-manager -i -p ask desinfect_2015-1.opsi" in der Kommandozeile ausführen.
  
Variante B: TrueImage-Dateien nachträglich auf den Server kopieren
  1. Die Dateien dat2.dat und dat3.dat aus dem Wurzelverzeichnis des TrueImage-Rettungssticks nach /tftpboot/linux/trueimage kopieren.
  2. Die Datei dat2.dat in ramdisk.dat und die Datei dat3.dat in kernel.dat umbenennen.


