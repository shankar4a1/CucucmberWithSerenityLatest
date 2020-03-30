
src
  + main
  + test
    + java                        Test runners and supporting code
    + resources
      + features                  Feature files
          + search                  Feature file subdirectories 
             search_by_keyword.feature 
       + webdriver                 Bundled webdriver binaries
         + linux
         + mac
         + windows 
           chromedriver.exe       OS-specific Webdriver binaries 
           geckodriver.exe
```

Requirment is to get only tag specicifc  features under Requirments tabs 
Commands:

Requirements are not getting listed under Requirments tabs using below commands

mvn clean verify -Dcucumber.options="--tags @smoke"


mvn clean verify "-Dcucumber.options=--tags @smoke"


##############################################################

All requirements are  getting listed under Requirments tabs using below command
mvn clean verify -Ddriver=chrome -Dcucumber.filter.tags=@smoke
