# Lern-Bericht
von Flynn Guerra

## Einleitung

In diesem Lernbericht geht es darum, wie man eine Session-ID in JSF anzeigen kann.

## Was habe ich gelernt?

Ich habe in diesem Projekt gelernt wie man eine SessionID durch Java code generiert und dann in JSF anhand einer xhtml anzeigen kann.

## Beschreibung
```Java
    public String getSessionID() {
        FacesContext fCtx = FacesContext.getCurrentInstance();
        HttpSession session = (HttpSession) fCtx.getExternalContext().getSession(false);
        return session.getId();
    }
```

```Xhtml
<h:outputLabel value="Ihre Sitzung wurde eröffnet: #{SitzVer.sessionID}" />
```
![sessionID](https://user-images.githubusercontent.com/69577267/186889480-f0416f4a-c379-4940-aaa9-ac38f254794b.png)

## Verifikation



# Reflektion zum Arbeitsprozess

# 👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief;
Die Arbeit an diesem Projekt im allgemeinen lief reibungslos ab. Der Code für das Auslesen der SessionID wurde uns in der Aufgabe vorgegeben und man musste diesen Code-Snippet nurnoch Korrekt anwenden, damit man die SessionID auf der Webseite angeben kann. Dies hat mir auch keine Probleme bereitet, da dass auslesen von Informationen aus dem Controller ein relativ einfacher Vorgang ist. Dieser Auftrag war ausserdem einer der wichtigeren, da es hier wichtig war die Grundprinzipien des Arbeiten mit JSF zu erlernen und zu "meistern".

# 👎 und etwas, was nicht gut lief.
Konkret an diesem Projekt gab es nur einen kleinen Fehler, da mir eine Datei gefehlt hat, welche bei der erstellung einer Web-Application auf Netbeans nicht direkt erzeugt wird. Diese Datei muss man selber erstellen oder aus vorherigen Projekten kopieren. In dieser Datei wird eine Startseite angegeben, sodass das Programm weiss, welche Datei halt gestartet wird.

**VBV**: Ich möchte Ihn Zukunft mich aufjedenfall noch mehr an dem Unterricht beteiligen und auch die Aufträge Konsequenter erledigen.
