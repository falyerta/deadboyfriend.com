# deadboyfriend.github.io
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
