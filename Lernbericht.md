# Lern-Bericht
Oltian Kadriu

## Einleitung

Wir lernen in diesem Modul wie man eine Web-Applikation mit Session-Handling realisiert.

## Was habe ich gelernt?

Ich habe gelernt, wie man Bild in JSF einbindet.

## Beschreibung

In JSF kann man den Tag <h:graphicImage /> verwenden, um ein HTML-Element "img" darzustellen. <br />
Im Projekt befindet sich ein Ressourcenordner namens "img", wo die Bilddatei "macbook.jpg" zu finden ist. <br />
Somit wollen wir, das Bild "macbook.jpg" darstellen. Um das zu tun, suchen wir im Code nach dem Ressourcenordner "img" und dem Bildnamen "macbook.jpg". 
Ausserdem geben wir dem Bild noch eine Bildbreite von 500, damit es nicht sehr gross im Browser erscheint.

```xhtml
<!-- JSF -->
<!-- Der Ressourcenordner "img" wird gesucht und darin die Bilddatei "macbook.jpg" -->
<h:graphicImage library="img" name="macbook.jpg" width="500"/>
```

![grafik](https://user-images.githubusercontent.com/69577043/187035871-db6577d1-8893-4447-ac01-59e3e1737e13.png)


```html
<!-- HTML output -->
<img src="/5.%20BildEinfuegenDemo/faces/javax.faces.resource/macbook.jpg;jsessionid=fd1d0defc21cadabd021082ad3c8?ln=img" width="500">
```

## Verifikation

Von der Beschreibung können Sie lesen, dass ich verstanden habe, wie man ein Bild in JSF einbindet. Ebenfalls sieht man am Code, dass ich dies anwenden kann. Der Screenshot vom Output bestätigt dies nochmals, denn er ist aus dem Code resultiert. Wie der Code sich von JSF zu HTML ändert, ist im zweiten Codeblock zu sehen.

# Reflektion zum Arbeitsprozess

Mit meiner Leistung in diesem Modul bin ich sehr zufrieden, denn ich konnte bisher alle Aufträge lösen. 

In einem Projekt musste ich die akutelle SessionID ausgeben, dabei war mein Code richtig, aber die SessionID wurde trotzdem nicht angezeigt. Damit habe ich dann mehrere Minuten verloren, bis ich meine Lehrperson fragen musste, wo der Fehler lag. Dabei lag der Fehler an dem Import oben im Code. Da meine Bean @SessionScoped war, muss auch ein passender Import gemacht werden und dabei wurden mir von NetBeans zwei vorgeschlagen und ich habe einfach das Erste genommen, was leider falsch war. Somit habe ich dann gelernt, dass ich den Import mit .enterprise nehmen muss.

**VBV**: Keinen
