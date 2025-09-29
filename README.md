# My Portfolio Template # My Old website design but still good

.Hey! So I made this portfolio website template for my old portfolio and I thought other students might want to use it too, or build off of it!

## What it looks like

It's a single page website with a dark theme. Has sections for your projects, about me, and contact info. The name on the homepage moves around when you hover over it which I think is pretty neat.

## How to use it

Just download everything and open index.html in your browser. Most of the stuff you need to change is in the JavaScript part at the bottom.

## File structure (kinda important)

```
your-portfolio/
├── index.html (the main file - duh)
├── images/ (put all your pictures here)
│   ├── hero-bg.jpg (background for the top part)
│   ├── projects-bg.jpg (background for projects)
│   ├── about-bg.jpg (background for about section)
│   ├── profile.jpg (your Pov)
│   └── project screenshots go here too
└── documents/
    └── your-resume.pdf (if you have one)
```

## Changing it to be about you

Ok so this part is actually pretty easy. Find this part in the HTML file:

```javascript
const portfolioConfig = {
  name: {
    first: "YOUR",
    last: "NAME"
  },
  title: "Your Title | Your Specialization",
  skills: ["React", "JavaScript", "Python", "Node.js", "SQL", "Git"],
  projects: [
    // your projects go here
  ]
};
```

Just replace all that stuff with your actual info. For projects, copy the format I used:

```javascript
{
  title: "Cool Project Name",
  tech: ["HTML", "CSS", "JavaScript"], // what you used to build it
  desc: "What your project does in like one sentence",
  longDesc: `More details about the project. You can use HTML tags in here.`,
  images: ["images/project1.jpg"], // screenshots
  links: [
    {
      type: "github",
      url: "your github link"
    }
  ],
  status: "Completed", // or "In Progress" if you're still working on it
  category: "Web Development"
}
```

## Images you need

- **hero-bg.jpg** - big background image for the top 
- **projects-bg.jpg** - background for projects section
- **about-bg.jpg** - background for about section  
- **profile.jpg** - a profesional 
- **project screenshots** - pictures of your projects

## Other stuff to change

Search for these in the HTML and replace with your info:

- Email addresses (there's like 3 of them)
- LinkedIn profile
- GitHub username
- The about me paragraph
- Education info
- Resume file name

## Making it live

I put mine on GitHub Pages which is free:

1. Make a GitHub repo
2. Upload all your files
3. Go to Settings > Pages in your repo
4. Pick your main branch
5. Done! You get a free website

You could also use Netlify or Vercel but GitHub Pages is the easiest IMO.

## Technical stuff

Uses Tailwind CSS for styling (it's pretty good once you get used to it) and Font Awesome for icons. Everything loads from CDNs so you don't need to download anything extra.

The animations are mostly CSS with some JavaScript for the interactive parts.

## Browser compatibility

Works on pretty much everything.

## Colors and stuff

If you want different colors, search for `blue-` in the HTML and replace with whatever color you want. Tailwind has tons of colors built in.

The font is Inter which looks clean. You can change it by updating the Google Fonts link and the CSS if you want something different.

## Known issues

- The background images might take a sec to load on slow connections
  
## Credits

Made this just for fun. Used some inspiration from other portfolio sites. Feel free to use it for whatever.

If you make something cool with it, let me know! Always interested to see what people build.

## Help

If something's broken or you can't figure out how to change something, just Google it or ask "ChatGPT". 

The JavaScript console in your browser will show errors if something's not working right.

---

That's pretty much it! Hope this helps someone. Took me forever to make but I'm pretty happy with how it turned out.
