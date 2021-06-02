Instructions:

1) The package contains 6 files.
   
   1.1) FSDockerfile
   1.2) switch.conf.xml
   1.3) freeswitch.xml
   1.4) default.xml
   1.5) testplivo1.xml
   1.6) testplivo2.xml
   
2) After copying the above files to a directory, we need to build a docker image from dockerfile
   
  $ docker build -f FSDockerfile .
  
3) Once the build is successful, we will get an image-id, which is used in this step  

  $ docker run --network host --rm -d <image-id>
  
4) Now we have freeswitch container running, we can register our clients now.
