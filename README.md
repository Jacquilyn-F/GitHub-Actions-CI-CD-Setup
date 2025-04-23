<a id="readme-top"></a>  
# CI-CD_GitHub_Actions_Pipeline

## Project Overview

The **CI/CD GitHub Actions Pipeline** project demonstrates how to set up a continuous integration and deployment workflow for a fullstack MERN application. By utilizing GitHub Actions, developers can ensure automated testing and deployment pipelines are enforced, enabling efficient and consistent development practices.

This project ensures that all Cypress component tests are run when a Pull Request is made to the `develop` branch, and the application is automatically deployed to Render when code is merged into the `main` branch.

## Features

- **CI with GitHub Actions**: Automatically runs Cypress component tests on PRs to `develop`.
- **CD to Render**: Auto-deploys app to Render when merging to `main`.
- **MERN Stack Support**: Fullstack JavaScript stack (MongoDB, Express, React, Node.js).
- **Custom Deploy Hook**: Secure and manual trigger using Render's deploy hook.
- **Git Flow Strategy**: Utilizes `main`, `develop`, and `feature/*` branches for structured releases.

## Getting Started

Follow the instructions below to get started with the CI/CD pipeline setup for your MERN application.

### Prerequisites

Ensure you have the following installed and configured:

- **GitHub Account** with an existing repository
- **Node.js & npm**
- **MongoDB Atlas** (or a local MongoDB instance)
- **Render Account**
- **Cypress** (added as a dev dependency)
- **Configured GitHub Secrets** (Render deploy hook URL and API Key)

### Installation

1. **Upload Starter Code**  
   Upload the contents of the `Develop` folder to your GitHub repository.

2. **Create Branches**  
   Set up a `develop` branch and a `main` branch in your repo. All PRs should target `develop`; only `develop` should be merged to `main`.

3. **Configure Render**  
   Deploy your app manually once via Render. Then:
   - Disable auto-deploy from the Render dashboard.
   - Copy the `Deploy Hook` URL and add it to your GitHub repo secrets.

4. **Set Up GitHub Actions**

   - Create two YAML workflow files in `.github/workflows/`:

     - `test-on-develop.yml`: Runs Cypress tests on PR to `develop`
     - `deploy-on-main.yml`: Triggers deployment to Render on merge to `main`

   Example secrets to configure:

   - `RENDER_DEPLOY_HOOK`
   - `RENDER_API_KEY`

## Walkthrough Video

Check out the walkthrough video that demonstrates the GitHub Actions pipeline from PR to deployment:

- [Walkthrough Video](https://your-video-link.com)

## Technologies Used

- **Frontend**: React
- **Backend**: Node.js, Express.js
- **Database**: MongoDB Atlas
- **Testing**: Cypress
- **CI/CD**: GitHub Actions
- **Deployment**: Render

## License

This project is licensed under the MIT license.

## Questions

If you have any questions, feel free to contact me:

- 📧 [jacquilyn.fletcher89@gmail.com](mailto:jacquilyn.fletcher89@gmail.com)
- 💻 [Jacquilyn-F](https://github.com/Jacquilyn-F)

<p align="right">(<a href="#readme-top">back to top</a>)</p>