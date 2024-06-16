# Postman-GitHub-Integration
A demonstration project for integrating Postman API testing with GitHub CI/CD workflows. This repository includes automated tests for API endpoints and showcases continuous integration using GitHub Actions.
## Contents
- **Postman Collection**: A collection of API requests including GET, POST, PATCH, and DELETE operations.
- **Postman Environment**: A configurable environment for managing variables and endpoints.
- **GitHub Actions Workflow**: CI workflow files to automate testing and deployment.

## Setup Instructions

### Prerequisites
- Postman installed on your local machine.
- A GitHub account.

### Postman Setup

1. **Import the Postman Collection**:
    - Open Postman.
    - Click on the `Import` button and select the collection file `Postman-Collection.json`.

2. **Create an Environment**:
    - Click on the `Environments` tab.
    - Create a new environment and add the necessary variables (e.g., `baseUrl`, `apiKey`).

3. **Configure Requests**:
    - Ensure that each request in the collection uses the environment variables.

### GitHub Setup

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/Postman-GitHub-Integration.git
    cd Postman-GitHub-Integration
    ```

2. **Create Branches**:
    ```bash
    git checkout -b dev
    git checkout -b master
    ```

3. **Connect Postman to GitHub**:
    - In Postman, go to the `Collections` tab.
    - Select the collection and click on the `...` (three dots) menu.
    - Choose `Export` and save the collection as a JSON file in the repository.

4. **Setup GitHub Actions**:
    - Create a `.github/workflows` directory in the repository.
    - Add a workflow YAML file to automate testing and deployment.

### Running Tests

1. **Execute Tests in Postman**:
    - Open the collection in Postman.
    - Click on the `Run` button to execute all requests and verify the responses.

2. **Continuous Integration**:
    - Push changes to the `dev` branch.
    - Create a Pull Request (PR) to merge changes from `dev` to `master`.
    - GitHub Actions will automatically run the tests and provide feedback.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License.
