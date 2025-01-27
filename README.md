# NoSQL project

## 📖 **Table of Contents**
1. [Descriptions](#descriptions)
2. [Prerequisites](#Prerequisites)
3. [Project structure](#Project-structure)
4. [Installation](#Installation)
5. [Contribution](#Contribution)
6. [Author](#Author)

Contains instructions to install and use `redis`, `mongo` and `OrientDB`, and uses `Jupyter notebook` to interact with the databases in Python or shell.
<h2 id="Descriptions">🧩 Descriptions</h2>
Contains instructions to install and use `redis`, `mongo` and `OrientDB`, and uses `Jupyter notebook` to interact with the databases in Python or shell.






<h2 id="Prerequisites">🤖 Prerequisites</h2>

- Anaconda
- Docker Desktop (make sure to reinstall Docker Desktop so the `docker` command line works)



<h2 id="Project-structure">🏗️ Project structure</h2>





<h2 id="Installation">🛠️ Installation</h2>

### Setup the conda environment

Remember to use the `Anaconda Powershell` prompt at the root of your project.

```
conda create -n nosql python=3.7
conda activate nosql
conda install -c anaconda mongo-tools
pip install jupyter jupyterlab redis pymongo
```

To run your jupyter notebook: `jupyter notebook` or `jupyter lab`

### Run Redis

In a separate command line prompt:

```
docker run -it --rm -n some-redis -p 6379:6379 redis
```

### Run MongoDB

In a separate command line prompt:

```
docker run -it --rm -n some-mongo -p 27017:27017 mongo:4
```

### Run OrientDB

In a separate command line prompt:

```
docker run -it --rm -n some-orientdb -p 2424:2424 -p 2480:2480 -e ORIENTDB_ROOT_PASSWORD=root orientdb:2.2
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
