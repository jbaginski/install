# Calabash Install Scripts for OS X and Windows

Two scripts for installing the Calabash gems on your computer.



## Installing on OS X
On OS X Maverics and above, Ruby is already installed in version 2.0 or above. On these systems installing Calabash without having to call sudo can be done by running this command


    ruby <(curl -fsSL https://raw.githubusercontent.com/calabash/install/master/install-calabash-local-osx.rb)

Obviously we recommend reading through that script before actually running it.

### Configuration

After installing you should add the following lines to your bash or zsh configuration files (usually `~/.bash_profile` or `~/.zshrc`)

    export GEM_HOME=~/.calabash
    export GEM_PATH=~/.calabash
    export PATH="$PATH:$HOME/.calabash/bin"

Then restart the terminal or source the appropriate configuration file.

### Using bundler

You can download the sample Gemfile with this command 


    curl -fsSL https://raw.githubusercontent.com/calabash/install/master/Gemfile -o Gemfile
    
Copy the Gemfile to the directory where you want to keep your Calabash tests and run the command `bundle install`.


## Installing on Windows

You must first have [Ruby installed](http://rubyinstaller.org/) along with the RubyInstaller DevKit installed. Once you have this done, download the Powershell script `install-calabash-local-windows.ps1` and run it using Powershell.

