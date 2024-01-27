<div align="center">
  
[![Twitter Follow](https://img.shields.io/twitter/follow/iamt_toby?style=social)](https://twitter.com/intent/follow?screen_name=iamt_toby)
  <br />
  <br />

  <h2 align="center">PicSureAI - AI image generation App </h2>

  ## Introduction

  AI image generation, an exciting and rapidly evolving field in the realm of artificial intelligence. In recent years, there has been a significant advancement in the capabilities of machine learning algorithms, particularly in the area of generative models. With the development of deep learning techniques, researchers have been able to create powerful AI models that can generate images that are nearly indistinguishable from real images. These AI image generation models have numerous potential applications in various fields, including entertainment, design, and advertising. 

This project was inspired by one of such powerful AI image generation models: `OpenAI's DALL-E`

This is a full-stack web application developed using the MERN stack. The application allows users to create AI-generated images using OpenAI's DALL-E API, based on their input text. The speciality of the developed application is, it offers a modern and minimal design with dynamic layouts, hover effects, and sharing options with the community.

  <a href="https://picsureai.fahiz.in/"><strong>➥ Live Demo</strong></a>

</div>

<br />

### Demo Screeshots

![PicSureAI Desktop Demo](./thumbnail.png "Desktop Demo")

## ❇️ Features added :

* AI image generation using OpenAI API.
* Modern and minimal interface for easy navigation.
* Surprise me! button.
* Search functionality.
* Download generated images to user's device.
* Hover effects that generate user's prompt along with username and download button.
* Share functionality to share the AI generated images with the community on the community section.

## 🧑‍💻 Tech Stack

**Client:** HTML, TailwindCSS, JavaScript, React

**Server:** NodeJS, Express, MongoDB, Cloudinary

**API:** OpenAI's DALL-E

- **MongoDB**: A popular NoSQL database used for storing application data.
- **Express.js**: A web application framework for building robust APIs with Node.js.
- **React**: A JavaScript library for building user interfaces.
- **Node.js**: A JavaScript runtime environment for server-side programming.
- **OpenAI API**: Harness the capabilities of the OpenAI API to generate AI images.
- **Tailwind CSS**: A utility-first CSS framework for creating responsive designs with minimal effort.

## 🧐 How to use

Here is a step-by-step guide on how to use the application:

- Upon visiting the home page, you will see a "Community Showcase" section with a search bar. Use the search bar to find images created by other users by entering keywords or usernames. Hover over any image to view the username, input prompt, and download icon.

- Click on the `Create` button at the top right of the page to go to the "Create" section. Here, you can generate AI-generated images by providing a username and input prompt or by using the `Surprise Me` button to get ideas for image generation.

- After entering the necessary details, click on the `Generate` button. If the generated image is not satisfactory, click on the `Generate` button again until you get a desired image.

- Once you have generated a desirable image, click on the `Share with Community` button to upload and share your custom AI-generated image. You can also download the image to your local machine by clicking on the download icon on the image preview.

- Your custom AI-generated image will now be displayed in the "Community Showcase" section for other users to see and search for.


## 🧐 How it works with the tech stack

The application is built using the MERN stack, which includes MongoDB, Express.js, React, and Node.js. In addition, the OpenAI DALL-E API is used for generating the AI images, and Cloudinary is used to store and showcase the images on the home page.

Here is a high-level overview of how the application works at the backend:

- The user submits a request to generate an AI-generated image, providing a username and input prompt.

- The request is sent to the server, which uses Node.js and Express.js to handle HTTP requests and responses.

- The server makes an API call to the OpenAI DALL-E API, passing the username and input prompt as parameters. The API returns an image that is generated based on the input prompt.

- The server receives the image from the DALL-E API and stores it in a MongoDB database. The image is also uploaded to Cloudinary, a cloud-based image management service, for showcasing on the home page.

- The server sends a response to the client, which includes the generated image and a link to the image on Cloudinary.

- The user can then share their custom AI-generated image with the community by clicking on the "Share with Community" button. This sends a request to the server to add the image to the community showcase section on the home page.

- The server retrieves the image from the MongoDB database and updates the home page with the new image, which is now visible to other users.

In summary, the backend of this web application uses the MERN stack and OpenAI's DALL-E API, along with Cloudinary for storing and showcasing the images on the home page. The server handles user requests, makes API calls to the DALL-E API, stores the generated images in a MongoDB database, and updates the home page with new images shared by users.


## 📖 Lessons Learned

By working on this project, I have learned several valuable lessons which helped me to build a broad range of skills that are useful in a variety of web development projects, including:

- *Full Stack Web Development*

The project involves working on both the front-end and back-end of the application, so that allowed me to gain a better understanding of full-stack web development.

- *MERN Stack*

Developing the application using the MERN stack provided me an opportunity to learn about the different technologies involved, including MongoDB, Express.js, React, and Node.js.

- *Image Processing*

Working on this image generation project somehow it provided me a chance to learn about image processing techniques, including manipulating images based on user input.

- *Sharing System*

By developing a feature that allows users to share their AI generated images with the community has provided me an insight into the importance of social features in web applications.

- *Design and User Experience*

Building a modern and minimalistic design taught me about the importance of design and user experience in web applications and how they impact user engagement.

Overall, this project was a great learning experience that helped me improve my web development skills and gain a better understanding of the technologies involved.

### Contact

If you want to contact with me you can reach me at [LinkedIn](https://www.linkedin.com/in/dee-prince-dede-970913217/).

## Getting Started

### Prerequisites

Before you begin, ensure you have the following prerequisites:

- Node.js and npm: Make sure you have Node.js and npm (Node Package Manager) installed.
- MongoDB: Set up a MongoDB database to store application data.

### Installation

```bash
git clone https://github.com/richdede/picsureai.git
cd picsureai

# Install server dependencies
cd server
npm install

# Install client dependencies
cd ../client
npm install

# Create a .env file in the server directory and add your OpenAI API key
echo "OPENAI_API_KEY=your_openai_api_key_here" > server/.env

# Start the development server for the server
cd ../server
npm start

# In a separate terminal window, start the React development server for the client
cd ../client
npm start
