# Jenkins CI/CD Demo

This repository demonstrates a complete Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins, Docker, and Python. The project features a simple Python application with automated testing and containerization.

## Project Structure

* `app.py`: The main Python application containing basic logic.
* `test_app.py`: Unit tests for the application using the `pytest` framework.
* `Dockerfile`: Instructions for containerizing the Python application.
* `Jenkinsfile`: Definitive pipeline script for automating the build, test, and deployment process.
* `requirements.txt`: List of Python dependencies required for the project.

## Prerequisites

To run this project, you will need:

* Python 3.11 or later.
* Docker installed and running.
* Jenkins server with the Pipeline plugin and Docker installed.
* Git for version control.

## Getting Started

### Local Development

1. **Install dependencies:**
```bash
pip install -r requirements.txt

```


2. **Run the application:**
```bash
python app.py

```


3. **Run tests:**
```bash
pytest

```



### Docker Containerization

You can build and run the application as a container:

1. **Build the image:**
```bash
docker build -t jenkins-demo-app .

```


2. **Run the container:**
```bash
docker run jenkins-demo-app

```



## CI/CD Pipeline

The project uses a declarative Jenkins pipeline defined in the `Jenkinsfile`. The pipeline consists of the following stages:

1. **Checkout Code**: Retrieves the latest source code from the main branch of the GitHub repository.
2. **Install Dependencies**: Uses `pip` to install necessary packages listed in `requirements.txt`.
3. **Run Tests**: Executes automated unit tests using `pytest` to ensure code quality.
4. **Build Docker Image**: Packages the application into a Docker image tagged as `jenkins-demo-app`.

### Pipeline Notifications

* **Success**: Prints "Pipeline completed successfully 🎉".
* **Failure**: Prints "Pipeline failed ❌".
   
 ---
 
## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

### How to Contribute

1. **Fork the Project**
Click the "Fork" button at the top right of the repository page to create a copy of the project on your own account.
2. **Clone your Fork**
```bash
git clone https://github.com/ThilinaJayamal/jenkins-ci-cd-demo

```


3. **Create your Feature Branch**
Create a branch for your new feature or bug fix:
```bash
git checkout -b feature/AmazingFeature

```


4. **Commit your Changes**
Write a concise and descriptive commit message:
```bash
git commit -m 'Add some AmazingFeature'

```


5. **Push to the Branch**
Push your changes to your forked repository:
```bash
git push origin feature/AmazingFeature

```


6. **Open a Pull Request**
Navigate back to the original repository and click the "New Pull Request" button. Provide a clear description of the changes you've made.

### Reporting Issues

If you find a bug or have a suggestion for improvement, please open an issue in the [GitHub Issues](https://www.google.com/search?q=https://github.com/ThilinaJayamal/jenkins-ci-cd-demo/issues) section of the repository.

---

## 👤 Author

**Thilina Jayamal** Software Engineering Student at the University of Sri Jayewardenepura.

* **LinkedIn:** [thilina-jayamal](https://www.linkedin.com/in/thilina-jayamal-b70160213)
* **GitHub:** [@ThilinaJayamal](https://github.com/ThilinaJayamal)
* **Email:** thilinajayamal271@gmail.com
