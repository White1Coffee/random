# Random
# Algemene Opslag & Server Bestanden

Welkom bij deze persoonlijke repository! Dit is een centrale, flexibele opslagplek voor uiteenlopende bestanden, scripts en plug-ins. Het hoofddoel van deze repo is om snel en eenvoudig bestanden te kunnen synchroniseren en downloaden naar externe (Linux) servers via Git of `wget`/`curl`.

## 📁 Repository Structuur

Omdat deze repository voor diverse doeleinden wordt gebruikt, is de inhoud als volgt georganiseerd:

*   **`/image/`:** Bevat afbeeldingen en media-bestanden.
*   **Root directory (`/`):** Bevat op dit moment verschillende Minecraft server-plug-ins (`.jar`-bestanden), waaronder:
    *   `EssentialsX` & `EssentialsXDiscord` (Serverbeheer en Discord-koppeling)
    *   `LuckPerms-Bukkit` (Permissiesbeheer)
    *   `Simple Voice Chat` & `OpenAudioMc` (Audio & spraak-integratie)
    *   `SimpleTrading` & `headdrop` (Gameplay-mechanics)
*   *(Toekomstig)*: Scripts (`.sh`, `.py`), configuratiebestanden (`.yml`, `.conf`) en andere server-assets.

---

## 🚀 Bestanden Downloaden op een Linux Server

Aangezien deze repository publiek is (`Public`), kun je de bestanden direct op je Linux-omgeving binnenhalen via de terminal. Hier zijn de handigste methoden:

### 1. De gehele repository clonen
Als je alle bestanden in één keer op je server wilt hebben:
```bash
# Clone de repository naar je server
git clone https://github.com/White1Coffee/random.git

# Navigeer naar de map
cd random
```

### 2. Specifieke bestanden downloaden via `wget` of `curl`
Als je slechts één specifiek bestand nodig hebt (bijvoorbeeld een plug-in of script), kun je de **Raw** URL van GitHub gebruiken.

**Voorbeeld met `wget`:**
```bash
wget https://raw.githubusercontent.com/White1Coffee/random/main/LuckPerms-Bukkit-5.5.84.jar
```

**Voorbeeld met `curl`:**
```bash
curl -O https://raw.githubusercontent.com/White1Coffee/random/main/LuckPerms-Bukkit-5.5.84.jar
```

---

## 🛠️ Aanbevolen Workflow voor Updates

Wanneer je vanaf je lokale computer nieuwe bestanden toevoegt die je later op je Linux server nodig hebt:

1. **Lokaal toevoegen en pushen:**
   ```bash
   git add .
   git commit -m "Toevoegen van nieuwe serverbestanden"
   git push origin main
   ```
2. **Updaten op de Linux server:**
   Als je de repo al gecloned hebt op je server, haal je de nieuwste bestanden simpelweg binnen met:
   ```bash
   git pull origin main
   ```

---

## 🔒 Veiligheidswaarschuwing
Aangezien deze repository **openbaar (Public)** is, moet je ervoor zorgen dat je **nooit** gevoelige informatie uploadt, zoals:
*   Wachtwoorden of database-credentials
*   API-keys of Discord bot tokens
*   Private SSH-sleutels
*   `.env` of `config.yml` bestanden waarin geheimen staan
