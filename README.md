## config
### Configuration Files

**Miscellaneous Configuration Files**

Using a private pypi repository
File location: $HOME/.pypirc
File location: ~/.pip/pip.conf

####How to Compile and Install Python 3 for static deployments (CentOS)

**Make sure your $HOME variable is set**
*or use the install script*
```
yum groupinstall -y "Development Tools"
yum install -y openssl-devel bzip2-devel expat-devel gdbm-devel readline-devel sqlite-devel
wget http://python.org/ftp/python/3.3.2/Python-3.3.2.tar.bz2
tar xvf Python-3.3.2.tar.bz2
cd Python-3.3.2
./configure
mkdir -p ~/.local
make altinstall prefix=$HOME/.local exec-prefix=$HOME/.local
```

finally, run `enable_python_3`
