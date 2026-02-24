
![Attachment.png](blob:capacitor://localhost/e01261cc-e9a7-4299-b444-e7648365a627)

Project Teapot (prjtpt) is a website that hosts multiplayer browser games.


### What’s the tech stack?
- Front-end: Vanilla
- Games: Three.js & Rapier Howler.js, etc)
- Transfer Protocol: WebTransport API
- Back-end: Golang (with quic-go & webtransport-go)
- Database: Postgres
- Hosting: Hostinger / GitHub Pages? (How much does it cost to host WebTransport connections? Can self hosting make sense here?)

We build the front-end as a SSR hypermedia application that uses three.js and various other frameworks to host clients of browser based games. It will use WebTransport API to connect to a game server built in Go. The website can also allow for profiles that could store player avatar information!

### Components:
Web application(vanilla) that includes a front page, authentication (log-in) / account creation (friends list - how do we display currently online friends - rcc?), and games page that opens up a stand alone game page using three js (pause menu allows player to go back to the games page.

Game server (golang) that allows players to open and connect to a lobby and start games with other players.

Database (or See how oAuth works? Does it require a db? I think we need a db anyway to store avatar configurations and things like leaderboards. Can this exist on the same go server? Or would this be separate?

Games:
- Table Tanks (Wii Tanks)
- [[Civilitea]](TBS)
- Ghost Hunters (Nintendo Land - Luigi’s Mansion)
- Teapotolis (RTS)
- Pirates (pirates of the Spanish Maine)
- Dungeon Delvers (Dark Souls + Betrayal)

Steps:
- [ ] Create public GitHub repo: prjtpt using go-svelte template
- [ ] Configure GitHub actions for stg & prod environments
- [ ] Create a golang application that will eventually be our server
- [ ] See if we can bundle our svelte front-end in the same repo and how that work
- [ ] Build out Postgres db and create test endpoint to get the contents of a test table
- [ ] See if we can use GitHub pages as a testing environment and then leave hostinger as the prod environment
- [ ] Design prjtpt front page and website style (3D, glassmorphism, etc?)

How much can we use AI to supplement my work?

*: we can host this on a subdomain of javiergonzalez.dev

javiergonzalez.dev should also exist at least as a single page site to land on

prjtpt.javiergonzalez.dev

Portfolio website, hosted for now on got hub pages but soon hostinger? Will be built with vanilla html and three.js with no need for a backend. How can we integrate analytics?

I think planet website could be quick and simple? 

Home - About - Work - Contact
- Hero shot over planet with sun & lens flare
- Center planet with corona/rear glow
- Exclude work section for now? (Prjtpt and itch?)
- Moon with landing site can include a contact form and socials (LinkedIn and YouTube / Twitch - once devlogs start)?

Look into tying camera movement to scroll wheel to orbit the planet and then move to a moon for the contact form