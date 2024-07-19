# Домашнее задание к занятию "`Уязвимости и атаки на информационные системы`" - `Степанов Владислав`

### Задание 1

1)
PORT     STATE SERVICE 
21/tcp   open  ftp 
22/tcp   open  ssh 
23/tcp   open  telnet 
25/tcp   open  smtp 
53/tcp   open  domain 
80/tcp   open  http 
111/tcp  open  rpcbind 
139/tcp  open  netbios-ssn 
445/tcp  open  microsoft-ds 
512/tcp  open  exec 
513/tcp  open  login 
514/tcp  open  shell 
1099/tcp open  rmiregistry 
1524/tcp open  ingreslock 
2049/tcp open  nfs  
2121/tcp open  ccproxy-ftp 
3306/tcp open  mysql 
5432/tcp open  postgresql 
5900/tcp open  vnc 
6000/tcp open  X11 
6667/tcp open  irc 
8009/tcp open  ajp13 
8180/tcp open  unknown 

2)
[vsftpd 2.3.4 - Backdoor Command Execution](https://www.exploit-db.com/exploits/49757)  
[BIND 9.4.1 < 9.4.2 - Remote DNS Cache Poisoning (Metasploit)](https://www.exploit-db.com/exploits/6122)  
[Samba 3.0.20 < 3.0.25rc3 - 'Username' map script' Command Execution (Metasploit)](https://www.exploit-db.com/exploits/16320)  

### Задание 2  

SYN, FIN, Xmas, UDP
SYN - если хост отвечает флагом SYN/ACK, это означает, что порт открыт, если RST, то порт закрыт.
FIN - отправляет FIN пакеты, если хост отвечает флагом FIN это означает, что порт открыт. Если RST, то закрытый порт.
Xmas - отправляет пакет с установленными флагами URG, PSH, FIN. Если порт закрыт, хост отвечает RST.
UDP - отправляет пустой UDP пакет. Если ответ что порт не доступен, порт закрыт. Другие ICMP ошибки указывают на то, что порт фильтруется. Если не отвечает или UDP, это может указать на открытый порт.


