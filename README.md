# deadboyfriend.github.io
├─ index.html
├─ style.css
├─ script.js
└─ assets/
   ├─ photos/
   └─ videos/
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Your Name — Photo & Film</title>
  <link rel="stylesheet" href="style.css"/>
</head>

<body>
  <header>
    <h1>jess</h1>
    <nav>
      <a href="#photo">Photo</a>
      <a href="#video">Film</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="photo" class="grid">
    <img src="assets/photos/photo1.jpg" alt="">
    <img src="assets/photos/photo2.jpg" alt="">
    <img src="assets/photos/photo3.jpg" alt="">
  </section>

  <section id="video" class="grid">
    <video src="assets/videos/video1.mp4" controls muted></video>
    <video src="assets/videos/video2.mp4" controls muted></video>
  </section>

  <footer id="contact">
    <p>Email: jz041813@gmail.com</p>
    <p>Instagram: @falyerta</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Helvetica, Arial, sans-serif;
  background: #0f0f0f;
  color: #f5f5f5;
}

header {
  padding: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav a {
  margin-left: 20px;
  text-decoration: none;
  color: #aaa;
  font-size: 14px;
}

nav a:hover {
  color: #fff;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 20px;
  padding: 40px;
}

img, video {
  width: 100%;
  height: auto;
  object-fit: cover;
}

footer {
  padding: 40px;
  font-size: 14px;
  color: #aaa;
}
document.querySelectorAll("video").forEach(video => {
  video.addEventListener("mouseenter", () => video.play());
  video.addEventListener("mouseleave", () => video.pause());
});
