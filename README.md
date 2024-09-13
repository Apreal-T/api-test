# Postman Collection Runner

This repository contains Postman collections that can be executed using GitHub Actions. The purpose of this project is to automate API testing using Postman and Newman.

## Table of Contents

- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Running the Collection Locally](#running-the-collection-locally)
- [GitHub Actions Workflow](#github-actions-workflow)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

To get started with this project, follow the steps below:

1. Clone the repository:
   
   git clone https://github.com/yourusername/repository-name.git
   cd repository-name
Install Postman to manage your API collections.

Import the Postman collection from the collections folder.

Prerequisites
Node.js (for running Newman)
Newman (Postman CLI)
You can install Newman globally using npm:


npm install -g newman
Running the Collection Locally
To run the Postman collection locally, use the following command:


newman run path/to/your/collection.json
You can also specify environment variables if needed:


newman run path/to/your/collection.json --env-var "key=value"
GitHub Actions Workflow
This repository includes a GitHub Actions workflow that automatically runs the Postman collection on every push to the main branch.

Workflow File
The workflow file is located at .github/workflows/postman.yml. It includes steps to:

Checkout the repository
Install Newman
Run the specified Postman collection
Manual Trigger
You can manually trigger the workflow from the GitHub Actions tab in your repository.

Contributing
Contributions are welcome! Please follow these steps to contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit them (git commit -m 'Add new feature').
Push to the branch (git push origin feature-branch).
Create a pull request.
