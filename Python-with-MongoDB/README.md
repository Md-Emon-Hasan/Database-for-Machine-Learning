# Python with MongoDB

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![MongoDB](https://img.shields.io/badge/Database-MongoDB-47A248?logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![PyMongo](https://img.shields.io/badge/Driver-PyMongo-13AA52)](https://pymongo.readthedocs.io/)
[![Jupyter](https://img.shields.io/badge/Notebooks-Jupyter-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](../LICENSE)

Practical Jupyter Notebook examples for connecting Python to MongoDB and working with document data using [PyMongo](https://pymongo.readthedocs.io/). These notebooks progress from a basic connection to queries, updates, and aggregation.

## Contents

| Notebook | What you will learn |
| --- | --- |
| [Connect Python With MongoDB](1%20Connect%20Python%20With%20MongoDb/Connect%20Python%20With%20MongoDb.ipynb) | Connect with `MongoClient`, select a database and collection, and insert documents. |
| [Querying JSON Documents](2%20MongoDb%20With%20Python-%20Querying%20Json%20Documents/MongoDb%20With%20Python-%20Querying%20Json%20Documents.ipynb) | Read documents and filter with equality, comparison, `$in`, `$and`, and `$or` queries. |
| [Updating Records](3%20MongoDb%20With%20Python-%20Updating%20Records/MongoDb%20With%20Python-%20Updating%20Records.ipynb) | Practice `update_one`, `update_many`, and `replace_one`. |
| [Aggregate Functions](4%20MongoDb%20With%20Python-%20Aggregate%20Functions/MongoDb%20With%20Python-%20Aggregate%20Functions.ipynb) | Group documents and calculate counts, sums, averages, and projected fields. |

## Requirements

- Python 3.9 or newer
- A MongoDB deployment: a local server or a MongoDB Atlas cluster
- Jupyter Notebook or JupyterLab

Install the notebook dependencies:

```bash
python -m pip install pymongo notebook
```

## Run the notebooks

1. Clone the repository and enter this module:

   ```bash
   git clone https://github.com/Md-Emon-Hasan/Database-for-Machine-Learning.git
   cd Database-for-Machine-Learning/Python-with-MongoDB
   ```

2. Start your local MongoDB server, or prepare a MongoDB Atlas connection string.
3. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

4. Open a notebook from the contents table and run its cells in order.

## Configure the MongoDB connection

The examples connect to MongoDB on the local machine:

```python
from pymongo import MongoClient

client = MongoClient("mongodb://127.0.0.1:27017/")
```

For Atlas or another deployment, use that deployment's connection string. Keep credentials out of notebooks committed to GitHub; load secrets from environment variables instead. Use a development database while experimenting because notebook cells insert and modify sample records.

## Notes

- These are independent educational notebooks, not a packaged application.
- Re-running insert cells may add duplicate sample documents.
- Database and collection names are selected in notebook code and can be changed as needed.

## Contributing

Suggestions, fixes, and additional examples are welcome. Open an issue to discuss a change, or submit a pull request with a clear description.

## License

Distributed under the [Apache License 2.0](../LICENSE).

## Connect with me

- 🌐 **Portfolio:** [emonlabs-ai.hitechparks.com](https://emonlabs-ai.hitechparks.com)
- 💻 **GitHub:** [Md-Emon-Hasan](https://github.com/Md-Emon-Hasan)
- 💼 **LinkedIn:** [Md Emon Hasan](https://www.linkedin.com/in/md-emon-hasan-695483237/)
- 🤗 **Hugging Face:** [emonHasan01](https://huggingface.co/emonHasan01)
- 📧 **Email:** [emon.mlengineer@gmail.com](mailto:emon.mlengineer@gmail.com)
- 📱 **WhatsApp:** [+8801834363533](https://wa.me/8801834363533)
