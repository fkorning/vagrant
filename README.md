═══════════════════════════════════════════════════════════════════════
# Vagrant
═══════════════════════════════════════════════════════════════════════

# Vagrant provisioner

	
<code> 

	#=============================================================================#
	# Manufakture Vagrant
	#-----------------------------------------------------------------------------#

                                  _____        __      __                        
      _____ _____    ____  __ ___/ ____\____  |  | ___/  |_ __ _________   ____  
     /     \\__  \  /    \|  |  \   __\\__  \ |  |/ /\   __\  |  \_  __ \_/ __ \ 
    |  Y Y  \/ __ \|   |  \  |  /|  |   / __ \|    <  |  | |  |  /|  | \/\  ___/ 
    |__|_|  (____  /___|  /____/ |__|  (____  /__|_ \ |__| |____/ |__|    \___  >
          \/     \/     \/                  \/     \/                         \/ 


	#-----------------------------------------------------------------------------#
	# (c) Francis Korning 2024.
	#=============================================================================#
 	                                                                              
</code>		
	
	
───────────────────────────────────────────────────────────────────────
## Preqequisites
───────────────────────────────────────────────────────────────────────

Make sure you have a *Manufacture* SysWin and CygWin full POSIX system running and installed.

	https://sourceforge.net/p/manufacture/syswin/

	https://sourceforge.net/p/manufacture/cygwin/

Manufacture provides the "su.exe" command to run administrator shells (instead of powershell).

In addition to cygwin, you'll probably have a separate gitbash (installed by DockerToolBox).

	
───────────────────────────────────────────────────────────────────────
# Installation
───────────────────────────────────────────────────────────────────────

	mkdir -p C:/work/Vagrant/vagrant-2.4
	
	cd C:/work/Vagrant
	
	# wget https://releases.hashicorp.com/vagrant/2.4.1/vagrant_2.4.1_linux_amd64.zip

	wget https://releases.hashicorp.com/vagrant/2.4.1/vagrant_2.4.1_windows_amd64.msi

	msiexec /i "vagrant_2.4.1_windows_amd64.msi" INSTALLDIR="C:\Work\Vagrant\vagrant-2.4" TARGETDIR="C:\Work\Vagrant\vagrant-2.4" /qb

	
───────────────────────────────────────────────────────────────────────
# Configuration
───────────────────────────────────────────────────────────────────────
	
* Set SYSTEM environment variables

	VAGRANT_HOME=c:\work\Vagrant\vagrant-2.4
	
	PATH=%PATH%;c:\work\Vagrant\vagrant-2.4\bin
	

* Restart the system

	 
───────────────────────────────────────────────────────────────────────
# Extension
───────────────────────────────────────────────────────────────────────

* Install Guest Extension Plugins 

	vagrant plugin install vagrant-disksize
	
	vagrant plugin install vagrant-vbguest
	

* Login 

	vagrant login
	
═══════════════════════════════════════════════════════════════════════
# (c) Francis Korning 2024.
═══════════════════════════════════════════════════════════════════════
