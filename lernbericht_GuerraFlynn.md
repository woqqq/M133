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

✍️ Erklären Sie kurz und bündig, inwiefern die von Ihnen verwendeten Medien zeigen, was Sie gelernt haben.

# Reflektion zum Arbeitsprozess

👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief; 

👎 und etwas, was nicht gut lief.

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.
