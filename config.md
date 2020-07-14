<!--
Add here global page variables to use throughout your
website.
The website_* must be defined for the RSS to work
-->
@def website_title = "Julia Streamers"
@def website_descr = "Here is where you find all things Julia streaming!"
@def website_url   = "https://tlienart.github.io/FranklinTemplates.jl/"

@def author = "Septimia Zenobia"

@def mintoclevel = 2

<!--
Add here files or directories that should be ignored by Franklin, otherwise
these files might be copied and, if markdown, processed by Franklin which
you might not want. Indicate directories by ending the name with a `/`.
-->
@def ignore = ["node_modules/", "franklin", "franklin.pub", "documentation.md"]

<!--
Add here global latex commands to use throughout your
pages. It can be math commands but does not need to be.
For instance:
* \newcommand{\phrase}{This is a long phrase to copy.}
-->
\newcommand{\R}{\mathbb R}
\newcommand{\scal}[1]{\langle #1 \rangle}
\newcommand{\streamer}[4]{
    @@card 
        @@avatar ~~~<img src="/assets/streamers/!#3"/>~~~ @@ 
        @@badge ~~~<a href="https://www.twitch.tv/!#1"><img src="https://img.shields.io/twitch/status/!#1?label=!#2&logo=twitch&logoColor=blue"/></a>~~~ @@
        @@name #2 @@ 
        @@desc #4 @@ 
    @@}

\newcommand{\style}[2]{~~~<span style="!#1">!#2</span>~~~}
