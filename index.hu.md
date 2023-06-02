---
cím: KOOMPI OS leírás
leírás: A KOOMPI OS használata az eszközeivel és beállításaival.
---

# KOOMPI OS

Kóstolja meg a Vanilla GNOME élményt Ubuntu-n enyhén fűszerezve. 

## GYIK

Válaszok a leggyakrabban ismételt kérdésekre (pedig a projekt elég fiatal).
- **Miért egy új disztribúció?**\
  A KOOMPI OS egy olyan Ubuntu alapú Linux disztribúció hiányában jött létre, 
  amely vanilla GNOME-ot kínál, a felhasználói élmény módosítása nélkül. 
  Később, az elképzelés ki lett terjesztve pár eszközzel és technológiával, mint 
  az Almost (igény szerinti felülírhatatlanság) és az pix (a Distrobox alapú 
  alrendszer).
- **OSTree-t használ?**\
  Nem. A KOOMPI OS az [`almost`](https://github.com/koompi-os/almost) által ér 
  el felülírhatatlanságot. Ezt a kelléket a fájlok felülírhatatlan tulajdonságán 
  alapuló, igény szerinti felülírhatatlansághoz írtuk. Ez a megközelítés bármely 
  partíciós sémán, vagy fájlrendszeren működik. Az OSTree még szóba jöhet a jövőben. 
- **Gördülő Kiadás?**\
  Nem. A KOOMPI OS egy pont-kiadású rendszer és az Ubuntu kiadási ciklust követi.

## Szekciók

- **[Felülírhatatlanság (`almost`)](/docs/almost)**\
Az Almost egy kellék a fájlok felülírhatatlan tulajdonságán alapuló, igény 
szerinti felülírhatatlansághoz.

- **[Csomagkezelő (`pix`)](/docs/pix)**\
Az pix egy olyan csomagkezelő, amely egy kezelt konténerbe enged csomagokat 
telepíteni, anélkül, hogy a hosztrendszert befolyásolná. Alkalmanként, az `pix` 
használatával lehetséges a hosztrendszerre is telepíteni csomagokat.
