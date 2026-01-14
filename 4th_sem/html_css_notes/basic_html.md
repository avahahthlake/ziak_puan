# Web Development Basics

## Hypertext Markup Language (HTML)
* It gives the structure of a webpage.
* It is the foundation, the skeletal structure of a website.

## Cascading Style Sheet (CSS)
* It adds style to a webpage.
* Decorations & design of a webpage.

---

## What you need to code up some website...
* **Browser:** Like Firefox (goated) or Chrome (mid).
* **Text Editor:** Like Notepad (goated), Neovim, or VS Code.

## Setup Process
1. First, install **VS Code** and open a folder; you could name it "website" for instance.
2. Inside that folder "website", make a file called `index.html`.
3. To make your life easier, install the **"Live Server"** extension, which will eventually make sense in a while.

---

## Basic example of `index.html`
```html
<!DOCTYPE html>
<html>
  <head>
    <title>My first website</title>
  </head>
  <body>
    <h1>This is an h1 heading</h1>
  </body>
</html>
```

# Multimedia and Icons

## Putting video on a webpage
To embed a video, use the `<video>` tag with attributes for dimensions and playback behavior.

```html
<video width="500px" controls autoplay muted loop>
    <source src="some_video.mp4" type="video/mp4">
    <source src="another_video.webm" type="video/webm">
</video>
```