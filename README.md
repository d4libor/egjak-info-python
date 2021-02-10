# Konfiguracia Visual Studio Code pre vyucbu programovania

Vytvorene pre demonstraciu moznej vyucby Python a inych programovacich jazykov bez toho, aby si napr. Python museli instalovat aj vsetci ziaci na svojich pocitacoch. jednoduchym sposobom budu mat ziaci pristup prostrediu, ktore je pripravene na pracu priamo ucitelom. vsetci ziaci budu mat rovnake prostredie, ziadne problemy s tym ze "u mna to nefunguje". navyse budu tymto sposobom uvedeny do modernych nastrojov pouzivanych v IT:
* Github
* Visual Studio Code
* Docker a nasledne suvisiace produkty ako Kubernetes, OpenShift atd.

## instalacia aplikacii
Nainstalovat treba nasledovne bezplatne aplikacie: 
1) Visual Studio Code https://code.visualstudio.com/download
2) Docker Desktop https://www.docker.com/products/docker-desktop

> Postup vratane screenshotov je rozpisany v originalnom dokumente **Development Containers in Education: A Guide for Instructors**
> * https://code.visualstudio.com/blogs/2020/07/27/containers-edu/?WT.mc_id=devcloud-11496-cxa

### instalacia rozsirenia

Po nainstalovani oboch aplikacii vo VS Code:

* nainstalovat rozsirenie **Remote - Containers extension**

![nainstalovat rozsirenie](https://code.visualstudio.com/assets/blogs/2020/07/27/3-extension.png)

### pripojit sa 

* stlacit klaves **F1** -> pripojit sa cez rozsirenie **Remote - Containers extension**

![Remote - Containers extension](https://code.visualstudio.com/assets/blogs/2020/07/27/5-commands-list.png)

* **Clone Repository in Container Volume...** na https://github.com/d4libor/egjak-info-python.git

![clone](https://code.visualstudio.com/assets/blogs/2020/07/27/6-clone-repo-command.png)

> pre skusku ake rozne prostredia je mozne pripravit takymto sposobom je mozne pouzit **F1** -> 
> * pripojit sa cez rozsirenie **Remote - Containers extension**
> * pouzit **Try a Sample...** . Takto je mozne nacitat priklady kontajnerov pre prostredia, ktore pripravil priamo tim Microsoft pre programovacie jazyky C++, Go, Java, PHP, .NET Core...

* **Create a unique volume.**

![volume](https://code.visualstudio.com/assets/blogs/2020/07/27/8-volume-command.png)

* nasledne bude lokalne zbuildovany Docker kontajner a ziak moze hned programovat. Spustanie programov je tiez super jednoduche. Pri otvorenom *.PY subore staci jednoducho kliknut vpravo hore na zelenu sipku **Run python file in terminal**

![build](https://code.visualstudio.com/assets/blogs/2020/07/27/10-starting-container.png)

Samozrejme je mozne vytvorit podobne prostredia aj pre ine programovacie jazyky a ich verzie (Python2, Python3...)
