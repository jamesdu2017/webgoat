WebGoat is a test J2EE web application provided by the Open Web Application
Security Project (http://www.owasp.org). This directory contains the WebGoat
5.0 sources.

You can use WebGoat Java sources directly for Java vulnerability scanning 
with Fortify Static Code Analyzer. You can perform the scan by running the following commands:

$ sourceanalyzer -b WebGoat5.0 -clean
$ sourceanalyzer -b WebGoat5.0 -source 1.5 -cp "WebGoat5.0/WebContent/WEB-INF/lib/*.jar" WebGoat5.0/JavaSource WebGoat5.0/WebContent
$ sourceanalyzer -b WebGoat5.0 -scan -f WebGoat5.0.fpr

See the Fortify Static Code Analyzer User Guide for full details on how to perform a scan.

Example output for a scan of this project is located in <SCA_Install>/Samples/basic/sampleOutput/WebGoat5.0.fpr.

Important:
Do not make this application accessible outside of your firewall or 
to people you do not trust. It contains planted vulnerabilities for testing.

