# Description: 
  
These are simple implementations of CAPS and CAPS-dark on ns-2.35.  
We have tested CAPS and CAPS-dark in the ubuntu 16.04.1 with Linux kernel 4.8.0-36-generic and 4.13.0-41-generic.
  
# Usage:

### 1. Download "ubuntu 16.04.1" and "ns-allinone-2.35.tar.gz"

You can download "ubuntu-16.04.1-desktop-amd64.iso" from this website:   
http://old-releases.ubuntu.com/releases/16.04.1/

You can download "ns-allinone-2.35.tar.gz" from this website:     
https://sourceforge.net/projects/nsnam/files/allinone/ns-allinone-2.35/ns-allinone-2.35.tar.gz/download
  
### 2. Place all the files： 

Please put the following files or folders  ( 'ns-allinone-2.35.tar.gz', 'ls.h', 'NS2.sh', 'CAPS.patch', 'CAPS-dark.patch', ‘CAPS.sh’, 'CAPS-dark.sh', 'many-to-one.sh', 'many-to-many.sh' and ‘testcase’ )  in the same level directory.  
For example: put all the above files and folders in the folder: "CAPS-NS2-master"

### 3. Installing NS2:
	
	cd CAPS-NS2-master
	sudo chmod -R 777 *
	sudo ./NS2.sh
  
### 4. Patching CAPS and Compiling NS2:
	
For CAPS:

	sudo ./CAPS.sh
	
or: For CAPS-dark (Another CAPS version without prior knowledge):
 	
	sudo ./CAPS-dark.sh
	
**Note:** All the patch files ('CAPS.patch' and 'CAPS-dark.patch') should be patched on the original ns-2.35.  
Please put the patch files inside the 'ns-allinone-2.35' folder, but outside the 'ns-2.35' folder. 
  
### 5. Now you can run the simple testcases:

	./many-to-one.sh 10 20 30 40 50 60 70 80
	./many-to-many.sh 10 20 30 40 50 60 70 80
	
 
If you have any questions, please email to jinbinhu@126.com
