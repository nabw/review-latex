# Latex package "review"
Minimal latex package for a hassle free reviewing process (beyond the review itself anyway). To use, just put the `review.sty` package next to your `main.tex` and import it with 
    \usepackage{review}

Usage is very simple, use this pseudo-latex review as an example: 

    \section*{Reviewer \#1}

    \reviewer{I reviewed this work and find it unbearable. Please delete it from the internet so that others don't need to go through the pain of reading it. Please see the following detailed questions.}

    We thank the reviewer for their thorough revision.

    \question{Why is this work so awful?}

    % Work in progress answers are red
    \answerWIP{Well, it is because... [what should I write here?]}

    \question{You missed the work by Mr Reviewer et al. (1865)}

    % Done answers are denoted as so in the code for readability
    \answerDone{We thank the reviewer for this suggestion, which we have added as follows:

      % You get a framed minipage for in-work quotes if you want.
      \citeinwork{ [...] this work was better done elsewhere [Rev65] }

    }
