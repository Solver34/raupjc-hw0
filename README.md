# raupjc-hw0

# Pitanje 1:
U sadržaju mape Bin/Debug nakon dodavanja class library kao reference konzolne aplikacije uočavam dvije nove datoteke: Class1.dll te Class1.pdb. Brisanjem tih .dll datoteke program javlja grešku (Could not load file or assembly 'ClassLibrary1') koja je posljedica toga da koristimo metodu iz nepostojece biblioteke koju smo prethodno izbrisali. Kada ne bi koristili metodu iz te biblioteke, program ne bi javljao gresku pri pokretanju. Pri slanju programa, osim .exe datoteke, poslao bih i sve .dll datoteke.

# Pitanje 2:
Nakon izmjene stringa u PrintHelloWorld metodi, pri pokretanju .exe datoteke prikazuje se stari string. Razlog tome je taj što sam nakon izmjene stringa projekt spremio, ali ga nisam buildao. Budući da se .dll datoteke mijenjaju tek nakon buildanja solutiona, pokretanje aplikacije je dovelo do ispisivanja starog stringa.

# Pitanje 3:
Nakon brisanja mape NodaTime.2.2.1 unutar direktorija packages, Visual Studio je svejedno uspio buildat solution te je vratio NodaTime.2.2.1 u direktorij packages.
