This is an unofficially supported ansible to install and confirm Maker with a set of dependencies. 

CURRENTLY, THIS ANSIBLE HAS ONLY BEEN TESTED WITH Ubuntu

Before you use this ansible, you'll need to setup the following:

* setup your ansible inventory with a group called maker-hosts and add your host(2) to that group
* copy all the directories in the roles/ directory into your ansible roles location
* copy your licensed tarball of maker into the roles/maker/files directory and set the MAKER_TARBALL in the playbook. Currently, this is set to "maker-2.31.8.tgz"
* copy your repeatmasker libs into roles/repeatmasker-v4/files directory and set all files in REPEATMASKER_LIBS in the playbook. Currently, this is set to repeatmaskerlibraries-20140131.tar.gz
* copy your tandem repeats finder binary into roles/repeatmasker-v4/files directory and set all files in TRF_BIN in the playbook. Currently, this is set to "trf407b.linux64"
