## Hi there 👋
Hair Fit is one of the capstone project that take "Human Healthcare and Living Wellbeings" theme. This application is made for all the people that interested in their hair style. Especially if they are want to know which hair style that fit with their facial shape. 

# Background of This Capstone Project
We began by exploring several ideas then discussing and reviewing the ideas by looking at the available datasets and possible jobs that are feasible to do from each learning path. We decided to bring this idea in our project because some people from our team also feel the same confusion in determining a haircut that suits their face shape and preferences. Some pre-existing applications come with features that help someone to choose their fashion or make-up, but features that provide a haircut option are not yet available. However, in determining a haircut that suits the user, several aspects need to be considered such as face shape, hair type, personal use reasons, and hairstyle preferences. 

# Meet The Capstone Team C23-PS426
- (ML) M340DSY0129 – Arum Putri Kurnia Sari – Universitas Sebelas Maret 
- (ML) M340DSY4971 – Viola Fajrin – Universitas Sebelas Maret 
- (CC) C168DKX4148 – Muhammad Shalbi Addandi – Universitas Esa Unggul 
- (CC) C168DSX1991 – Yohanes Bagas Ari Widatama – Universitas Esa Unggul 
- (MD) A340DSY1128 – Widia Hayati – Universitas Sebelas Maret 
- (MD) A054DSX3367 – Arief Muhammad – Politeknik LP3I 

# Task and Technical Description

## Cloud Computing
From the cloud computing side, we plan to deploy this application on cloud run + cloud SQL (MySQL) + GCS Bucket. 
### Why cloud run?
For model deployment, at first we want to use Tensorflow Js. But we encountered some problems, so we ASAP seperate it from backend service that are use Node Js. We are in conclusion to use FastAPI to deploy Tensorflow model. So the model container is stateless. In the other hand, the backend service is also stateless because eventhough it is serve the authorization, the backend service use token based authentication. We adapt the Oauth2 auth. More information about backend is on the backend service repository.
### Why GCS Bucket
The bucket is has a purpose to serve the static file such as image. It is also good place to store the machine learning mode and donwload it when building the container image. 
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
