HelloAndroidDependencies
========================

Testing best practices for dependency magament in Android Projects (using eclipse, android annotations, actionbar sherlock)

1) Add most dependecies with gradle
/home/ntesser/tools/gradle-1.7/bin/gradle build

2) Clean up with gradle (ant is our build system, gradle just add some dependencies)
/home/ntesser/tools/gradle-1.7/bin/gradle clean

3) Add Annotation Processing for android annotations
https://github.com/excilys/androidannotations/wiki/Eclipse-Project-Configuration
https://github.com/excilys/androidannotations/wiki/Building-Project-Maven-Eclipse

(I have to add 3 dependencies in the factory, so that the .factorypath looks like this:

<factorypath>
    <factorypathentry kind="PLUGIN" id="org.eclipse.jst.ws.annotations.core" enabled="true" runInBatchMode="false"/>
    <factorypathentry kind="WKSPJAR" id="/HelloAndroidDependencies/libs/androidannotations-api-2.7.1.jar" enabled="true" runInBatchMode="false"/>
    <factorypathentry kind="WKSPJAR" id="/HelloAndroidDependencies/compile-libs/androidannotations-2.7.1.jar" enabled="true" runInBatchMode="false"/>
    <factorypathentry kind="WKSPJAR" id="/HelloAndroidDependencies/libs/codemodel-2.4.1.jar" enabled="true" runInBatchMode="false"/>
</factorypath>

4) Download http://actionbarsherlock.com/ in the filesystem and follow the instruction at http://actionbarsherlock.com/usage.html
(create a project and add it as library to this project). then readd all libraries.
