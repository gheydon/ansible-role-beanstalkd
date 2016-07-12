Role Name
=========

Beanstalk is a simple, fast work queue.

Its interface is generic, but was originally designed for reducing the latency of page views in high-volume web applications by running time-consuming tasks asynchronously.

Requirements
------------

None

Role Variables
--------------

beanstalkd_listen_addr: 
  Address for beanstalk to listen on.
  default: 127.0.0.1

beanstalkd_listen_port:
  Port for beanstalk to listen to.
  default: 11300

beanstalkd_extra:
  Additional command line arguments to be used when beanstalkd is invoked

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: gheydon.beanstalkd, beanstalkd_listren_addr: 127.0.0.1, beanstalkd_listen_port: 113300 }

License
-------

BSD

Author Information
------------------

Gordon Heydon <gordon@heydon.com.au>