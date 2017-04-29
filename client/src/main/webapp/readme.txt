Instructions for using the OpenShift Container Platform OC Client

1.  Double-click the zip file in this directory to obtain the oc.exe file.
2.  Copy the file to your c:/users/<networkID>/bin directory.
3.  From the Git Bash prompt (installed separately), enter "oc login --server=ocp.ose.frb.org:8443"
      Provide your Windows network ID and password.
4.  If you are denied access, request access to your District's OpenShift developer group.

After getting logged in, you can begin creating applications with either the command line client or the browser.
To use the web console, browse to https://ocp.ose.frb.org:8443/console

Some oc commands are:

oc new-project <project>  ! create a new project
oc projects               ! list projects
oc project <project>      ! switch to a project
oc get all                ! get information on pods in your project
oc get templates -n openshift   ! list available templates
oc describe <resource>          ! examine project resources
oc new-app <image> -n <name>    ! create a new application within your project
oc env bc/<name> <environment-variable>=<value>


More information on the Red Hat OpenShift Container Platform can be found at docs.openshift.com
