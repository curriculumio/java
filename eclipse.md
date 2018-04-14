# Java setup

Many Java programmers use an **Integrated Development Environment** (IDE) to edit and run Java programs. I recommend using **Eclipse**, a free IDE that can be downloaded from [eclipse.org](http://eclipse.org).

## Install Java 8

Eclipse requires **Java 8**, which you can [download from Oracle](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html). You must first accept their [license agreement](https://tldrlegal.com/license/oracle-binary-code-license-agreement-for-the-java-se-platform-products-and-javafx), after which you can download the installer for your **operating system**.

![](java/eclipse/oracle.png)

### Mac OSX

The downloaded file will open a disk image, and you will have to double click the `.pkg` file inside the disk image to run the installer. You will need an account with administrator privileges to install Java 8.

![](java/eclipse/oracle-mac.png)

### Windows

On some Windows computers, the JDK 8 installer will not properly configure your computer to work with Java. This can usually be fixed by [setting your PATH variable](  http://docs.oracle.com/javase/8/docs/technotes/guides/install/windows_jdk_install.html#BABGDJFH).

Another possible issue that arises on Windows is when there are multiple versions of Java installed. Try uninstalling all versions of Java from the Control Panel, then re-install Java 8.

## Install Eclipse

The Eclipse installer can be downloaded from [eclipse.org/downloads](http://eclipse.org/downloads). Select your operating system to download its Eclipse installer.

![](java/eclipse/eclipse-download-site.png)

Click the orange download button to start downloading Eclipse.

![](java/eclipse/eclipse-download-button.png)

Open the downloaded Eclipse Installer and click "Eclipse IDE for Java Developers".

![](java/eclipse/eclipse-installer.png)

You can install Eclipse in the default `eclipse` folder, or select a different folder.

<div class="tip">
<p>On Mac OSX, you may want to change the installation folder to `/Applications/eclipse` if you don't plan on installing multiple versions of Eclipse.</p>
</div>

![](java/eclipse/eclipse-installer-location.png)

Accept the [Eclipse license agreement](https://www.tldrlegal.com/l/epl) (or click "Decide Later") to begin the installation.

![](java/eclipse/eclipse-installer-agreement.png)

Once Eclipse has completed installation, you can click the green Launch button to open it.

![](java/eclipse/eclipse-installer-launch.png)

## How to use Eclipse

Eclipse can be used with many programming languages, and has an immense set of features and tools under the hood. In our course, we will only need to do three basic things with Eclipse - create folders, create files in those folders, and import code from external files.

When you open Eclipse for the first time, you will need to click the "Workbench" link.

![](java/eclipse/eclipse-welcome.png)

The Workbench is just a fancy text editor that starts off with a lot of additional panels that we won't need. Click the x's to close every panel *except for the Package Explorer*.

<div class="tip">
<p>You can re-open any panel by going to `Window` > `Show View` and clicking on the name of the panel.</p>
</div>

![](java/eclipse/eclipse-close-panels.png)

### Create a project

A Java Project is just a folder on your computer that is managed by Eclipse. You can create Java Projects by right clicking on the Package Explorer, hovering over "New", and selecting "Java Project".

<div class="tip">
<p>If you hid the package explorer, navigate in the top menu to `Window` > `Show View` > `Package Explorer` to re-open it.</p>
</div>

![](java/eclipse/eclipse-new.png)

In the dialog box that pops up, enter a name for the project, then click "Finish".

![](java/eclipse/eclipse-new-project.png)

### Create a file

To create a file, right click on the `src` folder, hover over "New", and select "Class".

![](java/eclipse/eclipse-new-file.png)

### Create a package

A package is a sub-folder within the Java Project that provides an additional level of organization for your files.

### Install a library

Our curriculum uses [APCS](http://apcs.io) graphics, a free and open-source **library** developed at techlab for building games and animations. We distribute the code through a **Java archive** file, which uses the `.jar` extension. In general, you will find that Java developers distribute code through `.jar` files, so this process applies to *any library* that you wish to use in the future, not just ours.

Once you have [downloaded the APCS library](http://apcs.io/download/apcs.jar), you will need to drag the `apcs.jar` file from its location on your computer to a Java Project in Eclipse. Ensure that "copy files" is selected, then click OK.

<div class="tip">
<p>Be sure to drop the file on the project's name (not on the `src` folder).</p>
<p>Reduce the size of the Eclipse window so you can easily drag the file from its location on your computer to your Java Project.</p>
<p>Copying the library allows you to delete it from its original location on your computer.</p>
</div>

![](java/eclipse/library-copy.gif)

To tell Eclipse to use the APCS library, you will need to add it to the **build path**. Right click on `apcs.jar`, hover over "Build Path", then click "Add to Build Path".

![](java/eclipse/library-build-path.gif)

<div class="tip">
<p>Do not move or delete the `apcs.jar` file inside the Java Project.</p>
<p>If you create another Java Project, you will have to repeat these two steps to use the APCS library in it.</p>
</div>
