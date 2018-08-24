# **clearos-http-redirection**

  these configurations allow to redirect the request http to https

# **Prerequisites**
  as a prerequisite you must have a clearos and a server httpd configure

# **Installing**

  *to make it go to the next move:
    **/usr/clearos/sandbox/etc/httpd/conf.d/**
  
  *replace the framework.conf and devel.conf file with the file in the folder you are going to download

  *then open the two file using a text editor then look for that line: 
  **ErrorDocument 400 https://your ip adress:1501/app/base/session/login/**
  and put your ip address,do not forget this line is taken over for port 81 83 and 1501
  
# **Running the tests**

  after that make sure you have everything changed in the last step go in your browser and try to access a page 
  using the http protocol like this: **http://your ip adress:port/app/base/session/login**
  instead of having a bad request error you will be redirected to the secure page
  
  **do not miss the improvements**

  
