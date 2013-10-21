App42PaaS-Sinatra-MongoDB-Sample
================================

Sample Sinatra App with MongoDB for App42 PaaS Platform

## Getting Start with App42

1. Setup infrastructure for required environment
2. Create service
3. Deploy a Sinatra application

### Setup infrastructure for required environment

    $ app42 setupInfra   
    
### Create service

    $ app42 createService
    
DB Configure for Production environment (application_root_dir/app.rb) 

    # Production
     config.sessions = {
       :default => {
       :hosts => ["<host>:<port>"], # VM IP and VM Port
       :database => "<database name>", # Database Name
       :username => '<username>', # User Name
       :password => '<password>' # Password
     }
    
### Deploy a Sinatra application

    $ app42 deploy

#### Get application details:

    $ app42 appInfo --app AppName    
    
Visit your application:

