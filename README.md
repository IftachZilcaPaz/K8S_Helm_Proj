
# Helm Chart for Creating HTTPD, MySQL, and NGINX Pods.

This Helm chart project creates a Kubernetes deployment consisting of three pods, each running a container: one HTTPD (Apache), one MySQL, and one NGINX.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before you begin, ensure you have met the following requirements:
- You have a Kubernetes cluster up and running.
- You have Helm installed on your local machine. [Install Helm](https://helm.sh/docs/intro/install/)

## Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```
2. Install the Helm chart:
   ```bash
   helm install mychart ./chart-directory
   ```

## Usage

To verify that the pods are running, use the following command:
  ```bash
  kubectl get pods
  ```
You should see three pods listed, one for each container (HTTPD, MySQL, and NGINX).

## Configuration

You can customize the deployment by modifying the `values.yaml` file within the Helm chart directory. Here are some common configurations you might want to change:

- **HTTPD Image:** Change the HTTPD container image.
- **MySQL Image:** Change the MySQL container image and set environment variables like `MYSQL_ROOT_PASSWORD`.
- **NGINX Image:** Change the NGINX container image.

Example `values.yaml`:
```yaml
httpd:
  image: httpd:latest

mysql:
  image: mysql:latest
  env:
    MYSQL_ROOT_PASSWORD: examplepassword

nginx:
  image: nginx:latest
```

Apply changes by running:

```bash
helm upgrade mychart ./chart-directory
```

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request. We welcome any improvements or fixes!

1. Fork the repository.
2. Create a new branch.
3. Make your changes and commit them.
4. Push to your fork and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.




