---
**Ocean Observatories Initiative Cyberinfrastructure**  
**Integrated Observatory Network (ION)**  
**java-template-project**

---

# Description
This project is designed to serve as a starting point for future Java based projects on in the OOI-CI

**References**  

# Using the Template Project
1. Clone the project from:  

    git clone git@github.com:ooici/java-template-project.git  


1. Rename the project folder

    mv -r java-template-project [project-name]

1. Remove the *.git* directory

    cd [project-name]
    rm -rf .git

1. In the following files, replace all instances of **[project-name]** with the name of your project
  * ivy.xml
  * build.properties
  * build.xml
  * README.md

1. If your project is hosted somewhere other than the **ooici** github organization (atypical), change line 18 of *README.md* as appropriate

1. In the <u>javadoc</u> target of the *.settings/ooici-build.xml* file, replace the two instances of *[project-title]* with a title for your project

1. Put your java source files (with package hierarchy) inside the **src** directory

1. If your project has a default launch-point (main class), you can specify it in the *build.properties* file in the **runtime.main.class** property - this class will be used when the compiled jar is launched

1. **IMPORTANT** Delete/rename this file and rename *TEMPLATE-README.md* --> *README.md*

1. Refer to the *README.md* file for specifics on compiling and packaging your project.  For distribution/release mechanisms, contact Jamie Chen

# Push Your New Project to Github
1. Create a new github project (or have an authrized person make one for you) - **NOTE:** the url for this project should match what is specified on line 18 of *README.md*

1. Initalize your project as a git repository

    git init

1. Add the repository as a remote for your project

    git remote add ooici git@github.com:ooici/[project-name].git
    git branch --set-upstream ooici

1. Commit *all* of the files in the project

    git add -r *
    git commit -am "[your commit message]"

1. Push your changes to the github repository

    git push ooici master:master