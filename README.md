# llm-insta-content
### Using LLMs to Generate Images and Automate Instagram Accounts Content


#### Overview
The goal of this project was to utilize LLMs and image generation to automate the content for 4 instagram accounts.  


#### Process
 - Each instagram account was given a specific niche to follow.
 - Prompts for each instagram niche were engineered (engineered prompt lists were developed seperatly using LLMs to automatically generate all of them) then feed to OpenAI's 3.5 turbo API to extrapolate and convert into image generation prompts and also instagram captions.
 - The output image generation prompts were feed then to Dalle-3 to get a single image.
 - The image url output from Dalle-3 was used to store the images into an AWS S3 bucket to help streamline the upload to Instagram via the Instagram Graph API.
 - Once the images are stored in S3 buckets and the captions have been generated, the Instagram Graph API is used to upload all the content to each instagram account.
 - This entire processes is automated to run daily through having the code scheduled on https://www.pythonanywhere.com/ tasks.



#### Contact Me
 - If you would like to learn more about this project, please email me at acarterdata@outlook.com.
