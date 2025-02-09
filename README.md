# CI/CD Tutorial
1.	Create GitHub repository.
2.	Click add file
3.	Create directory structure: your_repo/.github/workflows/superlinter.yml
4.	Make sure the directory structure follows the format above!
5.	Copy and paste the YAML code from https://github.com/antr0n/CI_CD_Demo/blob/main/.github/workflows/superlinter.yaml
6.	Commit file to main
7.	Quickly navigate back to your repository and click the Actions tab at the top
8.	Here you can see your workflow running! Click it to see what it’s doing (it should be setting up the job or linting).
9.	Now we can test if the linter is working. Add a new python file (main.py) to main and copy paste the following code:
```Python
def hello():
    print("hi")

def bye():
  print("bye")

print(hello())
```
10.	Commit the python file to main and then quickly navigate back to the actions tab. Click the latest workflow run at the top of the list then click the lint codebase job and watch the automation in action!
11.	The linter should fail. To check the errors scroll down to the Run Super-Linter section. The error should be around lines 169-184.
12.	Fix the errors and commit your python file again. The lint code base job should succeed.
13.	Congratulations! You implemented continuous integration using GitHub Actions!
14.	From here you could deploy a continuous deployment workflow that automatically deploys your code to a server, docker image, or something else. Thanks for participating!
