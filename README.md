### A ELCTRONICS PRODUCT RECOMMANDATION SYSTEM

### dataset
Explaining the Dataset:
The dataset is a collection of product listings from various e-commerce websites. It includes information such as product names, brands, categories, prices, availability, condition, merchant information, and other related details.

The dataset is typically in the form of a table or a CSV file, with each row representing a unique product listing and each column containing specific attributes of the listing. you will get the dataset from the above link.

Dataset: https://www.kaggle.com/datasets/datafiniti/electronic-products-prices

### INTRODUCTION
E-commerce websites offer a wide range of products to customers, making it challenging for them to find what they are looking for. In this case, recommendation systems can come in handy to help customers discover relevant products. A recommendation system is a subset of machine learning, which predicts the user’s preferences based on their past behaviors, and recommends items that the user is likely to be interested in. In this blog, we will build an Electronics Recommendation System using Machine Learning and Flask.

### MODEL BUILDING
The next step is to build our machine learning model. We use the cosine similarity measure to find similar products based on their descriptions. The cosine similarity measure calculates the cosine of the angle between two vectors, and ranges from -1 to 1. A score of 1 means that the two vectors are identical, while a score of -1 means that they are completely dissimilar.

Flask App: After building the model, we will create a Flask app to make it accessible to users. Flask is a web framework that allows us to build web applications in Python. We create an HTML form where users can enter the name of a product, and our app will recommend similar products based on their input.

### CREATING FLASK APP (STEPS)

Install Flask: The first step is to install Flask. We can do this using pip, which is a package manager for Python.
Create the Flask App: We create a new file called app.py and import the Flask module. We then create a Flask instance called app.
Create the HTML Form: Next, we create an HTML form where users can enter the name of a product. We create a new file called index.html, and add the form to it.
Create the Recommendation Function: We create a function called get_recommendations that takes in the name of a product as input, and returns the top 20 most similar products. This function uses the machine learning model we built earlier to find similar products.
Create the Flask Route: We create a Flask route that listens for requests to the /predict URL. When a request is received, we get the name of the product from the HTML form, and call the get_recommendations function. We then render the results on a new HTML page called results.html.
Run the Flask App: Finally, we run the Flask app using the command python app.py. We can then access the app by visiting http://localhost:5000 in our web browser.


### conclusion

 In this project, we have discussed how to build an Electronics Recommendation System using Machine Learning and Flask. We have explained the dataset, data cleaning, model building, and the steps involved in building a Flask app. With this recommendation system, customers can discover relevant products based on their preferences, making it easier for them to find what they are looking for.