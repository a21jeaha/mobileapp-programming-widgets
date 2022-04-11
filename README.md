
# Rapport

**Widget Labb**

En constraint layout som har en vit färg, den kommer agera som grund för resten av applikationen. Därför sätts des constraints längst med kanterna av applikationen. 
```
<androidx.constraintlayout.widget.ConstraintLayout>

```

Nya färg resources i colors.xml skapades, och kommer användas sedan.

```
<color name="veryLightBlue">#5F74FC</color>
<color name="white">#FFFFFF</color>
```
I constraint layouten som skapades innan skapas en LinearLayout med den blå färgen, denna kommer senare att innehålla resterande widgets. En generel margin angavs för att förminska storleken av den blå widgeten.
```
 <LinearLayout
            android:id="@+id/widget_window_Background"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_margin="10dp"
            android:background="@color/veryLightBlue"

            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintEnd_toEndOf="parent"
            app:layout_constraintStart_toStartOf="parent"
            app:layout_constraintTop_toTopOf="parent">
  </LinearLayout>
 
```
Det skapdes sedan en TextView som placerades innanför LinearLayouten, I denna ruta skrev en liten kort textsträng som centrerades med hjälp av `android:gravity="center"` texten justerades sedan med hjälp av `android:textSize="" android:textStyle=""`.
Brädden för fönstret sattses efter dess förälder men med en generel magrin på 10dp för att ge den blå bakgrunden chansen att träda fram och sist ändrades bakgrundsfärgen till vit. 
```
<TextView
         android:id="@+id/text_window"
         android:layout_width="match_parent"
         android:layout_height="200dp"
         android:background="@color/white"
         android:layout_margin="10dp"
         android:text="@string/write_somthing_here"
         android:textSize="20sp"
         android:textStyle="italic"
         android:gravity="center"
         />
```
En ImageView skapades sedan där en bild som placerats i mappen **drawable** användes, den 
```
    <ImageView
        android:id="@+id/image"
        android:layout_width="250dp"
        android:layout_height="250dp"
        android:layout_gravity="center"
        android:src="@drawable/helloworld"
        />
```

_Du kan ta bort all text som finns sedan tidigare_.

## Följande grundsyn gäller dugga-svar:

- Ett kortfattat svar är att föredra. Svar som är längre än en sida text (skärmdumpar och programkod exkluderat) är onödigt långt.
- Svaret skall ha minst en snutt programkod.
- Svaret skall inkludera en kort övergripande förklarande text som redogör för vad respektive snutt programkod gör eller som svarar på annan teorifråga.
- Svaret skall ha minst en skärmdump. Skärmdumpar skall illustrera exekvering av relevant programkod. Eventuell text i skärmdumpar måste vara läsbar.
- I de fall detta efterfrågas, dela upp delar av ditt svar i för- och nackdelar. Dina för- respektive nackdelar skall vara i form av punktlistor med kortare stycken (3-4 meningar).

Programkod ska se ut som exemplet nedan. Koden måste vara korrekt indenterad då den blir lättare att läsa vilket gör det lättare att hitta syntaktiska fel.

```
function errorCallback(error) {
    switch(error.code) {
        case error.PERMISSION_DENIED:
            // Geolocation API stöds inte, gör något
            break;
        case error.POSITION_UNAVAILABLE:
            // Misslyckat positionsanrop, gör något
            break;
        case error.UNKNOWN_ERROR:
            // Okänt fel, gör något
            break;
    }
}
```


Bilder läggs i samma mapp som markdown-filen.

![](android.png)

Läs gärna:

- Boulos, M.N.K., Warren, J., Gong, J. & Yue, P. (2010) Web GIS in practice VIII: HTML5 and the canvas element for interactive online mapping. International journal of health geographics 9, 14. Shin, Y. &
- Wunsche, B.C. (2013) A smartphone-based golf simulation exercise game for supporting arthritis patients. 2013 28th International Conference of Image and Vision Computing New Zealand (IVCNZ), IEEE, pp. 459–464.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A. (2012) Experimentation in Software Engineering, Berlin, Heidelberg: Springer Berlin Heidelberg.
