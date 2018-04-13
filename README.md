Role Name
=========

Configures apt to be ready for package installation: 

* Updates sources list
* Installs aptitude
* Performs safe upgrade (otherwise package installation sometimes 
  fails with messed-up old dependencies)

Configures sources list, 

Requirements
------------

Debian 

Role Variables
--------------

    # Mirror to use
    apt_sources_repo_mirror: http://ftp.au.debian.org/debian/
    # Distribution to use 
    apt_sources_distro: stretch
    # Divisions to use e.g. 'main contrib non-free'
    apt_sources_divisions: main
    # Set true if you want to have access to source packages
    apt_sources_include_src: true

License
-------

BSD
