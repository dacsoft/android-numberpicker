Android 4.0 NumberPicker backported to 2.1  
Requires JakeWhartons NineOldAndroids library. It is included as a jar, but also available at: https://github.com/JakeWharton/NineOldAndroids  
Probably has to be built against API level 15  
  
To use this library, it's required that 4 attributes are added to your theme. Check the sample app on how this is done.

FORKER'S NOTE

This has been modified to build with Maven.

Clone the project and checkout the mavenize branch:
 $ git checkout mavenize
 
Build the library
 $ mvn clean install

Add this to your project POM:

<dependencies>
  ...
	<dependency>
    	<groupId>net.simonvt</groupId>
    	<artifactId>android-numberpicker-library</artifactId>
    	<version>1.0.0</version>
			<type>apklib</type>
  </dependency>
  ...
</dependencies>

Then build your project. Bam!

Hope to have this in the original project someday. 
Can someone help with the deployment to the maven repo?
Thanks to Jake Wharton, king of the universe and the POM files from ActionBarSherlock.
 
    
  