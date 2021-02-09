# egjak-info-python
repo pre egjak, vyucba informatiky, python

vytvorene pre demonstraciu moznej vyucby Python a inych programovacich jazykov bez toho, aby si python museli instalovat aj vsetci ziaci na svojich pocitacoch. jednoduchym sposobom budu mat ziaci pristup prostrediu, ktore je pripravene na pracu priamo ucitelom. vsetci ziaci budu mat rovnake prostredie, ziadne problemy s tym ze "u mna to nefunguje". navyse budu tymto sposobom uvedeny do modernych nastrojov pouzivanych v IT:
* Github
* Visual Studio Code
* Docker a nasledne suvisiace produkty ako Kubernetes, OpenShift atd.

Postup je rozpisany vratane screenshotov v originalnom dokumente 

**Development Containers in Education: A Guide for Instructors**

https://code.visualstudio.com/blogs/2020/07/27/containers-edu/?WT.mc_id=devcloud-11496-cxa

Nainstalovat treba nasledovne bezplatne aplikacie: 
1) Visual Studio Code https://code.visualstudio.com/download
2) Docker Desktop https://www.docker.com/products/docker-desktop

* nainstalovat do VS Code rozsirenie **Remote - Containers extension**
* vo VS Code sa pripojit cez rozsirenie **Remote - Containers extension** -> 

* **Clone Repository in Container Volume...** na https://github.com/d4libor/egjak-info-python.git , 

* **Create a unique volume.**

* nasledne bude lokalne zbuildovany Docker kontajner a ziak moze hned programovat. Spustanie programov je tiez super jednoduche. Pri otvorenom *.PY subore staci jednoducho kliknut vpravo hore na zelenu sipku **Run python file in terminal**

Samozrejme je mozne vytvorit podobne prostredia aj pre ine programovacie jazyky a ich verzie (Python2, Python3...)
