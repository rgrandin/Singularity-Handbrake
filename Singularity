BootStrap: docker 
From: fedora:28 


%runscript
    exec ghb


%apprun handbrake
    exec ghb


%post
    dnf install -y https://download0.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download0.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
    dnf install -y http://rpms.famillecollet.com/fedora/28/remi/i386/remi-release-28-3.fc28.remi.noarch.rpm

    dnf --enablerepo=remi install -y libdvdcss

    dnf install -y handbrake handbrake-gui

