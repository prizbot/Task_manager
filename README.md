# Task Management Application with Machine Learning

## Project Overview
This is a Python-based task management application that allows users to add, remove, list, and get recommendations for tasks based on their priority levels. The application uses the pandas library to handle data in a DataFrame and employs the scikit-learn library to implement a basic machine learning model for task prioritization.

## Workflow Steps
1. **Imports and DataFrame Initialization:**
   - The code starts by importing necessary libraries including pandas, numpy, and scikit-learn components such as CountVectorizer and MultinomialNB.
   - An empty DataFrame named tasks with columns 'Description' and 'Priority' is initialized to store task details.

2. **CSV Saving Function:**
   - The save_file() function saves the current state of the tasks DataFrame to a CSV file named "tasks.csv". This ensures data persistence.

3. **Machine Learning Model Setup:**
   - A CountVectorizer and a MultinomialNB classifier are instantiated and combined into a pipeline.
   - The model is then trained on the 'Description' and 'Priority' columns of the tasks DataFrame. However, this initial training would fail since the DataFrame is empty.

4. **Task Management Functions:**
   - add_task(description, priority): Adds a new task with the given description and priority to the DataFrame and saves it.
   - remove_task(desc): Removes the task with the specified description from the DataFrame and saves the updated DataFrame.
   - list_task(): Lists all tasks currently in the DataFrame. If no tasks are available, it notifies the user.
   - recommend_task(): Recommends a random high-priority task from the DataFrame. If no high-priority tasks are available, it notifies the user.

5. **User Interaction Loop:**
   - The script contains a while loop that continuously prompts the user with options to manage tasks or exit the application. User inputs are processed accordingly.

6. **Model Prediction:**
   - Towards the end, the code includes an example of how to predict the priority of a new task using the trained model. This showcases how the model can classify new tasks based on their descriptions.

This application is an interactive command-line tool that combines task management with basic machine learning to prioritize tasks. It demonstrates the integration of data manipulation, machine learning, and user interaction in Python. For a fully functional implementation, additional handling for empty DataFrame scenarios and error checks would be necessary.

## Contact

Feel free to reach out if you have any questions or suggestions:

- **LinkedIn**: [Priyadharshini NRS](https://www.linkedin.com/in/priyadharshininrs)
- **Email**: priyadharshininrs@gmail.com
