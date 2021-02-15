# Konfiguracia Visual Studio Code pre vyucbu programovania

Specialne v obdobi, kedy vyucba prebieha na dialku, musia ziaci na svoja notebooky kvoli vyucbe programovacich jazykov instalovat potrebne aplikacie (Python, Java develpment kit...). Toto moze predstavovat nezelanu komplikaciu, kedze ucitel musi riesit okrem vyucby aj problemy ziakov s instalaciou.

Nasledovny postup je samozrejme mozne pouzit aj na pripravu skolskych notebookov na vyucbu. nebude treba jednotlivo riesit verzie aplikacii na jednotlivych notebookoch.

Tento dokument je vytvoreny pre demonstraciu moznej vyucby Python a inych programovacich jazykov (pripadne aj napriklad zaklady prace s Linuxom) bez toho, aby si napr. Python museli instalovat aj vsetci ziaci na svojich pocitacoch. Jednoduchym sposobom budu mat ziaci pristup prostrediu, ktore je pripravene na pracu priamo ucitelom. Vsetci ziaci budu mat rovnake prostredie, ziadne problemy s tym ze "u mna to nefunguje". navyse budu tymto sposobom uvedeny do modernych nastrojov pouzivanych v IT:
* Github
* Visual Studio Code
* Docker

## Obsah

1. [instalacia aplikacii](#1-instalacia-aplikacii)
2. [instalacia rozsirenia](#2-instalacia-rozsirenia)
3. [pripojenie na Github](#3-pripojenie-na-github)
    - [3.1 stlacit klaves F1](#31-stlacit-klaves-f1)
    - [3.2 Clone Repository in Container Volume](#32-clone-repository-in-container-volume)
    - [3.3 Create a unique volume](#33-create-a-unique-volume)
    - [3.4 automaticke zbuildovanie Docker kontajnera](#34-automaticka-priprava-docker-kontajnera)
4. [spustanie programov](#4-spustanie-programov)

## 1. instalacia aplikacii
Pre vyucbu vsetkych dostupnych programovacich jazykov (Python, Java, PHP...) je potrebne nainstalovat [^1] len dve nasledovne bezplatne aplikacie:
1) Visual Studio Code https://code.visualstudio.com/download
2) Docker Desktop https://www.docker.com/products/docker-desktop

[späť na obsah](#obsah)

## 2. instalacia rozsirenia

Po nainstalovani oboch aplikacii vo VS Code:

* nainstalovat rozsirenie **Remote - Containers**

![nainstalovat rozsirenie](https://code.visualstudio.com/assets/blogs/2020/07/27/3-extension.png)

[späť na obsah](#obsah)

## 3. pripojenie na Github

> start aplikacie Docker Desktop moze trvat pomerne dlho. skor nez sa pristupi k dalsiemu kroku je dolezite ubezpecit sa, ze aplikacia hlasi **Docker Desktop is running**
>
> ![docker](https://docs.docker.com/docker-for-windows/images/whale-icon-systray-hidden.png)

[späť na obsah](#obsah)

### 3.1 stlacit klaves F1

pripojit sa cez rozsirenie **Remote - Containers**

![Remote - Containers extension](https://code.visualstudio.com/assets/blogs/2020/07/27/5-commands-list.png)

[späť na obsah](#obsah)

### 3.2 Clone Repository in Container Volume

na https://github.com/d4libor/egjak-info-python.git

![clone](https://code.visualstudio.com/assets/blogs/2020/07/27/6-clone-repo-command.png)

> pre skusku ake rozne prostredia je mozne pripravit takymto sposobom je mozne pouzit **F1** -> 
> * pripojit sa cez rozsirenie **Remote - Containers**
> * pouzit **Try a Sample...** . Takto je mozne nacitat priklady kontajnerov pre prostredia, ktore pripravil priamo tim Microsoft pre programovacie jazyky C++, Go, Java, PHP, .NET Core...
>
> ![sample](https://code.visualstudio.com/assets/docs/remote/containers/select-a-sample.png)

[späť na obsah](#obsah)

### 3.3 Create a unique volume

Priklad:

> ![volume](https://code.visualstudio.com/assets/blogs/2020/07/27/8-volume-command.png)

[späť na obsah](#obsah)

### 3.4 automaticka priprava Docker kontajnera

nasledne bude automaticky lokalne zbuildovany Docker kontajner

Priklad:

> ![build](https://code.visualstudio.com/assets/blogs/2020/07/27/10-starting-container.png)

[späť na obsah](#obsah)

## 4. Spustanie programov

Po uspesnej lokalnej priprave Docker kontajnera moze ziak hned programovat.

> ![start](https://code.visualstudio.com/assets/blogs/2020/07/27/11-sortpy-cropped.png)

Spustanie programov je tiez super jednoduche. Pri otvorenom *.PY subore staci jednoducho kliknut vpravo hore na zelenu sipku **Run python file in terminal**

Priklad:

> ![build](https://code.visualstudio.com/assets/docs/python/tutorial/run-python-file-in-terminal-button.png)

Samozrejme je mozne podobnym sposobom vytvorit pre ziakov prostredia aj pre ine programovacie jazyky a ich verzie.

[späť na obsah](#obsah)

****

## Povodny dokument v anglictine
Postup vratane screenshotov je rozpisany v originalnom dokumente **Development Containers in Education: A Guide for Instructors**
    * https://code.visualstudio.com/blogs/2020/07/27/containers-edu/?WT.mc_id=devcloud-11496-cxa

## Video navod

Video navod pre pracu s kontajnermi a VS Code https://channel9.msdn.com/Series/Beginners-Series-to-Dev-Containers?WT.mc_id=devcloud-11496-cxa

## Python priklady

priklady Python suborov su prevzate z https://github.com/microsoft/c9-python-getting-started

[späť na obsah](#obsah)
