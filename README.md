# npm-flow
This CI used github actions as the main ci tool.  
The file is in .github/workflows/main.yml  

### CI pipeline trigger
This CI is triggerd when there is a **push** or **pull request** onto main branch.

### Steps in main.yml  
- Based on ubunto image, install nodejs with versions specified in *strategy*.
- Install depencies.
- Run test cases.
- Build app.

### Suggested workflow
If git workflow is used, only pull request event is recommended because after merged the pipeline will be triggered twice due to push event.
