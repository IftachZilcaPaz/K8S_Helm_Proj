
![image](https://github.com/IftachZilcaPaz/ci_cd_github_action_aws/assets/151572520/c4b1a850-020a-42af-942a-37f0a8796a49)

---

<p>
<h1> Hey Again &nbsp;<img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" height="45" width="45"/>&nbsp;&nbsp;Welcome To My "K8S_Helm_Proj" &nbsp;=)</h1>
</p>
<br/>

<img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1689486594104/0883007c-df25-4d04-90f9-16a033cece42.gif" align="right" height="250" width="350" />


 <!--- ## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://katherineoelsner.com/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)
--->

## 🌐 Socials:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/iftach-z-19931491/) 

<!---
<img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/iftach-z-19931491/" height="30" width="40" />
--->

## 💻 Languages and Tools:

![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=flat&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/helm-%2523326ce5.svg?style=flat&logo=Helm&logoColor=white&labelColor=yellow&color=yellow)

# 📊 GitHub and More ✨ ):

<img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical" align="right" width="500"/>


# Helm Chart for Creating HTTPD, MySQL, and NGINX Pods

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

Replace placeholders like `your-username`, `your-repo`, and `chart-directory` with the actual values corresponding to your repository and Helm chart directory. This template should provide a comprehensive overview and instructions for your project.




