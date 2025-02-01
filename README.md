# Assessable_Activity2_WAD_2024_25
## Activity 1: EC2 instance
0. Open Amazon Web Services and go to EC2 Service
1. Create a security group for HTTP, HTTPS and SSH
2. Create an Ubuntu EC2 instance
3. Create an elastic IP address and allocate it to the instance
4. Connect to your instance via SSH from your host machine
5. Install apache2, nodejs, npm and express
6. Download the react Project from GitHub
7. Modify the package.json to add your public DNS in the homepage
8. Inside the project install the dependencies with npm install and build the project with npm run build
9. Configure the file for Apache2 VirtualHost, adding the public DNS as the ServerName, and the Proxy directives to connect to http://localhost:5173
10. Enable proxy modules, disable default Apache2 configuration and enable your file
11. Start the server with pm2 command inside the project directory
12. Open your browser and go to your public DNS http://ec2-34-234-48-114.compute-1.amazonaws.com

## Activity 2: S3 bucket
0. Open Amazon Web Services and go to S3 Service
1. Create a bucket
2. Configure te Static Web Hosting by enabling it,and adding the index document as index.html
3. Change the access to the bucket to Public Access
4. Generate a S3 Bucket Policy with this Statement characteristics:
	- Principal: *
	- Action: getObject
	- ARN: your-arn-name/*
5. In the Objects tab, drag the files of your project
6. Go to the website URL that is generated in the Static web hosting section http://my-vite-bucket-daw-mbg.s3-website-us-east-1.amazonaws.com

## Activity 3: GitHub
0. Go to GitHub and log in with your user
1. Create the new repository and add an empty README.md
2. Open the EC2 instance
3. Configure the SSH keys to connect to your GitHub from the EC2 instance
4. Clone your empty project to local
5. Copy the VirtualHost file configuration to your repository and ejecute add, a commit and then push it to the remote repository.
6. Edit the README.md and repeat the add, commit, and push.
7. Verify en each step what you are doing by checking git status and logs.
