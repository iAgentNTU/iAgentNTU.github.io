# Guild for Editing

```
.
├── _people                 # Put your profile here
│   ├── bibtex              # Put your publication list here (optional)
│   ├── images              # Put your images here
│   └── pdf                 # Put other files here
├── _professor              # Prof. Jane's profile
│   └── images              # Images to show in Prof. Jane's page
├── publication             # Publication list of the lab
├── research          
│   ├── _posts              # Pages for research projects
│   └── images              # Images to show in project pages
└── README.md
```

Install [jekyll](https://jekyllrb.com) in your local environment. Make sure your modification actually works before push it to github.


## Add a Personal Page
First, fork this repository to your github and clone it to your host.
```Shell
git clone https://github.com/{your_github_name}/iAgentNTU.github.io.git
cd iAgentNTU.github.io
```

Use Chi-Chia Huang's file as starting point.
```Shell
cd _people
cp Chi-Chia_Huang.md your_name.md
```

Edit the header part of your_name.md
```Markdown
---
layout: people                                               # Do not change
hidden: true                                                 # Do not change
title: Chi-Chia Huang
name: Chi-Chia Huang
chinese_name: 黃啟嘉
student_id: d01944003
status: quit                                                 # [ongoing|graduated|quit]
program: PhD student                                         # [PhD student|Master student|Undergraduate]
entry_year: 2012
exit_year: 2017
link: true                                                   # Do not change
external_url:
image: /people/images/chichia.jpg
research_interests: recommender system, internet of things
show_project: true                                           # false if you do not have any project yet
brief: 
# bibsrc: /people/bibtex/chichia.bib
bibsrc: '#bibtex'                                            # path to bib file or DOM id 

email:
  href: "http://www.google.com/recaptcha/mailhide/d?k=01MhlRNlCYMQRB3CtGk9pPWQ==&amp;c=Seat9oiuZshm6ibK_MUDZilOr7fBybQahRY7P83oUwM="
  onclick: "window.open('http://www.google.com/recaptcha/mailhide/d?k\\07501MhlRNlCYMQRB3CtGk9pPWQ\\75\\75\\46c\\75Seat9oiuZshm6ibK_MUDZilOr7fBybQahRY7P83oUwM\\075', '', 'toolbar=0,scrollbars=0,location=0,statusbar=0,menubar=0,resizable=0,width=500,height=300'); return false;"
homepage: 
facebook: https://www.facebook.com/Huang.ChiChia
linkedin: https://www.linkedin.com/in/chichiah
twitter: https://twitter.com/Chifatty
github: https://github.com/chifatty
---
```
For email part, you can just put your email here as
```
email: xxxx@xxxx.com
```
or you can use [Mailhide](https://www.google.com/recaptcha/admin#mailhide) service. Copy the value of `href` and `onclick`, and __please remember to escape `\` with `\\`__.

Then you are free to write anything you want. Please refer to [Jekyll Docs](https://jekyllrb.com/docs/posts/) for more information.

After you finish editing, __please examine the result in your local environment first__. If you are sure that everything works well, you can push your local branch to github.
```Shell
git push origin master
```

Then, fire a pull request on github page, and wait for the admin to merge your change.

## Add a Research Project Page
