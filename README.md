# 1.- Introduction
At home, my main device is and old Surface Pro 3 with 125gb. I have an old laptop, a gaming PC, my wife its laptop, some external hhd...information is very scattered. With the aim of centralize and make more accesible all our info, I would like to implement a NAS on my network.

This project would try to evaluate different possibilities and go ahead with the final choose.

# 2.- Define

## 2.1- Goal
- I think that I won't need a big capacity, but you know, the future.... I prefer to have more units of lower capacity. Based on this constrain, the system must be capable to manage 2 hard disk units.
- Minimum electrical conection will be an advance
- Cheaper teh better

## 2.2- Cases
Study cases will be defined in the next lines:

- CASE 1: Comercial NAS. Easier and faster option. No knowledge or welder skill are required. DS220j
- CASE 2: wDiy. Called "w" due to welder skill are needed. 3D printer are needed. Source: https://electrotutoriales.com/servidor-nas-con-raspberry-pi-hardware/
- CASE 3: fDiy. Called "f" due to the creator is French. No welder skill are required, 3D printer are needed. Source: https://youtu.be/suCkt-MaWJs
- CASE 4: Docker station. Just use a doker to feed hdd.
- CASE 5: ownDIY. Case 3 modified toavoid using PSU
- CASE 6: hDiy. Raspi+ Sata hat
- CASE 7: Odroid HC4

# 3.- Analysis
All prizes are form aliexpress or amanzon. If (free) is added just mean that I already has this hardware and for my own analysis the cost doesn't matter.

| Component | CASE 1 | CASE 2 | CASE 3 | CASE 4 | CASE 5 | CASE 6 | CASE 7 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Procesor | Synology: 200e | rpi 3b+: 200e (free) | rpi 3b+: 200e (free) | rpi 3b+: 200e (free) | rpi 3b+: 200e (free) | rpi 3b+: 200e (free) | Odroid hc4: 120e |
| Power supply | included | 12v 5Amp : 11e | PSU <150W: 50e (free) | rpi 3b+: 7e (free) | usb PSU: 40e | usb PSU: 40e | 15V 4Amp: 17e |
| Power conector | included | XL4005: 3e | jack connector: 4e | included | included | included | included |
| Sata link | included | Sata a USB: 4.1e | Sata a USB with jack: 9.36e | included | Sata doble USB:6.16 | Sata hat: 55e | included |
| Sata Conector | included | included | Included | Docker station: 34e | included | included | included |
| Case | included | Printed: 4e | Printed: 4e | not required | Printed: 4e | Printed: 4e | included |
| --- | --- | --- | --- | --- | --- | --- | --- |
| TOTAL | 200e | 222e (22e) | 219e (19e) | 245 (45e) | 250 (50e) | 299e (99e) | 137e |

# 4.- Conclusions
If rpi is available, cases 2 or 3 could be the best option. In my case, I finally choose Odroid. This board has 4gb RAM that will help me with some docker apps like NodeRED or Grocy without problems
