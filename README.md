# MLOps-End2End
End to End Machine Learning Project.

1. Data Ingestion
2. Data Transformation
3. Model Trainer
4. Model Evaluation
5. Model Deployment

## CI/CD Pipeline
- GitHub Actions

## Deployment
- AWS

## Actions:
## 1. Set up the environment locally:
```sh
cd your-project-folder
conda create -p venv python=3.8 -y  # You can also use python=3.8 to find the latest 3.8.x version available.
conda activate ./venv
```

### 1.a. Create a new repository on the command line:
```sh
git init
git add README.md
git commit -m "First Commit"
git branch -M main
git remote add origin https://github.com/gaganjotshan/MLOps-End2End.git
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git push -u origin main
```

### 1.b. setup.py
setup.py is a Python script traditionally used for configuring the packaging and distribution of Python projects. It is an essential file for any Python project that you want to distribute, either as a source distribution or as a precompiled wheel. The setup.py script contains metadata about the project, such as its name, version, author, license, and dependencies.

- **Purpose**: Primarily used for packaging and distributing your project. It defines the metadata about the project and its dependencies.
- **Typical Usage**: When you want to distribute your project (e.g., upload it to PyPI), other users or automated systems can install it using `pip install your_project`.

### 1.c. requirements.txt
The requirements.txt file lists the project dependencies.
On adding the requirements in the file,
```sh 
pip install -r requirements.txt  
```
will install all the mentioned requirements from the file.

- **Purpose**: Lists the exact versions of dependencies needed to run your project. It’s commonly used to recreate the exact environment in which your project runs.
- **Typical Usage**: When setting up the development environment or deploying the project, you use `pip install -r requirements.txt` to install all the required dependencies.


#### How to Link setup.py and requirements.txt
You can ensure that the dependencies listed in `requirements.txt` are also included in `setup.py` by reading the contents of `requirements.txt` within `setup.py`. This way, you maintain a single source of truth for your dependencies.


## 2. Scr folder and build up the packages
Organize your code into a src folder to keep the project structure clean and maintainable. The src folder will contain all the modules and packages necessary for your project.
