# Spectrum Workspace

The Spectrum workspace is a modified workspace for Symphony 2.0.5. It is deprecated in favour of the [official workspace repository](http://github.com/symphony/workspace).

## The Original Purpose

The original idea was to clean up the data base of the default Spectrum theme. [This has now been done](http://symphony-cms.com/community/discussions/24571/1/#position-8), for the most part.

I have modified this repository to be identical to the default Spectrum theme. This now serves as a demonstration for creating an all-inclusive ensemble repository. Even for that, it is unnecessary.

## Install from Spectrum Ensemble ZIP Archive

There are a few ways to install this workspace. Depending on what you prefer, you might like to simply download a complete ZIP file. Go to the downloads area to download the ZIP file, which contains the Symphony 2.0.5 core application, all required extensions, and the Spectrum workspace. This is the simplest, if you want to avoid using Git altogether.

## Install Spectrum Ensemble via Git

Refer to the [bauhouse/sym-spectrum](http://github.com/bauhouse/sym-spectrum) or the [official Symphony 2 repository](http://github.com/symphony/symphony-2) for the complete install instructions for Symphony 2. This install may be slightly different than the official symphony-2 repository, as I have updated extensions to the latest releases as of 25 July 2009.

	git clone git://github.com/bauhouse/sym-spectrum.git

That should be all. Install Symphony as usual. (Find the instructions at the [official Symphony 2 repository](http://github.com/symphony/symphony-2).)

## Install Symphony and Spectrum Workspace via Git

The Spectrum Ensemble repository brings together the Symphony 2.0.5 core application, the required extensions and the Spectrum workspace to simplify the install process. If you'd rather put everything together yourself, the process looks something like this:

	git clone git://github.com/symphony/symphony-2.git

Initialize the submodules

	git submodule init

Update the submodules

	git submodule update
	
At this point, all the files required for a clean install are ready. The second branch that has been included as a submodule is the workspace, which is referring to a specific commit of the spectrum branch of my fork of the Symphony workspace repository. To clone this fork separately, use the following commands:

	git clone git://github.com/bauhouse/workspace.git
	cd workspace
	git checkout -b spectrum
	git pull origin spectrum

