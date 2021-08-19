# SSD

## FORM FAKTOR

* M.2 är form faktor
* 2240/2260/2280 (22mm bred, 40/60/80mm hög)

## KEYING

* B - pin 12-19 (PCIe x2/SATA/USB 2.0/USB 3.0/HSIC/SSIC/Audio/UIM/I2C)
* M - pin 59-66 (PCIe x4/SATA)
* M-key is to the left, B-bey is to the right.
* M/B is SATA
* M is PCIe/NVMe
* M is PCIe/AHCI

## SPEED

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
* Seriell kommunikation
* Klarar hot-plug
* Ersätter PCI, PCI-X och AGP bus

* PCI-lane

## METHOD/PROTOCOL

* PCI-Express NVMe (drivers för läsning av PCI-e slots)
* SATA (drivers för HDD [spinnande teknologi])

## SKILLNADER

* SATA är hot-plug, NVMe är inte
* AHCI exponerar SATA interface.

## RPi - REKOMMENDATIONER

* RPi4(b) har 2 x USB3 (5 Gbps bandbredd), 2 x USB2
* RPi4 har inbyggd PCIe bus som går att nå via USB3 via en påbyggd brygga
* Om SATA används 

## SSD typer

SATA, AHCI, NVMe

2.5" SATA, mSATA, M.2 SATA, AHCI, NVMe will all perform the same in a USB 3.0 enclosur

SATA (6Gbps), NVMe (10Gbps)

Dual protocol uses two kinds of cables, Type-C to Type-A (5Gbps) and Type-C to Type-C (10Gbps)
