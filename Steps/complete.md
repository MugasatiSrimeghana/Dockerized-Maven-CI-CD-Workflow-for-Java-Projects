## Steps to create a pipeline
- Go to the Jenkins server
- Click on the 'New Item' in the left side of the dashboard
- Give a name as maven-pipeline
- Select 'Pipeline' and click 'OK'
- Scroll down to the 'Pipeline' section and select 'Pipeline script from SCM' in the 'Definition' dropdown
- Select 'Git' in the 'SCM' dropdown
- Give the repository URL as
```
https://github.com/your-user-name/repo-name.git
```
- Click 'Save'
- Click 'Build Now'
- So we have to make changes in the `build-jar.sh` file and `test.sh` file , You can refer my repository for the changes.
- After done the Changes , Build the project again
- Now the project will be built successfully
- Click on the build number
- Click on 'Console Output' to see the output
- If you see the output as 'Success' then the pipeline is working fine
- If you see the output as 'Failure' then check the error and fix it
- If you see the output as 'Aborted' then check the error and fix it
- May be you will find errors but keep troubleshooting , I also got errors many times

<img width="1308" height="666" alt="image" src="https://github.com/user-attachments/assets/d5ade30e-c62e-4df0-a006-e038a53147fd" />



## Final Result

<img width="1920" height="922" alt="pickchu" src="https://github.com/user-attachments/assets/17c1688b-cbaa-47d9-b252-8444f828c08b" />

