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
Erstellung einer Portfolio-Seite mit einem klar strukturierten Backend, das REST-APIs für CRUD-Funktionen bereitstellt. Das Frontend ist responsiv und interaktiv, und die Kommunikation zwischen den Komponenten wird mit dem Mediator-Pattern optimiert.

#### **1.2 User Stories**  
| US-№ | Verbindlichkeit | Typ       | Beschreibung                                                  |
|------|-----------------|-----------|--------------------------------------------------------------|
| 1    | Muss           | Funktion  | Backend stellt REST-APIs zur Verfügung, die CRUD-Operationen ermöglichen. |
| 2    | Muss           | Funktion  | Frontend ist vollständig responsiv und nutzerfreundlich.    |
| 3    | Muss           | Funktion  | Modal für die Anzeige von Projektdetails funktioniert korrekt. |
| 4    | Muss           | Qualität  | Mediator-Pattern wird im Frontend eingesetzt, um die Kommunikation zu optimieren. |

#### **1.3 Testfälle**  
| TC-№ | Ausgangslage       | Eingabe                        | Erwartete Ausgabe                                              |
|------|--------------------|--------------------------------|----------------------------------------------------------------|
| 1.1  | Backend nicht implementiert | GET /api/projects       | Fehlerantwort: "Backend nicht verfügbar"                      |
| 2.1  | Seite geladen      | Keine Eingabe                  | Die Seite wird korrekt angezeigt und ist responsiv.           |
| 3.1  | Projektliste vorhanden | Klick auf "Details anzeigen"  | Modal mit Projekt-Details wird geöffnet.                       |
| 4.1  | Modal geöffnet     | Klick auf "Schliessen"           | Modal wird geschlossen.                                        |

---

### **2. Planen**  

| AP-№ | Frist         | Zuständig       | Beschreibung                   | geplante Zeit |
|------|---------------|-----------------|---------------------------------|---------------|
| 1.A  | 17.11.2025    | Dorian Herzig   | Entwicklung des Frontends      | 180 min       |
| 2.A  | 24.11.2025    | Dorian Herzig   | Implementierung des Modals     | 150 min       |
| 3.A  | 01.12.2025    | Dorian Herzig   | Backend-Entwicklung (REST-APIs für CRUD-Funktionen) | 180 min (geplant) |
| 4.A  | 01.12.2025    | Dorian Herzig   | Implementierung des Mediator-Patterns im Frontend | 120 min       |

---

### **3. Entscheiden**  
- **Technologiewahl Backend:** Verwendung von Node.js, Express und MongoDB für das Backend, um ein robustes und skalierbares System mit klar strukturierten REST-APIs zu entwickeln. Die APIs sollen CRUD-Operationen unterstützen.  
- **Frontend-Technologien:** HTML, CSS und JavaScript für die Gestaltung eines responsiven und interaktiven Frontends.  
- **Mediator-Pattern:** Das Mediator-Pattern wird im Frontend verwendet, um die Kommunikation zwischen den Komponenten zu optimieren und so eine saubere Trennung der Logik zu erreichen.

---

### **4. Realisieren**  

| AP-№ | Datum        | Beschreibung                   | geplante Zeit | tatsächliche Zeit |
|------|--------------|---------------------------------|---------------|-------------------|
| 1.A  | 17.11.2025   | Entwicklung des Frontends       | 180 min       | 200 min           |
| 2.A  | 24.11.2025   | Implementierung des Modals      | 150 min       | 180 min           |
| 3.A  | 01.12.2025   | Backend-Entwicklung (geplant)   | 180 min       | -                 |
| 4.A  | 01.12.2025   | Implementierung des Mediator-Patterns im Frontend | 120 min   | 135 min           |

---

### **5. Kontrollieren**  

#### **5.1 Testprotokoll**  
| TC-№ | Datum       | Resultat                                          | Tester         |
|------|-------------|--------------------------------------------------|----------------|
| 1.1  | 18.12.2025  | Backend nicht implementiert, daher Fehlerantwort | Dorian Herzig  |
| 2.1  | 18.12.2025  | Modal zeigt die Projektdetails korrekt an         | Dorian Herzig  |
| 3.1  | 18.12.2025  | Kommunikation zwischen den Frontend-Komponenten funktioniert durch das Mediator-Pattern | Dorian Herzig  |

#### **5.2 Exploratives Testen**  
| BR-№ | Ausgangslage | Eingabe       | Erwartete Ausgabe                   | Tatsächliche Ausgabe |
|------|--------------|---------------|-------------------------------------|-----------------------|
| I    | Leere Datenbank | Klick auf "Details anzeigen" | Modal öffnet sich mit den Projektdetails | Modal öffnet sich korrekt |

---

### **6. Auswerten**  
Das Frontend wurde erfolgreich entwickelt und ist vollständig responsiv. Alle interaktiven Funktionen, wie das Modal zur Anzeige von Projektdetails, funktionieren wie erwartet. Das Mediator-Pattern wurde im Frontend erfolgreich implementiert und hat die Kommunikation zwischen den Komponenten optimiert.

Das Backend, das die REST-APIs für die CRUD-Operationen bereitstellen sollte, wurde zwar geplant, aber nicht umgesetzt. In einer zukünftigen Version könnte das Backend hinzugefügt werden, um die Portfolio-Seite mit dynamischen Inhalten aus einer Datenbank zu verbinden.

Ein weiteres Verbesserungspotenzial besteht in der Implementierung des geplanten Backends, um die gesamte Architektur des Projekts zu vervollständigen und die Interaktivität weiter zu steigern.
