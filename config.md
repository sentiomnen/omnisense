<!--
Add here global page variables to use throughout your
website.
The website_* must be defined for the RSS to work
-->
@def website_title = "omnisense"
@def website_descr = "Website for share studies of sentiomnen"
@def website_url   = "https://omnisense.vercel.app/"

@def author = "sentiomnen"

@def mintoclevel = 2

<!--
Add here files or directories that should be ignored by Franklin, otherwise
these files might be copied and, if markdown, processed by Franklin which
you might not want. Indicate directories by ending the name with a `/`.
-->
@def ignore = ["node_modules/", "franklin", "franklin.pub"]

<!--
Add here global latex commands to use throughout your
pages. It can be math commands but does not need to be.
For instance:
* \newcommand{\phrase}{This is a long phrase to copy.}
-->
\newcommand{\R}{\mathbb R}
\newcommand{\scal}[1]{\langle #1 \rangle}

<!--Text elements-->
\newcommand{\center}[1]{@@center !#1 @@}
\newcommand{\right}[1]{ @@right !#1 @@ }
\newcommand{\serif}[1]{ @@serif !#1 @@ }
<!--Special paragraphs-->
\newcommand{\proof}[2]{
   @@proof
   **Proof.** $!#1$\\
   !#2
   @@
}

<!--Layout-->
\newcommand{\link}[2]{
   @@link
   ~~~<a href="!#1">~~~
   !#2

   ~~~</a>~~~
   @@
}