Ukázkový projekt pro Linux administraci – konfigurace částečného LAMP stacku

Jedná se o závěrečný projekt, na jejímž základě mi byl udělen certifikát Junior Linux Administrator od ENGETO.
Cílem bylo vytvořit a nakonfigurovat částečný LAMP stack na vlastním virtuálním stroji.

Zadání:
- Vytvoření vlastní VM a nastavení sítě
- Vytvoření uživatele 'sysadmin' s přístupem pouze přes 'SSH klíč' a se sudo právy
- Instalace Apache a PHP
- Nasazení ukázkové PHP stránky na portu 8081

Použité technologie:
- VirtualBox + Ubuntu Server 22.04 LTS

Splněné úkoly:
1. ✅ Virtuální stroj s privátní IP, přístupný z hosta  
2. ✅ SSH konfigurace s RSA key-root login zakázán  
3. ✅ Instalace Apache + PHP  
4. ✅ Zobrazení webová stránky

screenshoty: 
Najdete ve složce [`screenshots/`](./screenshots):
- VM běžící ve virtualBoxu + ping
- SSH přihlášení s klíčem (a selhání s heslem)
- Konfigurace `sshd_config` a `httpd.conf`
- Funkční stránka v prohlížeči
