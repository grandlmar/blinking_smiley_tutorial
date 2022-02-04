# smiley_tutorial

## Schritt 1
Am LED-Display des BBC micro:bit soll ein blinkendes ``||basic: Symbol||`` angezeigt werden.

Wähle im ersten Schritt ein Symbol aus und zeige es am LED Display des BBC micro:bit an. 

```blocks
basic.showIcon(IconNames.Heart)
```

## Schritt 2

Erweitere das Programm so, dass das Symbol nur für 2 Sekunden am LED Display angezeigt wird.
Danach soll es nicht mehr angezeigt werden.

Folgende Befehle können dir helfen:

```block
    basic.pause(2000)
```

```block
    basic.clearScreen()
```

## Schritt 3

So sollte dein Programm nun aussehen:

```blocks
basic.showIcon(IconNames.Heart)
basic.pause(2000)
basic.clearScreen()
```

## Schritt 4

Um ein blinkendes Symbol zu erzeugen, benötigst du noch eine Wiederholungsanweisung, 
auch ``||loops: Schleife||`` genannt. 

Am besten du verwendest eine Endlosschleife.
Das machst du mit diesem Befehl:

```block
basic.forever(function () {
	
})
```

## Schritt 5 

Führe das Programm aus, was fällt dir auf?

```blocks
basic.forever(function () {
basic.showIcon(IconNames.Heart)
basic.pause(2000)
basic.clearScreen()
})
```

## Schritt 6

Du benötigst noch einen ``||basic: Pausiere||``-Befehl an geeigneter Stelle. 

```block
basic.pause()
```
## Schritt 7

So kann das fertige Programm aussehen:

```blocks
basic.forever(function () {
basic.showIcon(IconNames.Heart)
basic.pause(1000)
basic.clearScreen()
basic.pause(1000)
})
```