#### fire up server
``func start --python``

#### SQL Server on macOS

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"   
brew tap microsoft/mssql-release https://github.com/Microsoft/homebrew-mssql-release   
brew update   
HOMEBREW_NO_ENV_FILTERING=1 ACCEPT_EULA=Y brew install msodbcsql17 mssql-tools
```

#### ODBC API
``brew install unixodbc``

#### Install project requirements
``pip install -r requirements.txt --user``

#### Override python version via renaming
``alias python='python3.7'``
