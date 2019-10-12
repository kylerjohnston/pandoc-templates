$if(name)$
$name.first$ $name.last$
$endif$
$if(address)$
$address$
$if(city)$
$city$
$endif$
$endif$
$if(cellnum)$
Phone: $cellnum$
$endif$
$if(email)$
Email: $email$
$endif$
$if(website)$
Website: $website$
$endif$
$if(github)$
Github: $github$
$endif$
$if(additional-info)$
$additional-info$
$endif$

$if(skills)$
Skills
------

$for(skills)$
$skills.category$: $skills.skills$
$endfor$
$endif$

$if(experience)$
Work Experience
---------------
$for(experience)$
$experience.years$. $experience.title$, $experience.employer$, $experience.city$.
$experience.description$
$if(experience.achievements)$
$for(experience.achievements)$
  - $experience.achievements$
$endfor$
$endif$

$endfor$
$endif$

$if(volunteer)$
Volunteer and Service Work
--------------------------
$for(volunteer)$
$volunteer.date$. $volunteer.title$, $volunteer.employer$, $volunteer.location$.
$volunteer.description$

$endfor$
$endif$

$if(projects)$
Independent Projects
--------------------
$for(projects)$
$projects.date$. $projects.url$. $projects.github$.
$projects.description$
$if(projects.stack)$
$for(projects.stack)$
  - $projects.stack$
$endfor$
$endif$

$endfor$
$endif$

$if(publications)$
Publications and Presentations
------------------------------
$for(publications)$
$publications.date$. "$publications.title$." $publications.publisher$, $publications.location$.
$endfor$
$endif$

$if(education)$
Education
---------
$for(education)$
$education.years$. $education.degree$, $education.institution$, $education.city$.
$if(education.gpa)$$education.gpa$$endif$. $education.description$

$endfor$
$endif$
