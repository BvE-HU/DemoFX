# DemoFX: JavaFX kant-en-klaar voor IntelliJ
Je kunt dit IntelliJ-project Git-clonen en openen met IntelliJ. Het project is direct klaar voor gebruik.

# Hoe maak je dit project zelf in Intelli?
1. IntelliJ > Create New Project > Java > Next > Next > Kies projectnaam > Finish
2. File > Project Structure > Libraries > + > From Maven > org.openjfx:javafx-fxml:13 & V Download To 'projectdir/lib' > OK > OK > OK
3. File > Project Structure > Libraries > + > From Maven > org.junit.jupiter:junit-jupiter:5.4.2 & V Download To 'projectdir/lib' > OK > OK > OK
4. Rechtermuisklik op je project > New > Directory > 'test' > Enter
5. Rechtermuisklik op de nieuwe directory > Mark Directory as > Test Sources Root
6. Creëer in de src-folder de packages 'demo.model' en 'demo.userinterface'
7. Plaats in de demo package de klasse App.java (rechtermuisklik op de package > New > Java Class)
8. Plaats in de demo.userinterface package de klasse MainscreenController (rechtermuisklik op de package > New > Java Class)
9. Plaats in de demo.userinterface package de FXML-pagina Mainscreen (rechtermuisklik op de package > New > FXML File)
10. Rechtermuisklik op je project > New > File > '.gitignore'. Ignore de /lib/ en /out/ folders (beide op één regel).
11. Menu VCS > Import into Version Control > Create Git repository... > OK
12. Rechtermuisklik op de .idea directory > Git > Add (> Add)
13. Rechtermuisklik op de src directory in je project > Git > Add (> Add)
14. Rechtermuisklik op de .iml file in je project > Git > Add (> Add)
15. Rechtermuisklik op de .gitignore file in je project > Git > Add (> Add)
16. Menu Run > Edit Configurations > + > Application > Geef deze configuratie de naam 'App', vink de checkbox 'Share through VCS' aan, kies als Main-class demo.App, en als VM-options: '--module-path lib --add-modules javafx.fxml,javafx.controls'!
17. Menu VCS > Commit en commit al je bestanden onder vermelding van 'Initial commit'

18. Optioneel: menu VCS > Import into Version Control > Share Project on Github om je project met de wereld te delen! 
