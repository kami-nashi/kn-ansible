# kn-ansible
My own ansible playbooks used in my own environments

Installation Playbooks
 Used to install things from pkg managers, source, or otherwise
  install/vmware-tools.yml - Installs VMWare tools from local webserver, with deps per OS

Update Playbooks
 Used to update packages
  updates/pkg-update.yml - Updates packages via OS's package manager
  
Tasks Directory
  Use these to build up other playbooks ( examples in service/ )
   tasks/service_mc-start.yml   Starts the custom command for multicraft
   tasks/service_mc-stop.yml    Stops the custom command for multicraft
   tasks/service_www-start.yml  aka service apache2|httpd start
   tasks/service_www-stop.yml   aka service apache2|httpd stop
   
Service Playbooks
    service/mc_roll.yml   Completely stops multicraft, www services, then starts them
    service/mc_start.yml  Starts multicraft, www services from a  stopped state
    service/mc_stop.yml   Completely stops multicraft, www services
