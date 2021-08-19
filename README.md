# SSD

## FORM FACTOR
* M.2 drive is simply a term to describe the physical form factor of a drive.
* 2240/2260/2280 (22mm wide, 40/60/80mm height)

## KEYING
* B - pin 12-19 (PCIe x2/SATA/USB 2.0/USB 3.0/HSIC/SSIC/Audio/UIM/I2C)
* M - pin 59-66 (PCIe x4/SATA)
* M-key is to the left, B-bey is to the right.
* M/B is SATA
* M is PCIe/NVMe
* M is PCIe/AHCI

## SPEED
* SD Class 10 - 10MB/s
* SD UHS3 - 30 MB/s
* SD Video90 - 90MB/s
* HDD - 5 to 30 MB/s
* SATA - 500 MB/s
* NVMe - 3,500 MB/s

## PCIe
* Peripheral Component Interconnect Express
* Serial com
* Accepts hot-plug
* Supersedes PCI, PCI-X and AGP bus

## METHOD/PROTOCOL
* PCI-Express (NVMe)
* SATA
  * SATA-1 (150MB/s, 1.5Gbps)
  * SATA-3 (300MB/s, 3 Gbps)
  * SATA-3 (100MB/s, 6Gbps)

## DIFFERENCES
* SATA is hot-plug, NVMe is not
* AHCI exposes SATA interface.

## SSD type
SATA, AHCI, NVMe


2.5" SATA, mSATA, M.2 SATA, AHCI, NVMe will all perform the same in a USB 3.0 enclosur

SATA (6Gbps), NVMe (10Gbps)

Dual protocol uses two kinds of cables, Type-C to Type-A (5Gbps) and Type-C to Type-C (10Gbps)

There are two different methods a PC uses to read an SSD: SATA 3 and NVMe.
* SATA uses AHCI drivers that are designed for hard disk drives (HDD) with spinning technology 
* NVMe driver is specifically designed for SSDs data read straight from a PCI-E slot
