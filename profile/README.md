<h2 align="center">Bangkit Capstone Project 2022</h2>
<br />
<div align="center">
<img src="https://avatars.githubusercontent.com/u/105267397?s=400&u=3c4165b1956698e8df8e07b62d72ba4c3803d3f2&v=4" />
</div>
<br />
<h1 align="center">Hi, we are C22-PS080</h1>

<br />

## **Profiles**

We are a team of 6 consist of 2 CC Learning Path Students, 2 ML Learning Path Students, and 2 MD Learning Path Students.
<br/>

### Members

| Learning Path      | Name                           | Student ID     | University                          | Contacts                                                                                                                           |
| ------------------ | ------------------------------ | -------------- | ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Cloud Computing    | Ardinata Hari Saputra          | **C2009G0955** | Universitas Gunadarma               | [LinkedIn](https://www.linkedin.com/in/ardinata-hari-saputra-5a7a17112/) <br /> [Github](https://github.com/Ardinatahs)                                                                        |
| Cloud Computing    | Muhammad Rayhan Hamada Budiman | **C2009G0981** | Universitas Gunadarma               | [LinkedIn](https://www.linkedin.com/in/muhammad-rayhan-hamada-budiman-033021194/) <br /> [Github](https://github.com/RayhanHamada) |
| Machine Learning   | Amar Rahman Kamal              | **M2004F0189** | Institut Teknologi Sepuluh November | [LinkedIn](https://www.linkedin.com/in/amarrahman/) <br /> [Github](https://github.com/Chagiyaa)                                                                          |
| Machine Learning   | Rizkyka Mediano Sandie         | **M7009G0995** | Universitas Gunadarma               | [LinkedIn](https://www.linkedin.com/in/rizkyka-mediano-sandie-b93729199/) <br /> [Github](https://github.com/medianosandie)                                                                     |
| Mobile Development | Ahmad Budi Gustama             | **A7211G1943** | Universitas Indraprasta             | [LinkedIn]() <br /> [Github](https://github.com/abgits)                                                                            |
| Mobile Development | Nabilah Putri Cantika          | **A7211F1961** | Universitas Indraprasta             | [LinkedIn](https://www.linkedin.com/in/nabilah-putri-cantika-3524521b4/) <br /> [Github](https://github.com/nabilapisi)                                                                        |

### Project Title:

**Skin Disease Detection Using Image Classification Based on Android “SSkin”**

### Proposal Link

> [click here](https://docs.google.com/document/d/1HenIqoP5-g7DLbogeNNVU4GM7mitQjOYjeaPgTbd3UI/edit?usp=sharing)

### Features

There are 3 main features we're planning for the app,

- **Authentication (Sign up and login)**
  <br />
  Where user candidate can sign up, or for existing user to login and starts using the app.
- **Skin disease image prediction**
  <br />
  Where user can take a picture of a region of their skin that is suspected to have some skin conditions.
- **Showing user's skin disease detection history**
  <br />
  Where user can see list of their skin disease diagnoses, that consist of predicted condition, photo of their region of skin, overview of the predicted condition and if exists, the first-aid solution to the condition, like treatment methods, or even if possible, medicines recommendations.

### Plan

#### Cloud Infrastructure

<img src="https://raw.githubusercontent.com/Capstone-2022-C22-PS080/.github/main/GCP_Infrastructure_Diagram.svg" />

#### Explanation

- For authentication we will use Firebase Authentication, allowing user to sign up either with email and password, or just simply OAuth button tap.
- For serving user-related data such as user profile and diagnostic histories.
- Most prediction stuffs are mainly handled by Google App Engine that act as a REST API server that serves prediction from Vertex AI's model endpoint. After getting prediction result from Vertex AI's model endpoint, based from the result, GAE will fetch diagnosed skin disease's data from PostgreSQL instance (Compute Engine) that act as database instance. Before responding to the mobile client, GAE will also store request payload photos of user's skin region to Cloud Storage.

## Documentation

### Presentation

[Click Here](https://bit.ly/3MZCqzG)

### Logo

<img src="https://raw.githubusercontent.com/Capstone-2022-C22-PS080/.github/main/sskin_logo.png" height="150" />
<br />
No Background
<br />
<img src="https://raw.githubusercontent.com/Capstone-2022-C22-PS080/.github/main/sskin_logo_nobg.png" height="150" />

### Figma

- [Prototype](https://bit.ly/3lXmPF2)
- [Screens](https://bit.ly/3wZdCT2)

### Github

- Main Repositories

  - [REST API](https://github.com/Capstone-2022-C22-PS080/rest-api)
  - [SSkin Model Trainer](https://github.com/Capstone-2022-C22-PS080/ML-Bangkit-Capstone)
  - [Android App](https://github.com/Capstone-2022-C22-PS080/sskin-mobile)

- Utility Repositories
  - [Model Uploader](https://github.com/Capstone-2022-C22-PS080/Model-Uploader)

### Dataset

- [Dermnet Public Dataset](https://www.kaggle.com/datasets/shubhamgoel27/dermnet)

### Research
