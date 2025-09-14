Projekt pro Linux administraci – konfigurace částečného LAMP stacku

Jedná se o závěrečný projekt, na jejímž základě mi byl udělen certifikát Junior Linux Administrator od ENGETO.
Cílem bylo vytvořit a nakonfigurovat částečný LAMP stack na vlastním virtuálním stroji.

Zadání:
1. Vytvoření virtuálního stroje a nastavení privátní sítě.
2. Vytvoření uživatele 'sysadmin', nastavení SSH s RSA klíči a zakázání root loginu.
3. Instalace Apache a PHP.
4. Nasazení webové aplikace na portu 8081 s obsahem ve složce '/srv'.

Použité technologie:
- VirtualBox + Ubuntu Server 22.04 LTS

Splněné úkoly:
Úkol 1 – Virtuální stroj
- Vytvořen virtuální stroj ve VirtualBoxu a instalace Ubuntu 
- Síť nastavena na privátní IP (192.168.1.214)  

Screenshot: [Screenshot VM + ping](screenshots/task1_vm_ping.png)

---

Úkol 2 – SSH + uživatel sysadmin
- Vytvořen uživatel 'sysadmin' 
- Zakázán root login přes SSH
- Přihlášení funguje pouze pomocí RSA klíče  

Screenshot: [Úspěšné SSH přihlášení + sudo](screenshots/task2_ssh_key.png)  
Screenshot: [Zakázaný root login v sshd_config](screenshots/task2_root_disabled.png)

---

Úkol 3 + 4 – Apache + PHP + Web
- Apache nakonfigurován na portu 8081 
- DocumentRoot nastaven na '/srv'  
- PHP funkční  
- Webová stránka dostupná na 'http://192.168.1.214:8081'  

Screenshot: [Apache config /srv](screenshots/task3_apache_conf.png)  
Screenshot: [Běžící webová stránka](screenshots/task4_webpage.png)
