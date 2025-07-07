# Capstone Project - E-Commerce Platform CI/CD (Local Setup)

## Project Overview
This project automates a CI/CD pipeline for an e-commerce platform with a Node.js/Express backend API and React frontend, using GitHub Actions, Docker, and AWS Elastic Beanstalk. It includes caching, linting, versioning, and secure secret management. Executed on WSL Ubuntu with VS Code and Git Bash.

## Setup
- Initiated on Jul 07, 2025, 12:27 PM WAT.
- Used WSL Ubuntu, VS Code, and Git Bash in `C:\Users\Abraham\Documents\Workspace\Ecommerce_Platform`.

## Execution Steps
1. **Project Setup**:
   - Created `api` and `webapp` directories and initialized Git repository.
   - Pushed to `https://github.com/westgrin/ecommerce-platform`.
   - [Screenshot: `github_repo_files_local.png` - Shows repository files.]
2. **Backend API Setup**:
   - Set up Node.js/Express API with product listing, login, and order endpoints.
   - Added tests in `api/__tests__/api.test.js`.
   - [Screenshot: `nodejs_npm_version_local.png` - Shows Node.js and npm versions.]
   - [Screenshot: `api_npm_install_output_local.png` - Shows backend dependency installation.]
   - [Screenshot: `api_npm_test_output_local.png` - Shows backend test output.]
   - [Screenshot: `api_curl_output_local.png` - Shows API endpoint output.]
3. **Frontend Webapp Setup**:
   - Set up React app with product listing, login, and order placement.
   - [Screenshot: `webapp_npm_install_output_local.png` - Shows frontend dependency installation.]
   - [Screenshot: `webapp_output_local.png` - Shows frontend output.]
4. **Docker Integration**:
   - Created Dockerfiles for backend and frontend.
   - [Screenshot: `docker_version_local.png` - Shows Docker version.]
   - [Screenshot: `docker_run_output_local.png` - Shows Docker containers running.]
5. **AWS Elastic Beanstalk Setup**:
   - Initialized Elastic Beanstalk for backend and frontend.
   - [Screenshot: `awscli_version_local.png` - Shows AWS CLI version.]
   - [Screenshot: `eb_setup_output_local.png` - Shows `eb init` and `eb create` output.]
6. **GitHub Actions Workflows**:
   - Added `api.yml` and `webapp.yml` for CI/CD with caching and deployment.
   - Secured AWS credentials with GitHub Secrets.
   - [Screenshot: `github_secrets_config_local.png` - Shows secrets setup.]
   - [Screenshot: `github_actions_run_local.png` - Shows workflow runs.]
   - [Screenshot: `aws_webapp_output_local.png` - Shows deployed frontend.]
7. **Side Hustle Task**:
   - Added linting and versioning to backend workflow, tested with a PR.
   - [Screenshot: `github_release_output_local.png` - Shows release page.]

## Learning Summary
This project consolidated my GitHub Actions, Docker, and AWS skills, automating a full-stack e-commerce platform. I mastered modular workflows, Docker containerization, cloud deployment, and secure secret management, aligning with my DevOps goals (June 16, 2025) for scalable automation.

## Tools Used
- **WSL Ubuntu Terminal**: For Node.js, Docker, AWS CLI, and Git commands.
- **VS Code**: For editing code and `README.md`.
- **Git Bash**: For GitHub operations.
- **GitHub Actions**: For CI/CD automation.
- **Docker**: For containerization.
- **AWS Elastic Beanstalk**: For deployment.

## Project Deliverables
- **Documentation**: This `README.md` with steps and learning summary.
- **Screenshots**:
  - `nodejs_npm_version_local.png`
  - `api_npm_install_output_local.png`
  - `api_npm_test_output_local.png`
  - `api_curl_output_local.png`
  - `webapp_npm_install_output_local.png`
  - `webapp_output_local.png`
  - `docker_version_local.png`
  - `docker_run_output_local.png`
  - `awscli_version_local.png`
  - `eb_setup_output_local.png`
  - `github_repo_files_local.png`
  - `github_secrets_config_local.png`
  - `github_actions_run_local.png`
  - `aws_webapp_output_local.png`
  - `github_release_output_local.png`
- **Script Link**: [GitHub Repository](https://github.com/westgrin/ecommerce-platform)

## Local Development Instructions
1. Clone repository: `git clone https://github.com/westgrin/ecommerce-platform.git`
2. Backend: `cd api`, `npm install`, `node index.js`
3. Frontend: `cd webapp`, `npm install`, `npm start`
4. Docker: Build and run images as shown in Step 4.
5. AWS: Configure `aws configure` and `eb init` as shown in Step 5.

## Troubleshooting
- Fixed `ECONNRESET` error by setting DNS to `8.8.8.8` and clearing npm cache.
- Ensured commands were run in `/mnt/c/Users/Abraham/Documents/Workspace/Ecommerce_Platform`.
- Verified AWS credentials in GitHub Secrets.

## Conclusion
This capstone project successfully automated a CI/CD pipeline for an e-commerce platform, integrating backend, frontend, Docker, and AWS. The side hustle task enhanced my skills in linting and versioning, preparing me for advanced DevOps practices.