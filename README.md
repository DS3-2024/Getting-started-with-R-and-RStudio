# Getting started with R and RStudio


1) Install R
	a. For Mac OS users, you can download R [here](https://cran.r-project.org/bin/macosx/).  
		For R ≥4.1.0 there is a separate build for ARM-based Macs (also known as ‘M1/M2/M3’ and ‘Apple Silicon’).  
		Should have `Xcode Command Line Tools` installed for packages that require compilation - run `xcode-select --install` in Terminal or see [here](https://mac.install.guide/commandlinetools).  
		gfortran issues on Apple Silicon computers: check out the [macrtools R package](https://github.com/coatless-mac/macrtools/).  
	b. For Windows users, you can download R [here](https://cran.r-project.org/bin/windows/base/). 
	c. For Lunix users, you can download R [here](https://cran.rstudio.com/bin/linux/). 

2) Install RStudio IDE
	Download [here](https://posit.co/download/rstudio-desktop/)
	Cheatsheet [here](https://rstudio.github.io/cheatsheets/html/rstudio-ide.html)

3) Updating R and RStudio
https://support.posit.co/hc/en-us/articles/200486138-Changing-R-versions-for-the-RStudio-Desktop-IDE
	a) Mac OS:
		by default the RStudio IDE will run against the current version of R.Framework
		list all of the versions of R.Framework on your system and determine which one is considered the current one by executing the following command in Terminal:
		```
		ls -l /Library/Frameworks/R.framework/Versions/
		```
		To change the current version of R.Framework, you can either:
		Run the installer from CRAN for the R version you want to be current
		Update the R.framework/Versions/Current directory alias directly using ln -s
		To override the RSTUDIO_WHICH_R environment variable to the R executable that you want to run against (add to XXX file)
		```
		export RSTUDIO_WHICH_R=/usr/local/bin/R
		```

	b) Windows users:
		You may need to uninstall R to update it
		On Windows, the RStudio IDE uses the system's current version of R by default.
		You can override which version of R is used via General panel of the RStudio Options dialog. # TEST
		Another option for Windows users is to use a package called installr

	c) On Linux:
		RStudio Desktop IDE uses the version of R pointed to by the output of the following command:
		```
		which R
		```
		To override the RSTUDIO_WHICH_R environment variable to the R executable that you want to run against (add to ~/.profile file)
		```
		export RSTUDIO_WHICH_R=/usr/local/bin/R
		```

	d) Updating RStudio
	   Help > Check for Updates > Quit and Download...




Alternatives
CAVATICA - Data Studio # NEED BILLING GROUP, TEST
Posit Cloud https://posit.cloud/plans/free # NEED TO TEST