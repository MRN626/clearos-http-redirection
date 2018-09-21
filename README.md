# **clearos-http-redirection**
  When we try to open the Administration login page, without typing "httpS" first, 
  the site doesn't redirect or provide a link   to the correct address, it only shows an error message.
  these configurations allow to redirect the request http to https
 
# **License**
  this project project use LGPLv3 licence

# **Prerequisites**
  firstly you should have clearos install on your machine and make sure
  to install and configure a server httpd

# **Installing**

  *to make it go to the next move:
    **/usr/clearos/sandbox/etc/httpd/conf.d/**
  
  *replace the **framework.conf** and **devel.conf** file with the file in the folder you are going to download

  *then open the two file using a text editor then look for that line: 
  
  **ErrorDocument 400 https://ip:1501/app/base/session/login/**
  
  *then replace **ip** on this line with your IP address
    do not forget this line is taken over for port 81 83 and 1501
  
# **Running the tests**

  after that make sure you have everything changed in the last step go in your browser and try to access a page 
  using the http protocol like this: **http://your ip adress:port/app/base/session/login**
  instead of having a bad request error you will be redirected to the secure page
  
# **Contributing**


if you have any problems report to the following address:
e-mail: ngalukiyemaureen@gmail.com 
https://github.com/orgs/itotafrica

to join our community go to:
https://itotafrica.com/forum/ or https://www.clearos.com/clearfoundation/social/community

**do not miss the improvements**


  
