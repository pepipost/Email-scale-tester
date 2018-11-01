# Pepipost as Email-scale-tester 🏋 

## Introduction 
  
   Being Developer our first priority of starting implemention of any product is POC(proof of concept). Great POC requires great benchmark but benchmarking with different tools sometimes becomes messy. We are trying to make an utility which can be used flexibly either by UI or command line. 
 
  
### What should be my contribution  ?

  * You need to contribute to this project by building Scale-tester mentioned with requirement below using any coding language.
    
    * Smtp scale tester ([reference](#utilities))
    
    * Api scale tester ([reference](#utilities))
    
    * you can build a UI with backend.
    
      **OR**
    
    * you can build a command line interface.
    
   
### How can i start my contribution ?

  * You can just have read through this great [article](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/) which will help you in contribution to this project, followed by our [CONTRIBUTING.md]()
  
  * [Sign-up]() to pepipost for apikey which will be required for your [Utilities](#utilities) in order to make scale-tester for pepipost-API, activate your account and send your first test mail using our sandbox domain.
  
  * Pepipost APIs from our developers documentation (in order to test pepipost API Scale-test)

<a name="utilities"></a>
### Reference / utilities

  * Smtp Scale tester
  
  ```bash
  pepi-smtp-scaler -h 'smtp.myhost.com' -P 587/25 -t 'anything@sink.pepipost.com' -tmails 10000 -n 5 
  
  options are
  -h        host of smtpmail
  -P        Port no you want to connect
  -t        to emailid for load testing (it varies from client to client)
  -tmails   total no of mails you need to test 
  -n        no of parallel node you want to trigger
  
  Output 
  connection time :: 0.100ms          time taken for connection
  sending speed   :: 100 mails/sec    time taken in seconds/mintues for sending email
  network speed   :: 10 mbps          network speed while testing
  ```
  
  * APIs Scale tester
  
  ```bash
  pepi-api-scaler -h 'https://api.sommething.com/sendemail/' -f 'something@mydomain.com' -t 'anything@sink.pepipost.com' -tmails 100000 -n 10
  
   options are
  -h        host of smtpmail
  -P        Port no you want to connect
  -t        to emailid for load testing (it varies from client to client)
  -tmails   total no of mails you need to test 
  -n        no of parallel node you want to trigger
  
  Output 
  connection time :: 0.100ms          time taken for connection
  sending speed   :: 100 mails/sec    time taken in seconds/mintues for sending email
  network speed   :: 10 mbps          network speed while testing
  
  ```
   *Note :: addition of parameters in input and output is mandatory. Reference can be taken from [apache ab](https://blog.getpolymorph.com/7-tips-for-heavy-load-testing-with-apache-bench-b1127916b7b6)*
   
   *Tips :: use SDK for pepi-api-scaler* :grinning:
 
 #### What are requirements to get my pull request(PRs) accepted ?

  * Brief introduction of your challenge and making.
  * Prerequisites.
  * Installation Guide.
  * Example
  * Usage cases for each functionality.
  * Blog representing you hard work.
  
  You can publish your challenge by creating a pull request here in this reposistory.
  
### cheers :beer:

### All the Best :thumbsup:

## Happy Coding...! :tada:
  

  
  
  
  
   

