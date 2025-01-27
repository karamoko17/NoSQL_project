# NoSQL project

## 📖 **Table of Contents**
1. [Descriptions](#descriptions)
2. [Prerequisites](#Prerequisites)
3. [Project structure](#Project-structure)
4. [Installation](#Installation)
5. [Contribution](#Contribution)
6. [Author](#Author)


<h2 id="Descriptions">🧩 Descriptions</h2>

This repository offers comprehensive tutorials for working with NoSQL databases: Redis, MongoDB, and OrientDB. It includes step-by-step instructions for installing and configuring these databases, as well as hands-on examples of interacting with them using Python or shell commands through Jupyter Notebooks.

Contents
- Redis: Installation and usage guidelines.
- MongoDB: Essential commands and data manipulation techniques.
- OrientDB: Introduction and configuration setup.

These tutorials are perfect for anyone looking to explore NoSQL databases in an interactive and practical way, providing clear examples and guidance for real-world applications.

<h2 id="Prerequisites">🤖 Prerequisites</h2>

- Anaconda
- Docker Desktop (make sure to reinstall Docker Desktop so the `docker` command line works)


<h2 id="Project-structure">🏗️ Project structure</h2>

```
├── data/
│   ├── movieslens_movies.json
│   └── movieslens_users.json
├── lecture/
│   └── nosql_lecture.pdf
├── notebooks/
│   ├── 1-redis.ipynb
│   ├── 2-mongo.ipynb
│   └── 3-orientdb.ipynb
├── .gitignore
└── README.md
```

<h2 id="Installation">🛠️ Installation</h2>

GitHub repository

Run the following command in your terminal to clone the GitHub repository:
```bash
https://github.com/karamoko17/NoSQL_project.git
```

Then move to the project directory and create a new conda environment with the following command :

1. Open the Anaconda Powershell prompt at the root of your project.
2. Create and activate a Conda environment:
```
conda create -n nosql python=3.7  
conda activate nosql  
```

3. Installez les outils nécessaires :
```
conda install -c anaconda mongo-tools  
pip install jupyter jupyterlab redis pymongo  
```

4. Lancez votre Jupyter Notebook ou Jupyter Lab:
```
jupyter notebook  
# ou  
jupyter lab  
```

You can also use Visual Studio Code !

## Run the databases
### Run Redis

In a separate command line prompt:

```
docker run -it --rm --name some-redis -p 6379:6379 redis
```

### Run MongoDB

In a separate command line prompt:

```
docker run -it --rm --name some-mongo -p 27017:27017 mongo:4
```

### Run OrientDB

In a separate command line prompt:

```
docker run -it --rm --name some-orientdb -p 2424:2424 -p 2480:2480 -e ORIENTDB_ROOT_PASSWORD=root orientdb:2.2
```

<h2 id="Contribution">🤝 Contribution</h2>

Contributions are welcome! Feel free to open a ticket or submit a pull request to suggest improvements. Here's how you can get involved:

1. Fork the project.
2. Create a branch for your feature.
3. Make your changes and validate them with a clear message.
4. Push your changes to your branch on the remote repository.  
5. Submit a pull request to have your contribution reviewed.

<h2 id="Author">🎯 Author</h2> 
This project was designed and developed by KARAMOKO Awa, a student in Master 2 SISE (Statistics and Computer Science for Data Science) at Université Lumière Lyon 2.
