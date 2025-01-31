# SolarGIS
 Predicting Rooftop solar energy potential using real time solar irradiance data combined with extracted building footprints. Adjusting PV output taking into consideration partial shading originating from surrounding obstacles such as trees, buildings, etc. 

### Project Objectives:
•	Predicting the approximate power output specified number of PV modules can produce when installed on rooftops in given location while also estimating how partial shading can affect the total power generated. 
•	Aiding resource planners, ordinary citizens and startups to accurately predict solar energy outputs in urban settings, thereby aiding in transition to green energy and fulfillment of UN SDGs.
•	Building a deep learning model that can output the average solar energy potential of a day when provided with the area of rooftop, average solar irradiance in the location along with heights of objects obstructing sunlight in the specified area. 

## Running with Docker

You can run this project using Docker. Below are the steps to set up and run the application in a Docker container.

### 1. Build the Docker Image

First, ensure you are in the project directory where your `Dockerfile` is located.

Run the following command to build the Docker image:

```bash
docker build -t solargis .
```
### 2. Run the Docker Container

Once the image is built, you can run the application using the following command:

```bash
docker run -p 8080:8080 solargis
```
This will start a container from the solargis image and map port 8080 inside the container to port 8080 on your local machine.

### 3. Access the Application
After running the container, the application should be accessible at:

```bash
http://localhost:8080
```
### 4. Stopping the Docker Container
To stop the running Docker container, use the following command:

```bash
docker stop <container_id>
```
You can find the container ID by running:

```bash

docker ps
```
This will display the list of running containers. Copy the container_id of the container you want to stop, and use it in the docker stop command.

## How to Run the App
To run the Streamlit app, open the terminal inside the folder and use the following command:

```bash
streamlit run solargis.py
```

### Library installations: 
```bash
pip install -r requirements.txt
```

Check out the open-source dataset: [Open Buildings](https://sites.research.google/open-buildings/)

## Deployment: 

Use Google cloud to deploy the project. Once you have configured google cloud project and sdk in your computer, use this command to deploy.
```bash
gcloud app deploy
```
Deployed version available on streamlit cloud but app doesn't run well due to cloud specifications.  

## Overview 

The details of the project are covered in this video : https://youtu.be/IiyKUs6mKco


## Gallery :
 
![Demo](assets/display.gif)

<br>




