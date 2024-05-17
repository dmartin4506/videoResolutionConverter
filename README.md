
# Video Resolution Converter Tool

This project leverages the ffmpeg tool and Thunder Client Rest API Client for local video resolution conversion. Simply drag in your desired video file into the main video-processing-service directory, run the application and make a Thunder Client Post request.
More details can be found below for steps. 



## How It's Made:

**Tech used:** Video File Resolution Converter TechStack: TypeScript, Next.js, Express.js, and FFmpeg

The tool was built from Express TypeScript Boilerplate and leverages the Thunder Client Rest API extension within VS Code. 

## To deploy the solution on your own:
 - Clone the Repository to VS Code
 - CD into the video-processing-service directory 
 - You may need to install the below dependencies:
    npm install express
    npm install --save-dev typescript ts-node

    npm install --save-dev @types/node @types/express

    npm install fluent-ffmpeg
    npm install --save-dev @types/fluent-ffmpeg

    You should also have the following downloaded and installed:

    - ffmpeg
    - Node.js and NPM

## To start it up locally:
run npm run start

Within Thunder Client in VS Code:

You will need to create a POST Request with the following JSON Request body:

{
  "inputFilePath": "./yourVideoFileGoesHere.mp4",
  "outputFilePath": "./processed-yourVideoFileGoesHere.mp4"
}

After sending the POST request, the file should be converted and downloaded with the new resolution. 

