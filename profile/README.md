# Fishrs 🎣🦀🧠

Fishrs answers the age old question: "How can you get a Rust developer to go outside?"

Fishrs is an embedded machine learning project utilizing the [Unda](https://github.com/unda-ml/unda) crate to make intelligent inferences for a fishing robot. In other words, it's the only way I ever would go fishing. The primary goal of Fishrs is to predict the type of fish hooked on the line and determine the optimal moment to automate the reeling process. This prediction is based on a combination of key input data points, including:

- **Longitude**: The geographic coordinate that specifies the east-west position. 🗺️
- **Latitude**: The geographic coordinate that specifies the north-south position. 🧭
- **Water Depth**: The depth of water where the fishing activity is taking place. This is collected using a special .json file specifying depths of Lake Waubesa and is created as a lon-lat hashmap. 📏
- **Pull Strain**: The strain or tension on the fishing pole caused by the fish. 🏋️

By leveraging these data points, Fishrs takes away the entire point of fishing and allows you to do the exact same thing you'd be doing anyway, sit and do nothing. 

Or better yet, now that you don't need to facilitate this fishing pole, you can cast another fishing rod!

## Key Features

- **Machine Learning Inferences**: Utilizes the Unda machine learning crate to analyze and interpret real-time data from the fishing environment.
- **Fish Type Prediction**: Accurately predicts the type of fish based on input data, helping fishers identify their catch even before it is reeled in.
- **Automated Reeling Process**: Determines the optimal time to start the automated reeling process, ensuring that the fish is caught with minimal effort and maximum efficiency.

## How It Works

Fishrs employs a combination of machine learning algorithms and real-time data analysis to make its predictions. Here's a high-level overview of the process:

1. **Data Collection**: The fishing robot collects data on longitude, latitude, water depth, and pull strain.
2. **Data Processing**: The collected data is processed and fed into the Unda machine learning model.
3. **Inference Making**: The model analyzes the data to predict the type of fish and the optimal time to automate the reeling process.
4. **Action Execution**: Based on the predictions, the robot initiates the appropriate actions, such as starting the reeling process.

## Future Enhancements

- **Expanded Data Inputs**: Incorporating additional data points such as water temperature, time of day, and weather conditions to improve prediction accuracy.
- **Enhanced Model**: Currently the model is planned to just be a simple Dense neural network. I believe that we could potentially use a Transformer network instead to work with series of previous fishing data.
