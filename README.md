Webstack99
==========

* Webstack99 is for the Httpd proxy server (entry point from outdoor) + letsencrypt server


Install
-------

1. Configure httpd server

    * Step1: import http configuration file to container
	`ansible-playbook -i hosts --become --ask-become-pass --tags httpd_configure webstack99_containers_manager.yml`

    * Step2: stop/start webstack99 containers to get letsencrypt certificate

    * Step3: import https configuration file to container
    `ansible-playbook -i hosts --become --ask-become-pass --tags httpd_configure webstack99_containers_manager.yml`
