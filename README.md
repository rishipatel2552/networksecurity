<p align="center">
    <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" align="center" width="30%">
</p>
<p align="center"><h1 align="center">NETWORKSECURITY</h1></p>
<p align="center">
	<em>Securing Networks, Enhancing Safety with Smart Data Science</em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/license/rishipatel2552/networksecurity?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/rishipatel2552/networksecurity?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/rishipatel2552/networksecurity?style=default&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/rishipatel2552/networksecurity?style=default&color=0080ff" alt="repo-language-count">
</p>
<p align="center"><!-- default option, no dependency badges. -->
</p>
<p align="center">
	<!-- default option, no dependency badges. -->
</p>
<br>

##  Table of Contents

- [ Overview](#-overview)
- [ Features](#-features)
- [ Project Structure](#-project-structure)
  - [ Project Index](#-project-index)
- [ Getting Started](#-getting-started)
  - [ Prerequisites](#-prerequisites)
  - [ Installation](#-installation)


---

##  Overview

The NetworkSecurity project is a cutting-edge solution designed to enhance cybersecurity through machine learning. By automating data ingestion, validation, transformation, and model training, this platform ensures robust network protection. Ideal for IT security teams, it offers tools for efficient threat detection and response, backed by consistent, reproducible workflows.

---

##  Features

|      | Feature         | Summary       |
| :--- | :---:           | :---          |
| ⚙️  | **Architecture**  | <ul><li>Utilizes a multi-component structure with separate modules for data ingestion, transformation, validation, and training.</li><li>Employs a containerized approach using `<Docker>` for consistent deployment environments.</li><li>Integrates with MongoDB for data management, enhancing the project's scalability and performance.</li></ul> |
| 🔩 | **Code Quality**  | <ul><li>Adheres to Python best practices with modular code in components like `networksecurity/components/model_trainer.py`.</li><li>Includes robust exception handling mechanisms in `networksecurity/exception/exception.py`.</li><li>Utilizes configuration management with `<python-dotenv>` for environment variables.</li></ul> |
| 📄 | **Documentation** | <ul><li>Documentation includes detailed setup and usage instructions using `<pip>` and `<Docker>`.</li><li>Code comments and structured logging in `networksecurity/logging/logger.py` aid in maintainability.</li><li>Utilizes `<GitHub Actions>` for automated documentation processes in `.github/workflows/main.yml`.</li></ul> |
| 🔌 | **Integrations**  | <ul><li>Integrates with `<MongoDB>` for data storage and management.</li><li>Uses `<MLflow>` for model tracking and logging performance metrics.</li><li>Automated CI/CD pipeline setup with `<GitHub Actions>` in `.github/workflows/main.yml`.</li></ul> |
| 🧩 | **Modularity**    | <ul><li>Highly modular design with separate directories for different stages of the ML pipeline.</li><li>Components like `networksecurity/components/data_ingestion.py` and `networksecurity/components/data_transformation.py` enhance code reusability.</li><li>Clear separation of concerns across utility functions and model management.</li></ul> |
| 🧪 | **Testing**       | <ul><li>Includes unit tests and integration tests, e.g., database connectivity tests in `test_mongodb.py`.</li><li>Utilizes `<pytest>` for running tests as specified in the test commands.</li><li>Automated testing integrated into the CI/CD workflow with `<GitHub Actions>`.</li></ul> |
| ⚡️  | **Performance**   | <ul><li>Leverages efficient data processing libraries like `<numpy>` and `<pandas>`.</li><li>Optimized model training using `<scikit-learn>` and custom metrics in `networksecurity/utils/ml_utils/metric/classification_metric.py`.</li><li>Performance logging and monitoring integrated using `<MLflow>`.</li></ul> |
| 🛡️ | **Security**      | <ul><li>Focuses on network security model training to detect and respond to threats.</li><li>Secure handling of environment variables and configurations using `<python-dotenv>`.</li><li>Data validation and schema management ensure data integrity and security.</li></ul> |

---

##  Project Structure

```sh
└── networksecurity/
    ├── .github
    │   └── workflows
    ├── Dockerfile
    ├── Network_Data
    │   └── phisingData.csv
    ├── README.md
    ├── data_schema
    │   └── schema.yaml
    ├── final_model
    │   └── preprocessor.pkl
    ├── main.py
    ├── networksecurity
    │   ├── __init__.py
    │   ├── __pycache__
    │   ├── cloud
    │   ├── components
    │   ├── constant
    │   ├── entity
    │   ├── exception
    │   ├── logging
    │   ├── pipeline
    │   └── utils
    ├── push_data.py
    ├── requirements.txt
    ├── setup.py
    └── test_mongodb.py
```


###  Project Index
<details open>
	<summary><b><code>NETWORKSECURITY/</code></b></summary>
	<details> <!-- __root__ Submodule -->
		<summary><b>__root__</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/test_mongodb.py'>test_mongodb.py</a></b></td>
				<td>- Establishes a connection to a MongoDB database using environment-specific configurations to verify connectivity<br>- By pinging the MongoDB server, it confirms the operational status and readiness of the database within the project's architecture, ensuring that the database interactions are set up correctly and are functional.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/main.py'>main.py</a></b></td>
				<td>- Main.py orchestrates the training pipeline for a network security model by managing processes across data ingestion, validation, transformation, and model training<br>- It configures each stage, logs progress, and handles exceptions, ensuring the model is trained with validated and transformed data to enhance network security effectively.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/requirements.txt'>requirements.txt</a></b></td>
				<td>- Requirements.txt specifies the necessary Python libraries for the project, ensuring consistent environments across different setups<br>- It includes libraries for data manipulation (pandas, numpy), database interaction (pymongo, certifi), machine learning (scikit-learn), serialization (dill), configuration management (python-dotenv, pyaml), and model tracking (mlflow), facilitating a robust, scalable, and reproducible data science workflow.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/setup.py'>setup.py</a></b></td>
				<td>- Setup.py serves as the configuration backbone for the NetworkSecurity project, orchestrating the package setup process<br>- It dynamically gathers and specifies dependencies from a requirements.txt file, ensuring the project's environment is correctly established with necessary libraries<br>- Additionally, it defines the project’s metadata including version, author details, and package information.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/Dockerfile'>Dockerfile</a></b></td>
				<td>- Serves as the blueprint for building the project's Docker container, specifying the environment, dependencies, and instructions necessary for running the application<br>- It ensures consistent deployment across different environments, facilitating development, testing, and production workflows within the codebase architecture.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/push_data.py'>push_data.py</a></b></td>
				<td>- Push_data.py serves as a data integration tool within the project, converting CSV data into JSON format and inserting it into a MongoDB database<br>- It utilizes environmental variables for secure database connections and handles exceptions through custom error management, enhancing the robustness of the network security data management process.</td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- networksecurity Submodule -->
		<summary><b>networksecurity</b></summary>
		<blockquote>
			<details>
				<summary><b>components</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/components/data_ingestion.py'>data_ingestion.py</a></b></td>
						<td>- DataIngestion in the networksecurity project manages the extraction of data from MongoDB, processes it for machine learning readiness, and splits it into training and testing datasets<br>- It ensures data is stored correctly in a feature store and handles the initial steps of data preparation for model training.</td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/components/data_transformation.py'>data_transformation.py</a></b></td>
						<td>- DataTransformation in the networksecurity project manages the preprocessing of training and testing datasets for a machine learning model<br>- It utilizes a KNNImputer for handling missing values and saves the transformed data along with the preprocessing object, facilitating reproducibility and consistency in data handling across model training and evaluation phases.</td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/components/model_trainer.py'>model_trainer.py</a></b></td>
						<td>- ModelTrainer in `networksecurity/components/model_trainer.py` orchestrates the training of various machine learning models for network security, evaluates their performance, and logs the best model using MLflow<br>- It leverages preprocessed data, optimizes model parameters, and saves the trained model for future predictions.</td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/components/data_validation.py'>data_validation.py</a></b></td>
						<td>- DataValidation in the networksecurity project ensures data integrity by validating column counts and detecting dataset drift between training and testing datasets<br>- It leverages statistical tests to confirm data consistency, outputs validation reports, and prepares datasets for subsequent training stages.</td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>entity</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/entity/artifact_entity.py'>artifact_entity.py</a></b></td>
						<td>- Defines data structures essential for managing artifacts across various stages of the machine learning pipeline in the network security project<br>- These include structures for data ingestion, validation, transformation, and model training metrics, facilitating organized data handling and ensuring integrity throughout the model development process.</td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/entity/config_entity.py'>config_entity.py</a></b></td>
						<td>- Defines configuration classes for various stages of a network security training pipeline, including data ingestion, validation, transformation, and model training<br>- Each class initializes directories and file paths based on a timestamped artifact directory, ensuring organized storage and retrieval of training artifacts and models.</td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>utils</b></summary>
				<blockquote>
					<details>
						<summary><b>main_utils</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/utils/main_utils/utils.py'>utils.py</a></b></td>
								<td>- Manages data interactions and model evaluations within the network security project by reading, writing, and manipulating YAML and binary files<br>- It includes functions for saving and loading numpy arrays and serialized objects, and for optimizing and assessing machine learning models using grid search and R2 scoring metrics.</td>
							</tr>
							</table>
						</blockquote>
					</details>
					<details>
						<summary><b>ml_utils</b></summary>
						<blockquote>
							<details>
								<summary><b>model</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/utils/ml_utils/model/estimator.py'>estimator.py</a></b></td>
										<td>- NetworkModel, located within the networksecurity/utils/ml_utils/model/ directory, encapsulates the functionality for making predictions using a pre-trained model and a preprocessing step<br>- It handles exceptions specifically tailored to network security applications, ensuring robust error management and logging throughout the prediction process.</td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>metric</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/utils/ml_utils/metric/classification_metric.py'>classification_metric.py</a></b></td>
										<td>- Calculates and encapsulates classification metrics for model evaluation within the network security project<br>- Specifically, it computes the F1 score, precision, and recall of predictions against true values, returning these metrics as a structured artifact<br>- This functionality aids in assessing the performance of machine learning models used for security threat detection and response.</td>
									</tr>
									</table>
								</blockquote>
							</details>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>logging</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/logging/logger.py'>logger.py</a></b></td>
						<td>- Establishes a logging system for the Network Security project, creating a unique log file for each session based on the current date and time<br>- It configures the logging format and sets the logging level to INFO, ensuring all relevant events are recorded systematically in a dedicated directory within the project structure.</td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>exception</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/networksecurity/exception/exception.py'>exception.py</a></b></td>
						<td>- Defines a custom exception class, NetworkSecurityException, within the network security module to enhance error handling by capturing and formatting detailed error information, including the file name and line number where exceptions occur<br>- This class leverages the project's logging system to facilitate debugging and maintenance of the network security functionalities.</td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- .github Submodule -->
		<summary><b>.github</b></summary>
		<blockquote>
			<details>
				<summary><b>workflows</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/.github/workflows/main.yml'>main.yml</a></b></td>
						<td>- Manages the automated processes for the project by defining a GitHub Actions workflow in `.github/workflows/main.yml`<br>- This setup automates testing, building, and deploying the application, ensuring consistent execution and deployment practices across development environments<br>- It plays a crucial role in maintaining the operational integrity and efficiency of the software development lifecycle.</td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- data_schema Submodule -->
		<summary><b>data_schema</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/rishipatel2552/networksecurity/blob/master/data_schema/schema.yaml'>schema.yaml</a></b></td>
				<td>- Defines the data schema for a machine learning model by specifying the structure and data types of various features related to web security, such as IP addresses, URL characteristics, and SSL certificates<br>- This schema supports the model's ability to analyze and predict web-based threats effectively, ensuring robust data integrity and consistency across the system.</td>
			</tr>
			</table>
		</blockquote>
	</details>
</details>

---
##  Getting Started

###  Prerequisites

Before getting started with networksecurity, ensure your runtime environment meets the following requirements:

- **Programming Language:** Python
- **Package Manager:** Pip
- **Container Runtime:** Docker


###  Installation

Install networksecurity using one of the following methods:

**Build from source:**

1. Clone the networksecurity repository:
```sh
❯ git clone https://github.com/rishipatel2552/networksecurity
```

2. Navigate to the project directory:
```sh
❯ cd networksecurity
```

3. Install the project dependencies:


**Using `pip`** &nbsp; [<img align="center" src="https://img.shields.io/badge/Pip-3776AB.svg?style={badge_style}&logo=pypi&logoColor=white" />](https://pypi.org/project/pip/)

```sh
❯ pip install -r requirements.txt
```



