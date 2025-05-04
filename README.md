# Mein erster KI-Workflow mit n8n und DeepSeek 

Ich habe zum ersten Mal einen vollständigen Automatisierungs-Workflow mit **KI-Unterstützung** gebaut – und das Beste: **die KI hat mir dabei geholfen, sich selbst einzubinden**. 


## Was macht der Workflow überhaupt?

Ich habe mit **n8n** einen KI-gesteuerten Flow erstellt, der Folgendes tut:

1. **Trigger**: Sobald ich meinem eigenen Telegram-Bot eine Nachricht schreibe (z. B. „lies meine email“), startet der Prozess.

2. **Gmail Node**: Der Flow greift automatisch auf mein Gmail-Postfach zu und holt sich die **10 neuesten E-Mails** aus dem Posteingang.

3. **Texte zusammenführen**: Diese 10 E-Mails werden mit einem **Function Node** (bzw. Aggregate-Technik) zu **einem großen Textblock** zusammengeführt.

4. **DeepSeek-Verbindung**:  
   Der kombinierte Text fließt in einen **HTTP Request Node**, der mit **DeepSeek AI** verbunden ist.  
   Die Kommunikation läuft über einen **API Key**, und die E-Mail-Daten werden über ein **sauber formatiertes JSON im Body** gesendet.

5. **Zusammenfassung**:  
   DeepSeek analysiert den Text und erstellt daraus eine **kompakte Zusammenfassung** der wichtigsten Inhalte.

6. **Antwort per Telegram**:  
   Die KI-Antwort landet automatisch wieder in Telegram – direkt in meinem Chat mit dem Bot. So bekomme ich meine Zusammenfassung sofort zurück. 


## Warum habe ich das gemacht?

- Kein manuelles E-Mails durchlesen mehr  
- KI übernimmt das Denken – ich nur noch das Lesen  
- Alles läuft vollautomatisch, sobald ich eine Nachricht schicke


Ich bin super zufrieden mit dem Ergebnis. Es war mein erster richtiger Workflow.

**Und das alles mit Hilfe der KI selbst.** 

