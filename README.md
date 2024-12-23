# 🌟 LlamaIndex Query Engine 🌟

Welcome to the **LlamaIndex Query Engine** project! 🚀  
This project demonstrates how to create and interact with a **query engine** using `LlamaIndex`. It builds an index from documents stored in a specified directory and allows you to query the indexed data. If the index already exists, it loads the index from persistent storage, ensuring fast and efficient retrieval.

---

## 🚀 Features

- 📄 **Document Indexing**: Loads documents from a specified directory and creates an index.
- 💾 **Persistent Storage**: Saves the index to disk for later use, avoiding unnecessary re-building.
- 🔍 **Query Engine**: After building or loading the index, you can perform queries with natural language.
- 🔧 **Customizable**: Easily adapt the project for different datasets and query requirements.

---

## 📋 Requirements

Before you get started, make sure you have the following:

- 🐍 **Python 3.x**: Make sure you have Python 3 installed.
- 🍃 **Conda**: We use Conda environments to manage dependencies.
- 📦 **`llama_index`**: This package is used for indexing and querying data.

---

## ⚙️ Setup

### 1. Clone the repository

Start by cloning the project to your local machine:

```bash
git clone https://github.com/your-username/llamaindex-project.git
cd llamaindex-project
```

### 2. Create a Conda environment

To create a Conda environment and install the necessary dependencies, run:

```bash
conda env create -f environment.yml
```

This will create a new environment with all the required packages, including `llama_index`.

### 3. Activate the Conda environment

Once the environment is created, activate it using:

```bash
conda activate llamaindex-env
```

### 4. Install additional dependencies (if any)

If there are any extra dependencies, you can install them using:

```bash
pip install -r requirements.txt
```

This will install any missing packages that are required.

---

## 🏃‍♂️ Usage

### 1. Prepare your data

Place your documents in the `data` folder. The `SimpleDirectoryReader` will automatically load all documents from this directory to build the index.

### 2. Running the script

Once your data is prepared, run the script to either **create** or **load** the index, and then **perform a query**.

```bash
python main.py
```

### 3. Code Breakdown


- **Storage Check**: First, the script checks if the index already exists in the `./storage` directory.
- **Create or Load Index**: If the index doesn't exist, it loads documents from the `data` folder and creates a new index. If the index exists, it loads it from storage.
- **Querying**: Once the index is created or loaded, you can perform queries like `"list some essentials topics we learn?"`.

---

## 📂 Directory Structure

Here’s an overview of the project structure:

```
/llamaindex-project
│
├── /data                 # Folder for storing your documents to index
├── /storage              # Directory for storing the index
├── main.py               # Main Python script for indexing and querying
├── environment.yml       # Conda environment configuration
├── requirements.txt      # List of additional Python dependencies
└── README.md             # This file
```

---

## ❓ Troubleshooting

- **API Key Issues**: If you encounter issues with API keys (e.g., for OpenAI), ensure that your keys are correctly set in the `.env` file or environment variables.
- **Missing Dependencies**: Make sure the Conda environment is activated and all required dependencies are installed.

---

## 📝 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

---

## 🤝 Contributing

We welcome contributions! Feel free to fork the repository, make changes, and open pull requests. If you have suggestions or encounter issues, please open an issue in the repository.
