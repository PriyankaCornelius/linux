1- Fork torvalds/linux repository and clone it.

2- Install all the dependancies necessary to build kernel on your system usin the following commands:-

sudo apt-get build-dep linux linux-image-$(uname -r)

sudo apt-get install libncurses-dev gawk flex bison openssl libssl-dev dkms libelf-dev libudev-dev libpci-dev libiberty-dev autoconf

3- Create a new directory 'cmpe283' inside the cloned Linux folder.

4- Copy files 'Makefile' and 'cmpe283-1.c' to the cmpe283 folder.

5- Inside the cmpe283 directory, build the module using the following commands:-

cd cmpe283

make all

6- List the files inside the cmpe283 directory to check if the kernel object got created using the ls command.

7- Run the kernel object and display the contents of the MSR using the following commands:-

sudo insmod cmpe283-1.ko

sudo rmmod cmpe283-1.ko

dmesg
