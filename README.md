# SSD

Minnesanteckningar om SSD minnen, form faktorer, kontakter, hastigheter och tjänster, allt för att skapa en kunskapsbas inför att populera Rasberry Pi's och PC's med solid state drives.

## FORM FAKTOR

* M.2 är namnet på form faktorn
* M.2 är specifikation på internt expansionskort
* 2240/2260/2280 anger dess mått (22mm bred, 40/60/80mm hög)
* M.2 hanterar SATA och PCIe SSD
* M.2 standarden är varianter på 
  * upp till 4 PCIe lanes
  * en SATA 6Gb/s 
  * och/eller en USB 3.0 port
  
<img src="https://www.delock.com/infothek/M.2/images/formfaktoren-vergleich.jpg" width="600px">

*www.delock.com*


## ANSLUTNINGSNYCKLING

* B - SATA
* M - PCIe (x2, x4)
* M/B - PCIe eller SATA

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/M2_Edge_Connector_Keying.svg/350px-M2_Edge_Connector_Keying.svg.png" width="600px">

*https://en.wikipedia.org/wiki/M.2*

## SEKUNDÄRMINNES HASTIGHETER

* SD Class 10 - 10MB/s
* HDD - 5 to 30 MB/s
* SD UHS3 - 30 MB/s
* SD Video90 - 90MB/s
* SATA - 500 MB/s
  * SATA-1 (150MB/s, 1.5Gbps)
  * SATA-3 (300MB/s, 3 Gbps)
  * SATA-3 (600MB/s, 6Gbps)
* NVMe - 3,500 MB/s

## PCIe

* Peripheral Component Interconnect Express

<img src="https://ssl-product-images.www8-hp.com/digmedialib/prodimg/lowres/c04113066.png" width="600px">

*hp.com*

* Seriell kommunikation
* Klarar hot-plug
* Ersätter PCI, PCI-X och AGP bus

* PCI-lanes är flera seriella anslutningar på PCIe
* PCI-lanes kan parallellkopplas för att öka bandbredden
* PCIe är alltså seriell och parallell samtidigt
* Exempel på märkning - PCIe 2.0 / x4 (använder 4 lanes, 4ggr snabbare)
* PC's BIOS hanterar lanes

<img src="https://media.fs.com/images/community/upload/wangEditor/201912/30/_1577696037_99zwUgQjV6.jpg" width="600px">

*fs.com*

<img src="https://media.fs.com/images/community/upload/wangEditor/201912/30/_1577696088_ktAUQfs9PJ.jpg" width="600px">

*fs.com*

## METHOD/PROTOCOL

* PCI-Express NVMe (drivers för läsning av PCI-e slots)
* SATA (drivers för HDD [spinnande teknologi])

## SKILLNADER SATA - NVMe

* SATA är hot-plug, NVMe är inte
* AHCI exponerar SATA interface.

## RPi - REKOMMENDATIONER

* RPi4(b) har 2 x USB3 (5 Gbps bandbredd), 2 x USB2
* RPi4 har inbyggd PCIe bus som går att nå via USB3 via en påbyggd brygga

<img src="https://i1.wp.com/opencloudware.com/wp-content/uploads/2021/05/mirkopc-with-raspberry-pi-compute-module-4.jpg?resize=1024%2C576&ssl=1" width="600px">

*wp.com*

* Om SATA används (rekommenderas av RPi.org) så behövs en USB3-M.2 adapter

## SSD typer

SATA, AHCI, NVMe

2.5" SATA, mSATA, M.2 SATA, AHCI, NVMe will all perform the same in a USB 3.0 enclosur

SATA (6Gbps), NVMe (10Gbps)

Dual protocol uses two kinds of cables, Type-C to Type-A (5Gbps) and Type-C to Type-C (10Gbps)
