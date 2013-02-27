make_kernel
===========

Compile a set of kernels with a set of predefined options/suffixes.

If you are constantly finding yourself recompiling kernels and just changing one or two options like cpu type and virtio support, this script is just for you.


How it works
===========

Open up the configuration file and add the options you want to use following the example there. Then:

 # cd /path/to/your/kernel/
 # make_kernel -s "CompanyA" -o opteron virtio ipv6

If you set an option in the config file but didn't specificaly called it in the command line the script will NOT CHANGE anything.

Options
===========
 -s suffix
 -o list of predefined kernel options
 -h help
