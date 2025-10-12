# Hey 👋, I'm Amal Thomas

<p align="center">
  <a href="https://github.com/DenverCoder1/readme-typing-svg"><img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=20&pause=1000&color=00FF7F&random=false&width=435&lines=MERN+Stack+Aspirant;Frontend+Developer;Learning+the+Backend+Stack." alt="Typing SVG" /></a>
</p>

---

## 🚀 About Me

💡 Passionate about building fast, modern web applications.
🎯 **Goal:** To become a proficient **MERN Stack Developer** (MongoDB, Express, React, Node.js).
🌱 Currently solidifying my backend knowledge in **Node.js** and **Express**, and diving into **MongoDB** for database management.
💻 Building small projects to integrate my frontend (HTML, CSS, JS) and backend skills.

---

## ⚡ Tech Stack

| Proficient Skills | Learning/Studying |
| :---: | :---: |
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) | ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=flat&logo=node.js&logoColor=white) |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white) | ![Express.js](https://img.shields.io/badge/express.js-%23404D59.svg?style=flat&logo=express&logoColor=white) |
| ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) | ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white) |

---

## 🔥 GitHub Stats

![Amal's GitHub Stats](https://github-readme-stats.vercel.app/api?username=amalthomas26&show_icons=true&theme=tokyonight)

![Amal's Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=amalthomas26&layout=compact&theme=dracula)

---

<p align="center">
  <img src="https://raw.githubusercontent.com/amalthomas26/amalthomas26/output/github-contribution-grid-snake-dark.svg" alt="Snake Animation" />
<p>


// Authorization token that must have been created previously. See : https://developer.spotify.com/documentation/web-api/concepts/authorization
const token = 'BQCyD7ouXoiJ14sNLg1Hpb_1E7w1DzU3dL-y3i6eoCUejBHa3YhxXF9xZWkU5Qe0g_ov2VEtBpfj6NDwdfOA9m16hIi2cpCgvz2JmCPmsIbguHgih_hnjYRXWsykw7IHJTGbSEMTgRT97hJD3vzPPO4uZZz3M96fsg54Ty1N9bRKcGCWKMd1UUZJU2Lioww850z3EbRWtMnNZ60Oi_2QJE9kRKnRi_2mzIECqbhCBv0yBRPQiHIRVyD7nmBVfxydnWT1fqEtIqVJXIDUxZNNgXxhpjgoYJkM6x0cziOOErwn-iaeKG_UMWmynoZLVMf07wT0';
async function fetchWebApi(endpoint, method, body) {
  const res = await fetch(`https://api.spotify.com/${endpoint}`, {
    headers: {
      Authorization: `Bearer ${token}`,
    },
    method,
    body:JSON.stringify(body)
  });
  return await res.json();
}

async function getTopTracks(){
  // Endpoint reference : https://developer.spotify.com/documentation/web-api/reference/get-users-top-artists-and-tracks
  return (await fetchWebApi(
    'v1/me/top/tracks?time_range=long_term&limit=5', 'GET'
  )).items;
}

const topTracks = await getTopTracks();
console.log(
  topTracks?.map(
    ({name, artists}) =>
      `${name} by ${artists.map(artist => artist.name).join(', ')}`
  )
);






## 🎶 Fun Zone

![A GIF showing the weather app working on desktop and mobile screens](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExaHd1d3JzbW41dHkyY3A1YW9oejJ5OWV4MDFzOWI3ZzR3b2ZpZDBpZyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/S3thLnRWEpRwq6iDIO/giphy.gif)
<p align="center">
    "Code. Create. Repeat." 🚀
</p>

---

## 🌐 Connect with Me

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white)](https://instagram.com/amalthomas.26) 
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=flat&logo=gmail&logoColor=white)](mailto:amalthomaschennattu@gmail.com) 






























