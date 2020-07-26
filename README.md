# msa-devops-2020

Website URL: https://msa-2020-devops-pbhu540.azurewebsites.net/

Build pipeline: 
- The pipeline triggers a build to occur based on the set triggers, which are: if changes are committed to the 'Master' and 'Develop' branches. Following that the pipeline goes through the steps laid out in the azure-pipelines.yml gfor what should happen in the build for the web app to be built properly on targetted hardware. 

Release Pipeline:
- Release pipeline first has a filter applied to only occur if a build is produced in the build pipeline for the 'Master' branch. The release pipeline takes the artifacts from the build pipeline (I.e build instructions for the web app) and deploys it to the live website that is hosted by Microsoft Azure at the given URL above.
One thing to note about the release pipeline is everyone would have a unique URL, as such knowing when to make changes to the given instructions is important for it to deploy properly to my own website.
