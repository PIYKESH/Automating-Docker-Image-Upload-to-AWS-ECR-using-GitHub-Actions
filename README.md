# Creating a simple web app in Python can be done using a web framework. As Flask is a popular choice for building web applications in Python due to its simplicity and ease of use.
# Firstly created a file named app.py.
# Then created a folder named templates in the same directory as app.py, and inside it, create a file named index.html .
# Simple web app defines a route ("/") that renders an HTML template with a message. When you run the app by running python app.py .
# Visit to check http://127.0.0.1:5000/ in your web browser, and you should see your simple web app displaying the message "Hello! .
# To containerize your Python web app using Docker, you'll need to create a Dockerfile. Make sure your app.py and any other necessary files are in the same directory as the Dockerfile.
# Create a file named Dockerfile and save it without checking the append extension as it would not build you image later.
# Make sure to update the dependencies according to your actual requirements. 
# Use this command to build the image 'docker build -t web-app .' ,Here web-app is the image name which I have given in yyour case you can give any.
# After building the image, you can run your container by ruuning this 'docker run -p 5000:5000 web-app' .
# Create a private repo using AWS-ECR service under the AWS Account, If you don't have create on as we need it later to setup the github actions which is technically CI/CD.
# So after setting up your repo under AWS Account as a private one with required permission we are good to go.
Then only part which is left is writing down the yaml file to perform the Github Action, As we'll create workflow that triggers on push or pull request events which include steps to build the Docker image and push it to AWS ECR making it to optimize the workflow runs.


