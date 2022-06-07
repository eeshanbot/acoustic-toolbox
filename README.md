# acoustic-toolbox
public Github port of the official Acoustics Toolbox provided at [oalib.hlsresearch.com/AcousticsToolbox](oalib.hlsresearch.com/AcousticsToolbox)

### changes needed to run properly
My system is Ubuntu 22.04 and Matlab 2020b; I had to fix where the MATLAB gfortran library was pointing towards. You can read more about this [here](https://stackoverflow.com/questions/9628273/libgfortran-version-gfortran-1-4-not-found). Check what package of MATLAB and gfortran you are using to modify the following bash commands as needed.

	cd /usr/local/MATLAB/R2020b/sys/os/glnxa64
	sudo ln -sf /usr/lib/x86_64-linux-gnu/libgfortran.so.5.0.0 libgfortran.so.5