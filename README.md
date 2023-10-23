# Yolomy E-commerce Application: Deployment using Ansible & Vagrant
## Prerequisites
Make sure that you have the following installed:
- [Vagrant](https://developer.hashicorp.com/vagrant/downloads)
- [Ubuntu 22.04 Vagrant Box](https://app.vagrantup.com/centos/boxes/7)

## Setting up Vagrant
- To set up Vagrant, follow: [link](https://developer.hashicorp.com/vagrant/downloads).
- Verify that Vagrant is installed by running:
  
  ```vagrant --version```
  The output should be as this:
  
  ```Vagrant 2.4.0```

- Upon successful installation of Vagrant, install CentOS/7:
  
  ```vagrant box add generic/centos7```

- Upon successful setup of CentOS/7, follow up with the next steps.

## Running the application

#### Clone the repository
```
git clone https://github.com/momureithi/My-IP3-Config-Management-Project.git
```

#### Change into the `My-IP3-Config-Management-Project` folder
```
cd My-IP3-Config-Management-Project
```


#### Automate deployment of the Yolomy e-Commerce web application using Ansible and Vagrant
 ```
 vagrant up --provision
 ```

#### Access the Yolomy e-Commerce web application from the browser

```
http://localhost:3000
```

#### Go ahead and add a product (note that the price field only takes a numeric input)