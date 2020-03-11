# DemoFX: JavaFX kant-en-klaar voor IntelliJ

# Hoe maak je dit project zelf in Intelli?
1. IntelliJ > Create New Project > Java > Next > Next > Kies projectnaam > Finish
2. File > Project Structure > Libraries > + > From Maven > org.openjfx:javafx-fxml:13 & V Download To 'projectdir/lib' > OK > OK > OK
3. File > Project Structure > Libraries > + > From Maven > org.junit.jupiter:junit-jupiter:5.4.2 & V Download To 'projectdir/lib' > OK > OK > OK
4. Rechtermuisklik op je project > New > Directory > 'test' > Enter
5. Rechtermuisklik op de nieuwe directory > Mark Directory as > Test Sources root
6. Creëer in de src-folder de packages 'demo.model' en 'demo.userinterface'
7. Plaats in de demo package de klasse App.java (rechtermuisklik op de package > New > Java Class)
8. Plaats in de demo.userinterface package de klasse MainscreenController (rechtermuisklik op de package > New > Java Class)
9. Plaats in de demo.userinterface package de FXML-pagina Mainscreen (rechtermuisklik op de package > New > FXML File)
9. Rechtermuisklik op je project > New > File > '.gitignore'. Ignore de /lib/ en /out/ folders (beide op één regel).
10. Menu VCS > Import into Version Control > Create Git repository... > OK
11. Menu Run > Edit Configurations > + > Application > Geef deze configuratie de naam 'App', vink de checkbox 'Share through VCS' aan, kies als Main-class demo.App, en als VM-options: '--module-path lib --add-modules javafx.fxml,javafx.controls'!
