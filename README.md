stereogl
========

Steroskopische OpenGL Animation - Hausarbeit GD
-----------------------------------------------
- Modell: OpenGL Teatpot http://de.wikipedia.org/wiki/Utah-Teekanne


Wiki-Links: 
-----------
- [Berechnung Abstand etc.] http://de.wikipedia.org/wiki/Stereoskopisches_Sehen#Der_Kreuzblick
- [Bildbeispiele] http://de.wikipedia.org/wiki/Stereoskopie

Dokumentation
-------------
- Berechnung
- Idee
- Umsetzung

Präsentation
------------
- Aufbau Dokumentation folgen

Beispielprogramm
----------------
- Umsetzung mittels SDL, C++/C und OpenGL

Nötige Bibliotheken für Ubuntu
------------------------------
- SFML --> http://www.sfml-dev.org/tutorials/1.6/window-opengl.php
- [SFML] sudo apt-get install libcsfml-dev libsfml-dev glutg3-dev
<br><br>
Wahrscheinlich nicht nötig, bei Problem sollte damit aber mal experimentiert werden:
- [Setting up OpenGL-Dev in Ubuntu]http://www.codeproject.com/Articles/182109/Setting-up-an-OpenGL-development-environment-in-Ub
- [alternativ] sudo apt-get install freeglut3-dev
- [alternativ] sudo apt-get install build-essential libsdl1.2debian libsdl1.2-dev libgl1-mesa-dev libglu1-mesa-dev libsdl-image1.2 libsdl-image1.2-dev

Entwicklungsumgebung
--------------------
- Eclipse Indigo mit CDT C/C++ Plugin: http://www.eclipse.org/downloads/packages/eclipse-ide-cc-developers-includes-incubating-components/indigosr2
- [Git in Eclipse EGit] http://www.vogella.com/articles/EGit/article.html
<br><br>
Dem Linker müssen in der Regel folgende Libs bekannt gemacht werden:
    <li> sfml-system
    <li> sfml-window
    <li> sfml-graphics
<br><br>
- [OpenGL in Eclipse] http://lifeofaprogrammergeek.blogspot.de/2008/06/opengl-glut-and-glew-in-eclipse.html

<br><br>
- Netbeans 7.1.1 mit C/C++ Plugin / Git-Unterstützung integriert http://netbeans.org/kb/docs/ide/git.html
    <li> Team -> Git -> Clone
    <li> Repo-Url[SSH]: github.com:fraterv/stereogl.git
    <li> [Start a new C++ Project in Netbeans]http://zetcode.com/articles/netbeanscdevelopment/
    <li> rechte Maustaste auf das Projekt -> Properties -> Linker -> Librarys -> Add Option -> OtherOption [-lglut / -lGL / -lGLU]