# Konfiguracia Visual Studio Code pre vyucbu programovania

Specialne v obdobi, kedy vyucba prebieha na dialku, musia ziaci na svoja notebooky kvoli vyucbe programovacich jazykov instalovat potrebne aplikacie (Python, Java develpment kit...). Toto moze predstavovat nezelanu komplikaciu, kedze ucitel musi riesit okrem vyucby aj problemy ziakov s instalaciou.

Tento postup je samozrejme mozne pouzit aj na pripravu skolskych notebookov na vyucbu. nebude treba jednotlivo riesit verzie aplikacii na notebookoch.

Tento dokument je vytvoreny pre demonstraciu moznej vyucby Python a inych programovacich jazykov bez toho, aby si napr. Python museli instalovat aj vsetci ziaci na svojich pocitacoch. Jednoduchym sposobom budu mat ziaci pristup prostrediu, ktore je pripravene na pracu priamo ucitelom. Vsetci ziaci budu mat rovnake prostredie, ziadne problemy s tym ze "u mna to nefunguje". navyse budu tymto sposobom uvedeny do modernych nastrojov pouzivanych v IT:
* Github
* Visual Studio Code
* Docker

## 1) instalacia aplikacii
Pre vyucbu vsetkych dostupnych programovacich jazykov (Python, Java, PHP...) je potrebne nainstalovat len dve nasledovne bezplatne aplikacie: 
1) Visual Studio Code https://code.visualstudio.com/download
2) Docker Desktop https://www.docker.com/products/docker-desktop

> Postup vratane screenshotov je rozpisany v originalnom dokumente **Development Containers in Education: A Guide for Instructors**
> * https://code.visualstudio.com/blogs/2020/07/27/containers-edu/?WT.mc_id=devcloud-11496-cxa

## 2) instalacia rozsirenia

Po nainstalovani oboch aplikacii vo VS Code:

* nainstalovat rozsirenie **Remote - Containers**

![nainstalovat rozsirenie](https://code.visualstudio.com/assets/blogs/2020/07/27/3-extension.png)

## 3) pripojit sa 

> start aplikacie Docker Desktop moze trvat pomerne dlho. skor nez sa pristupi k dalsiemu kroku je dolezite ubezpecit sa, ze aplikacia hlasi **Docker Desktop is running**
>
> ![docker](https://docs.docker.com/docker-for-windows/images/whale-icon-systray-hidden.png)

### 3.1) stlacit klaves **F1** -> 

pripojit sa cez rozsirenie **Remote - Containers**

![Remote - Containers extension](https://code.visualstudio.com/assets/blogs/2020/07/27/5-commands-list.png)

### 3.2) **Clone Repository in Container Volume...** 

na https://github.com/d4libor/egjak-info-python.git

![clone](https://code.visualstudio.com/assets/blogs/2020/07/27/6-clone-repo-command.png)

> pre skusku ake rozne prostredia je mozne pripravit takymto sposobom je mozne pouzit **F1** -> 
> * pripojit sa cez rozsirenie **Remote - Containers**
> * pouzit **Try a Sample...** . Takto je mozne nacitat priklady kontajnerov pre prostredia, ktore pripravil priamo tim Microsoft pre programovacie jazyky C++, Go, Java, PHP, .NET Core...
>
> ![sample](https://code.visualstudio.com/assets/docs/remote/containers/select-a-sample.png)

### 3.3) **Create a unique volume.**

Priklad:

> ![volume](https://code.visualstudio.com/assets/blogs/2020/07/27/8-volume-command.png)

### 3.4) nasledne bude lokalne zbuildovany Docker kontajner a ziak moze hned programovat.

Priklad:

> ![build](https://code.visualstudio.com/assets/blogs/2020/07/27/10-starting-container.png)

### 3.5) Spustanie programov je tiez super jednoduche. Pri otvorenom *.PY subore staci jednoducho kliknut vpravo hore na zelenu sipku **Run python file in terminal**

Priklad:

> ![build](https://code.visualstudio.com/assets/docs/python/tutorial/run-python-file-in-terminal-button.png)

Samozrejme je mozne vytvorit pre ziakov podobne prostredia aj pre ine programovacie jazyky a ich verzie.

Video navod pre pracu s kontajnermi a VS Code https://channel9.msdn.com/Series/Beginners-Series-to-Dev-Containers?WT.mc_id=devcloud-11496-cxa

> priklady prevzate z https://github.com/microsoft/c9-python-getting-started
