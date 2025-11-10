# Mini Cloud-Native App mit Docker Compose & Kubernetes

Anleitung: [Praxisprojekt: Von Docker Compose zu Kubernetes — Orchestrierung in Aktion](https://deluxe-utahraptor-24a.notion.site/A-Praxisprojekt-Von-Docker-Compose-zu-Kubernetes-Orchestrierung-in-Aktion-2a7965089da68023839ed5552f4c6f6a?pvs=74)

## Ausgangssituation

Stell dir vor, du arbeitest als **Cloud Engineer** in einem kleinen Start-up namens **MiniCloud**.  
Euer Ziel: Eine einfache, aber skalierbare **Webanwendung**, die später problemlos in der Cloud laufen kann.  

Euer Produkt besteht aus drei Komponenten:
- **Frontend** – eine kleine Website mit HTML & JavaScript  
- **Backend** – eine Python Flask API  
- **Datenbank** – eine MariaDB zur Speicherung von Nutzerdaten  

Zunächst soll alles lokal mit **Docker Compose** laufen.  
Danach migriert ihr die Anwendung in **Kubernetes**, um echte Cloud-Native-Konzepte wie **Pods**, **Deployments**, **Services**, **ConfigMaps** und **Secrets** zu erleben.

---

## Ziel

Am Ende dieses Projekts hast du:
- eine **funktionierende 3-Tier-Anwendung** mit Frontend, Backend & Datenbank,
- sie zuerst mit **Docker Compose** gestartet,
- und anschließend erfolgreich nach **Kubernetes migriert**.

Dabei lernst du zentrale DevOps- und Cloud-Grundlagen praxisnah kennen:
- Container-Orchestrierung  
- Service-Verbindungen in Kubernetes  
- Self-Healing und Skalierung  

---

## Schritte

###  **1. Projektvorbereitung**
- [x] Projektstruktur anlegen (`frontend`, `backend`, `docker-compose.yml`)
- [x] Flask-Backend mit MariaDB-Anbindung implementieren
- [ ] Einfaches HTML-Frontend mit API-Aufruf erstellen
- [ ] Dockerfiles für Backend & Frontend schreiben

---

### **2. Multi-Container-App mit Docker Compose**
- [ ] `docker-compose.yml` erstellen (Frontend, Backend, Datenbank)
- [ ] Anwendung mit `docker compose up -d --build` starten
- [ ] Test: `http://localhost:8080` → „Benutzer laden“ klicken
- [ ] Funktion prüfen und Daten aus der Datenbank abrufen

---

### **3. Kubernetes-Grundlagen verstehen**
- [ ] Wiederholung: Was sind Pods, Deployments, Services?
- [ ] Vergleich zu Docker Compose herstellen
- [ ] Kubernetes Dashboard oder Lens öffnen und Übersicht betrachten

---

### **4. Migration nach Kubernetes**
- [ ] Namespace erstellen (`namespace.yaml`)
- [ ] ConfigMap & Secret für App-Config & Passwörter anlegen
- [ ] Deployments & Services für DB, Backend & Frontend schreiben
- [ ] Backend und Frontend als lokale Images (`backend:v1`, `frontend:v1`) bauen
- [ ] Kubernetes-Manifeste anwenden (`kubectl apply -f ...`)
- [ ] Test: Zugriff über `http://localhost:30080`

---

### **5. Self-Healing beobachten**
- [ ] Mit `kubectl delete pod` einen Pod manuell löschen
- [ ] Beobachten, wie Kubernetes den Pod automatisch ersetzt
- [ ] Vergleich: Verhalten unter Docker Compose vs. Kubernetes

---

### **6. Abschluss & Reflexion**
- [ ] Unterschiede zwischen Docker Compose und Kubernetes diskutieren
- [ ] Vorteile deklarativer Systeme verstehen
- [ ] Ideen für Erweiterungen (Ingress, Monitoring, Autoscaling)

---

## Ergebnis

✅ Du hast eine vollständige, lauffähige **Mini Cloud-Native Anwendung** gebaut  
✅ Du verstehst, wie Container mit Kubernetes orchestriert werden  
✅ Du kannst erklären, warum Kubernetes in der Cloud unverzichtbar ist  

---

> **Bonus-Idee:**  
> Erweitere dein Setup um ein echtes Cloud Deployment (z. B. AWS EKS, Google GKE oder Azure AKS)  
> oder füge ein Ingress mit einer eigenen Domain hinzu.

---

**Tools:** Docker Desktop (mit aktiviertem Kubernetes), Lens, VS Code  
