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

- **Cloud Computing Learning Path**

  - Ardinata Hari Saputra (**C2009G0955**) (_Universitas Gunadarma_)
  - Muhammad Rayhan Hamada Budiman (**C2009G0981**) (_Universitas Gunadarma_)
    <br />
    <br />

- **Machine Learning Learning Path**

  - Amar Rahman Kamal (**M2004F0189**) (_Institut Teknologi Sepuluh November_)
  - Rizkyka Mediano Sandie (**M7009G0995**) (_Universitas Gunadarma_)
    <br />
    <br />

- **Mobile Development Learning Path**

  - Ahmad Budi Gustama (**A7211G1943**) (_Universitas Indraprasta_)
  - Nabilah Putri Cantika (**A7211F1961**) (_Universitas Indraprasta_)
    <br />
    <br />

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
  Where user can see list of their skin disease diagnoses, that consist of predicted condition, photo of their region of skin, overview of the predicted condition and   if exists, the first-aid solution to the condition, like treatment methods, or even if possible, medicines recommendations.

### Plan

#### Cloud Infrastructure

<img src="https://raw.githubusercontent.com/Capstone-2022-C22-PS080/.github/main/GCP_Infrastructure_Diagram.svg" />

#### Explanation
- For authentication we will use Firebase Authentication, allowing user to sign up either with email and password, or just simply OAuth button tap. 
- For serving user-related data such as user profile and diagnostic histories.
- Most prediction stuffs are mainly handled by Google App Engine that act as a REST API server. After getting prediction result from Tensorflow prediction in the app engine, specifically POST /predictions endpoint, based from the result, GAE will fetch diagnosed skin disease's data from PostgreSQL instance (Compute Engine) that act as database instance. After that GAE will respond to mobile client with disease data.
