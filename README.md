#### Installation setup for Windows
<hr>

* Go to jenkins download site https://jenkins.io/download/ and select the installer for windows.
* Follow up the installation wizard and it gets installed on default port 8080.
* Open any browser and type http://localhost:8080 to verify the installation.
* Get the default admin password for the file initialAdminPassword from installation location (C:\Program Files (x86)\Jenkins\secrets)
* Create the user account in the startup page.

#### Installing github plugin
<hr>

* Click on Manage Jenkins from dashboard and select Manage Plugins to view/add all available plugins.
* Go to available tab and search for GitHub Integration Plugin.
* Click download now and install after restart option. This will install the plugin and restart jenkins server.

#### Setup Java Home, Git and Maven
<hr>

* Go to manage jenkins -> global tool configuration.
* Under JDK section, provide the Java home (ex C:\Java\jdk_1_8) path of your machine.
* Under Git installation section, provide the git (ex C:\Git\bin\git.exe) executable path of your machine.
* Under Maven installation section, provide the maven home (ex C:\maven\apache-maven-3.6.0\) path of your machine.

#### Creating new job (FreeStyle)
<hr>

* Click on the New Item to create jenkins job.
* Select free style project from the next section.
* Select GitHub project and provide the git project url.
* Under SCM section, select Git and provide the git repository url.
* Under SCM section, select Git and provide the git repository url.
* Under Build Trigger section, select GitHub hook trigger for GITScm polling.
* Under Build section, provide the project pom xml file and mention the maven goal (ex clean package).

#### Creating new pipeline job
<hr>

* Click on the New Item to create jenkins job.
* Select pipeline project from the next section.
* We can either create the jenkinsfile in the SCM project or write inline piplescript.
<TBD>


