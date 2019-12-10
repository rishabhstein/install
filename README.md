The solvers porousFoam and fractureFoam utilize some of the libraries
from Vitaliy's 3D code. The install scripts and instructions in this
repo should help things go more smoothly. 


First make your local OpenFOAM directory and clone this repository:

mkdir $HOME/OpenFOAM

cd $HOME/OpenFOAM

sudo yum install git

git clone https://github.com/tonyladd/install

Then follow the step-by-step instructions outlined in README:

### Step by step installation:

1. Install development tools first by using following command:

      yum groupinstall 'Development Tools' 
      yum install git zlib-devel texinfo gstreamer-plugins-base-devel \
      libXext-devel libGLU-devel libXt-devel libXrender-devel libpng-devel \
      libXinerama-devel libXrandr-devel libXi-devel libXft-devel \
      libjpeg-turbo-devel libXcursor-devel \
      readline-devel ncurses-devel python python-devel

2. Installation of OpenFOAM by following step:
  ## First download the source
      cd $HOME
      mkdir OpenFOAM
      cd OpenFOAM
      git clone https://github.com/OpenFOAM/OpenFOAM-4.x.git
      git clone https://github.com/OpenFOAM/ThirdParty-4.x.git
      
      cd ThirdParty-4.x
      mkdir download
      

