# Lern-Bericht
von Flynn Guerra

## Einleitung

In diesem Lernbericht geht es darum, wie man eine Session-ID in JSF anzeigen kann.

## Was habe ich gelernt?

Ich habe in diesem Projekt gelernt wie man eine SessionID durch Java code generiert und dann in JSF anhand einer xhtml anzeigen kann.

## Beschreibung

✍️ Verwenden Sie drei verschiedene Medien, um zu zeigen, was Sie gelernt haben. Zum Beispiel:

* Eine textliche Beschreibung
* Ein deutliches, aussagekräftiges Bild oder eine kommentierte Bildschirm-Aufnahme
* Ein gut dokumentierter Code-Fetzen
* Ein Link zu einem *selbst aufgenommenen* youtube-Video oder `.gif`.

```Java
    public String getSessionID() {
        FacesContext fCtx = FacesContext.getCurrentInstance();
        HttpSession session = (HttpSession) fCtx.getExternalContext().getSession(false);
        return session.getId();
    }
```

## Verifikation

✍️ Erklären Sie kurz und bündig, inwiefern die von Ihnen verwendeten Medien zeigen, was Sie gelernt haben.

# Reflektion zum Arbeitsprozess

👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief; 

👎 und etwas, was nicht gut lief.

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.
