- install node version 14.15.0:
    nvp install 14.15.0
    nvm use 14.15.0

- Install project enviroment:
    - install AWS CLI
    - install git
    - install python
    - install virtual enviroment & add the path in the enviroment
    - install EB CLI
        source: https://github.com/aws/aws-elastic-beanstalk-cli-setup

- Inside desired directory clone (download) the app:
    git clone https://github.com/Amin-Wassef/Hosting-A-Full-Stack-App.git

- create eb environment (for the first time only from the app):
    eb create =>    environment name
                    application name
                    classic
                    N

- App Deployment (git push):
    - At the frontend:
        - install dependencies:
            npm install
        - build frontend:
            npm run build
        - deploy changes:
            eb deploy
    - At the backend:
        - install dependencies:
            npm install
        - build backend:
            npm run build
        - deploy changes:
            eb deploy