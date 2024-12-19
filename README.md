# Portfolio-Projekt Dokumentation  
**Autor:** Dorian Herzig  

### **Versionierung**  
| Datum       | Version  | Zusammenfassung                    |
|-------------|----------|------------------------------------|
| 15.11.2025  | 0.1.0    | Projektstart, Planung abgeschlossen |
| 20.12.2025  | 1.0.0    | Projekt abgeschlossen             |

---

### **1. Informieren**  

#### **1.1 Projektziel**  
Erstellung einer Portfolio-Seite mit einer klar strukturierten REST-API, einem responsiven Frontend und der Integration des Mediator-Patterns.

#### **1.2 User Stories**  
| US-№ | Verbindlichkeit | Typ       | Beschreibung                                                  |
|------|-----------------|-----------|--------------------------------------------------------------|
| 1    | Muss           | Funktion  | Backend-API unterstützt CRUD-Funktionen                     |
| 2    | Muss           | Funktion  | Frontend ist vollständig responsiv                          |
| 3    | Kann           | Qualität  | Mediator-Pattern optimiert die Kommunikation zwischen Komponenten |

#### **1.3 Testfälle**  
| TC-№ | Ausgangslage       | Eingabe                        | Erwartete Ausgabe                                              |
|------|--------------------|--------------------------------|----------------------------------------------------------------|
| 1.1  | Datenbank leer     | GET /api/projects             | Leere Projektliste wird zurückgegeben                         |
| 2.1  | Datenbank mit Daten| GET /api/projects             | Liste gespeicherter Projekte wird angezeigt                   |
| 3.1  | Falsche Eingabe    | POST ungültige Daten           | Fehlerantwort: \"Ungültige Eingabe\"                          |

#### **1.4 Diagramme**  
✍️ Diagramme können hier eingefügt werden.

---

### **2. Planen**  

| AP-№ | Frist         | Zuständig       | Beschreibung                   | geplante Zeit |
|------|---------------|-----------------|---------------------------------|---------------|
| 1.A  | 17.11.2025    | Dorian Herzig   | Entwicklung des Backends       | 180 min       |
| 2.A  | 24.11.2025    | Dorian Herzig   | Entwicklung des Frontends      | 150 min       |
| 3.A  | 01.12.2025    | Dorian Herzig   | Implementierung Mediator-Pattern| 120 min       |

---

### **3. Entscheiden**  
- **Technologiewahl:** Verwendung von Node.js, Express und MongoDB für das Backend.  
- **Frontend-Technologien:** HTML, CSS, JavaScript für responsives Design.  
- **Mediator-Pattern:** Zur Optimierung der internen Kommunikation.  

---

### **4. Realisieren**  

| AP-№ | Datum        | Beschreibung                   | geplante Zeit | tatsächliche Zeit |
|------|--------------|---------------------------------|---------------|--------------------|
| 1.A  | 17.11.2025   | Entwicklung des Backends       | 180 min       | 160 min            |
| 2.A  | 24.11.2025   | Entwicklung des Frontends      | 150 min       | 140 min            |
| 3.A  | 01.12.2025   | Implementierung Mediator-Pattern| 120 min       | 130 min            |

---

### **5. Kontrollieren**  

#### **5.1 Testprotokoll**  
| TC-№ | Datum       | Resultat                                          | Tester         |
|------|-------------|--------------------------------------------------|----------------|
| 1.1  | 18.12.2025  | Funktioniert wie erwartet                        | Dorian Herzig  |
| 2.1  | 18.12.2025  | Ausgabe entspricht den gespeicherten Projekten   | Dorian Herzig  |
| 3.1  | 18.12.2025  | Fehler wird korrekt ausgegeben                   | Dorian Herzig  |

#### **5.2 Exploratives Testen**  
| BR-№ | Ausgangslage | Eingabe       | Erwartete Ausgabe                   | Tatsächliche Ausgabe |
|------|--------------|---------------|-------------------------------------|-----------------------|
| I    | Leere Datenbank | GET-Anfrage | Leere Liste                         | Leere Liste           |

---

### **6. Auswerten**  
Das Projekt wurde erfolgreich abgeschlossen. Der Mediator-Pattern-Einsatz war lehrreich und hat die Kommunikation deutlich verbessert. Verbesserungspotenzial liegt in der frühzeitigen Planung von Tests.  
