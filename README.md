# Quiver Launcher
Multi-game launcher ~~and idle detector~~ made for [The Full Indie Summit](https://fullindiesummit2024.eventbrite.ca/) (2024)

![image](https://github.com/user-attachments/assets/12208de3-7680-4e9b-bc66-f0243d833faa)


## Getting Started
1. `pip install -r requirements.txt`
1. `yarn` (Get NodeJS and `npm install --global yarn` if you don't have it)
1. `yarn start`

Client-side JS starts in `index.html`, "server-side JS" (ie: ran locally, privileged to do NodeJS stuff, but isolated from the client code) starts in `index.js`.

`public` and `static` folders are just for organization. Resources directly linked in the html like images and videos are automatically bundled in the final build. Other stuff is not regardless of what directory it's in.

If all that sounds like a headache, just use the dev build on game day like I did :)

## Building

1. `yarn make`
1. NOTE: Your static folder will have to be copied over **manually** into your build's folder
1. Goes without saying you will need python with the pip installed dependencies on any PC running the build

## Customization

1. Upload all yours games into the `static` folder
1. Edit the `file` attributes on the buttons in `index.html`
2. Swap out `/public/logo192.png`
3. Swap out `/public/attract.webm` with a montage of all your games available
4. Adjust the time stamps in the attract array so as games are hovered, the video player skips to the time where they are
5. Adjust the `taskill` commands in `index.js` to be for your games that are really stubborn about closing.
6. Polish whatever you want with CSS and HTML!
