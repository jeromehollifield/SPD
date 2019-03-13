<h1>Setup Guide for Netbeans 10, Java JDK 11, and JavaFX 11</h1>

<p>This project will require that all contributors use the same tools, otherwise there will be compatibility issues.</p>
<p><em>Before updating everything, you may want to uninstall the Older versions of JDK and Netbeans</em></p>
<strong>FOllOW these directions in sequence to get the environment running correctly:</strong>
<ol>
  <li>Download JDK11 bin.exe (or mac version): <a href ="https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html">Here</a></li>
  <li>Download Netbeans 10: <a href="https://www-us.apache.org/dist/incubator/netbeans/incubating-netbeans/incubating-10.0/incubating-netbeans-10.0-bin.zip">Here</a></li>
  <li>Download JavaFX11 SDK: <a href="https://gluonhq.com/products/javafx/">Here</a></li>
</ol>

<h2>Setting up JDK11</h2>
<ol>
  <li><strong>Run the .exe installer to install JDK 11.</strong></li>
  <li><strong>On windows, once the installation finishes you will need to set the system environment variables</strong></li>
  <ul>
    <li>In Windows search, type <em>"variables"</em></li>
    <li>An option to "Edit the system environment Variables" will come up...select it.</li>
    <li>In the windows that pops up select <strong>Advanced Tab > Environment Variables</strong></li>
    <li>In System Variables section, highlight <strong>Path</strong> and click <strong>Edit</strong></li>
    <li>Click <strong>New</strong></li>
    <li>Click <strong>Browse</strong></li>
    <li>Travel to the directory where Java 11 is installed.  Once there open the folder and select the <strong>bin</strong> folder.</li>
    <li>Click <strong>OK</strong> and keep clicking OK on all other windows until everything closes</li>
  </ul>
  <li><strong>Verify Java installation and environment path.</strong>
    <ul>
        <li>Open a command prompt on windows</li>
        <li>In the command prompt type <strong><em>javac -version</em></strong><li>
        <li>You should get an output along the lines of: <em>javac 11.0.2</em></li>
        <li>If your output shows the correct version of java, then you have setup your installation and environment path correctly.</li>
    </ul>
  </li>
    
  
</ol>

<h2>Installing and setting up Netbeans 10</h2>

<ol>
  <li>Extract the .zip netbeans file to the location you want it installed permanently (i extracted it to my <em>Program Files</em> folder).</li>
  <li>In your netbeans file that you extracted, go to the<strong>bin</strong> folder.
  <li>run the netbeans.ext (64 bit) as administrator</li>
  <li>In the IDE, choose <strong>Tools > plugins > Available plugins</strong></li>
  <li>Select the following plugins: 
  <ul>
    <li>MuiltiProperties</li>
    <li>netbeans-deb-export</li>
    <li>netbeans-appimage-export</li>
    <li>nbjavac Library</li>
    <li>Oracle JS Parser Implementation</li>
  </ul>
  </li>
  <li>Click <strong> install</strong> and go through the installation process.</li>
  <li>Restart Netbeans</li>
</ol>


<h2>JavaFX11 for Netbeans 10</h2>
<p>Ensure to follow the steps as there is a bit of a process for JavaFX to work correctly on Netbeans 10</p>
<ol>
  <li>Unzip the JavaFX SDK to desired location (i put mine in the java folder in program files where JDK11 is to easily find it).</li>
  <li>Add Environment path variable: 
      <ul>
        <li>Go to your environment variables windows settings</li>
        <li>Highlight <strong>Path</strong> in the System variables section and click <strong>edit</strong></li>
        <li>Click <strong>New</strong>, then <strong>Browse</strong></li>
        <li>Travel to the directory where you put the JavaFX SDK folder and open it</li>
        <li>It will open that directory, which has three other folders: bin , legal, and lib</li>
        <li>Select the <strong>lib</strong></> folder and click <strong>OK</strong></li>
        <li>Click <strong>OK</strong> again until you have colosed the environment settings window.</li>
      </ul>
  </li>
  <li>Setup JavaFX 11 on Netbeans</li>
  <li>Open Netbeans</li>
  <li><strong>Go to Tools > Libraries > New Library</strong></li>
  <li>Name it <strong>JavaFX11</strong></li>
  <li>Add the .jars in the lib folder from JavaFX11:
      <ul>
        <li>Make sure the <strong>Classpath</strong> tab is selected</li>
        <li>Click the <strong>Add JAR/FOlder...</strong> button</li>
        <li>Open the lib folder in the JavaFX11 folder and select all the .jar files, but make sure you don't add the src.zip file because it will cause an exception</li>
        <li>click the <strong>Add JAR/Folder</strong> button</li>
      </ul>
</ol>


