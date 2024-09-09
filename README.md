This repository contains an example CI pipeline that bundles a MatLab AppDesigner app into standalone installers for each platform.

## Instructions

* You need a **MatLab Batch Licensing Token** for this. If you are affiliated with Heidelberg University, you can get in touch with the [Scientific Software Center](https://ssc.uni-heidelberg.de) for assistance. Otherwise, you need to apply for [MatLab's Batch Licensing Pilot](https://www.mathworks.com/support/batch-tokens.html)
* Add the batch licensing token to your repository as [a secret](https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions#creating-secrets-for-a-repository) called `MATLAB_LICENSE_TOKEN`
* Copy the `matlab-bundle.yml` file into the `.github/workflows` folder of your project
* Adjust the bits marked as `TODO` in that file

Upon pushing to the `main` branch of your repository, the installers will first be created. You can download them from the Github Workflow run overview upon successful completion.

## License

The provided workflow is licensed CC-0. The contained example app is copyrighted by MathWorks and provided purely for the sake of demonstrating the workflow.
