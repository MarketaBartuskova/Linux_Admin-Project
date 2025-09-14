# Projekt pro Linux administraci – Nastavení částečného LAMP stacku na vlastní VM

 Jedná se o závěrečný projekt, na jejímž základě mi byl udělen certifikát Junior Linux Administrator od ENGETO.
 Cílem bylo vytvořit a nakonfigurovat částečný LAMP stack na vlastním virtuálním stroji.

---

***Zadání:***
1. Vytvoření virtuálního stroje a nastavení privátní sítě.
2. Vytvoření uživatele 'sysadmin', nastavení SSH s RSA klíči a zakázání root loginu.
3. Instalace Apache a PHP.
4. Nasazení webové aplikace na portu 8081 s obsahem ve složce '/srv'.

---

***Použité technologie:***
- VirtualBox + Ubuntu Server 22.04 LTS

---

***Splněné úkoly:***
Úkol 1 – Virtuální stroj
- Vytvořen virtuální stroj ve VirtualBoxu a instalace Ubuntu 
- Síť nastavena na privátní IP (192.168.1.214)

Screenshot: [Běžící VM + ping](screenshots/foto1.png)  
Screenshot: [IP adresa VM + ping na hosta](screenshots/foto2.png)

---

Úkol 2 – SSH + uživatel sysadmin
- Vytvořen uživatel 'sysadmin' 
- Zakázán root login přes SSH
- Přihlášení funguje pouze pomocí RSA klíče  

Screenshot: [Úspěšné SSH přihlášení pomocí klíče](screenshots/foto3.png)  
Screenshot: [Zakázaný root login v sshd_config](screenshots/foto4.png)  
Screenshot: [Neúspěšný pokus o login heslem](screenshots/foto5.png)

---

Úkol 3 + 4 – Apache + PHP + Web
- Apache nakonfigurován na portu 8081 
- DocumentRoot nastaven na '/srv'  
- PHP funkční  
- Webová stránka dostupná na '192.168.1.214:8081'  

Screenshot: [Konfigurace Apache pro /srv a port 8081](screenshots/foto6.png)  
Screenshot: [Běžící webová stránka](screenshots/foto7.png)
