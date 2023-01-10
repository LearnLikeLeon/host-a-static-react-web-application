# host-a-static-react-web-application
Develop and deploy a simple web application using a continuous integration and continuous delivery environments in the cloud.

![A sketch of the architecture used to explain this project](https://user-images.githubusercontent.com/121564302/211456534-692c8920-60d5-41bb-9a6e-8bc2938f11ee.png)

## Create the project scaffold :

  * Create a new GitHub repository which will be used for this project with a 'README' file and a '.gitignore' file.

  * Create development environment that is cloud-based such as : 
      ### AWS CloudShell
      ### AWS Cloud9
      
  * Create and initialize a repository :
      - The easiest way to do this is by using the command ' create-react-app '. 
      - Install this package using the following command in your Command Prompt or the terminal of your cloud-based IDE.
      - Run the following commands :
      
            $ npx create-react-app {application_name}
            $ cd {application_name}
            $ code .
            $ npm start
        
      - Initialize git :
        
            $ git init
        
      - Add the Remote Repository available in your server :
      
            $ git remote add {default_name_of_your_remote_server} git@github.com:{username}/{your_remote_repository_name}.git
            $ git remote -v
        
      - In case your remote server is ahead with some changes :
      
            $ git pull {default_name_of_your_remote_server} {branch_name_of_your_remote_repository}
            $ git status
            $ git add {filename_1.extension} {filename_2.extension}.....{filename_n.extension}
            $ git commit -m " A meaningful message regarding the achieved milestone in this project "
            $ git push -u {default_name_of_your_remote_server} {branch_name_to be pushed in_your_remote_repository}
        
     * Link your remote repository with AWS Amplify Services :
     
        - After you authorize the AWS Amplify Console, AWS Amplify fetches an access token from the repository provider, but it doesn’t store the token on the AWS               servers.             
        - AWS Amplify accesses your remote repository using deploy keys installed in a specific repository only.
        
     * Configure, review and confirm your application's build and test settings. 
     
     * Save and deploy your web application through a global content delivery network (CDN).
 
