TYPO3-Solr-CentosAutostart
==========================

1. Copy the tomcat6 file to /etc/init.d
2. Make sure that the JAVA_HOME value is correct. The script has been tested with CentOS6 and java-1.6.0-openjdk.x86_64 installed via YUM. If you've installed a different version of Java, you will probably need to change the JAVA_HOME variable.
3. Add the startup script to chkconfig with "chkconfig --add tomcat6" as root
4. Set tomcat6 to startup on boot: "chkconfig --level 345 tomcat6 on"

Note: this script is basically a copy of Ingo Renner's startup script for Debian, with the JAVA_HOME path set for CentOS. Thanks, Ingo!

Good luck!