Here is a Jenkins CLI and Management Cheat Sheet in Markdown. This covers the command-line interface (CLI), common service commands for Linux, and API-based triggers. 
🚀 Jenkins Service Management (Linux)
If you are running Jenkins on a Linux server (Ubuntu/CentOS), use these to manage the service. 
Command 	Description
sudo systemctl start jenkins	Start the Jenkins service
sudo systemctl stop jenkins	Stop the Jenkins service
sudo systemctl restart jenkins	Restart Jenkins (common after plugin updates)
sudo systemctl status jenkins	Check if Jenkins is running or has errors
sudo systemctl enable jenkins	Set Jenkins to start automatically on boot
tail -f /var/log/jenkins/jenkins.log	View real-time Jenkins logs for troubleshooting
🛠️ Jenkins CLI (jenkins-cli.jar)
To use these, you first need to download the CLI tool from your instance at http://[your-jenkins-url]/cli. 
Command 	Description
java -jar jenkins-cli.jar -s [URL] help	List all available CLI commands
java -jar jenkins-cli.jar -s [URL] build [JobName]	Trigger a specific build/job
java -jar jenkins-cli.jar -s [URL] list-jobs	List all jobs in the current view
java -jar jenkins-cli.jar -s [URL] safe-restart	Restart Jenkins after all jobs finish
java -jar jenkins-cli.jar -s [URL] install-plugin [ID]	Install a plugin by its short ID
java -jar jenkins-cli.jar -s [URL] get-job [JobName]	Export a job's configuration to XML
🌐 Jenkins API (using curl)
You can trigger Jenkins actions using standard Linux networking commands. 
Command	Description
curl -X POST [URL]/job/[JobName]/build	Trigger a build via API
curl -u [user]:[token] [URL]/info	Get Jenkins system info in JSON format
curl -X POST [URL]/safeRestart	Initiate a safe restart via web request
🐳 Jenkins in Docker
If you run Jenkins as a container, use these Docker commands: 
Command 	Description
docker logs -f [container_id]	View Jenkins logs inside the container
docker exec -it [id] /bin/bash	Open a terminal inside the Jenkins container
docker restart [container_id]	Restart the Jenkins container
🔑 Important Note: Authentication
For most CLI and API commands, you will need an API Token. 
Log in to Jenkins.
Click your Username (top right) -> Configure.
Under API Token, click Add new Token.