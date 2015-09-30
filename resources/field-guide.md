# Field Guide to tech + product
The world of media tech + product can be confusing at first. As a newly professionalized division within media companies (borne out of startup culture and legacy IT departments), these jobs, tools, and work can be confusing until you've actually worked within a company that has these cultures & seen how they operate.

This field guide is meant to be useful primarily for college students and professors trying to become acquainted with this field, in hopes that we might help address [the pipeline problem](http://davisshaver.com/2015/08/18/weve-got-a-pipeline-problem-in-media-tech-product/) our industry currently faces.

## The roles
### Engineering
#### Analytics/Data Science
Analytics engineers wrangle the sea of data available to the modern media organizations, trying to turn signal into noise. Their go-to programming languages are Python and R, and they also use proprietary systems such as Google Analytics, Omniture, Tableau, and many others. 

#### CMS 
CMS engineers work on the publishing systems used by news organizations. The most common open source publishing systems are WordPress, Django, and Drupal, but there are also dozens of commercial and proprietary systems used at all types of organizations, including CMS particularly suited for video workflows or print workflows. The languages used by the CMS developer vary by platform, but the most common are Python and PHP.

#### Operations
Operations engineers are generally found in larger organizations, as the ops engineer's primary responsibility is ensuring  predictable and scalable performance of an organization's technology stack. Ops engineers tend to be fluent in use of *nix command line interfaces, as well as with virtualization, container, and deployment tools like Vagrant, Docker, or Capistrano, and with cloud computing providers like RackSpace or Amazon Web Services. Automation, including configuration management and continuous integration/deployment, is a core skill for this type of engineer.

#### Frontend
Frontend engineers transform design concepts into interactive web pages using HTML, CSS, and JavaScript. Some frontend engineers also do some measure of user interface design and user experience design, though this varies by team. Frontend engineers have a big influence on perceived site performance.

### Product/UX
#### Product Manager
Product managers synthesize and influence both the inputs and outputs of a product. Product managers start with the value proposition of a product – how is success being measured? – and work towards that goal by describing the vision to other roles within a team and articulating/organizing how each unit can contribute to the greater good. Product managers tend to be comfortable with the tools used by other roles, and often provide additional value by consolidating those disparate sources of information into a single narrative for organization leadership and other stakeholders.

#### Project Manager
Project managers are generally found in larger organizations, and tend to work closely with product managers. Project managers provide a layer of order and planning to product efforts that might otherwise seem chaotic with many moving parts. Project managers help keep a team on track to meet deadlines. In teams that use one of the formal agile methodologies, project managers can serve as scrum masters or their Kanban equivalent. Project managers tend to rely on software like Jira, Trello, Pivotal Tracker, or Github to assist with these efforts.

#### UX Designer
User experience designers tend to do two types of work. The first involves new products or concepts, in which a UX designer will help the product manager and stakeholders determine the product's actual look and feel. This type of work tends to start with information architecture and user flow before diving into the actual user interface considerations. The second type of work performed by UX designers concerns existing products or interfaces, wherein a UX designer might search for additional optimizations that can be made to improve the performance of a product. The UX designer most frequently will use wireframe tools (like Balsamiq or Omnigraffle), high-fidelity mockup tools (like Illustrator or Sketch), and prototyping tools (like Invision or Oragami).

#### Quality Assurance/Support
QA and support team members vary in their level of technical ability. Some teams have QA engineers who specialize in automated testing of applications and websites, but more common is a QA/support role that falls closer to product than engineering. QA/support helps ensure that products are working as expected for the end user, whether that's a consumer, an employee, or another system. Bug tracking software is commonly used by these personnel, and you are likely to find them in issue tracking tools like Jira, Pivotal Tracker, Github, or Fogzilla, as well as communication tools such as Slack (for internal support) and email/messaging services (for external support).

## The tools
### Programming languages
#### JavaScript
#### Objective C
#### PHP
#### Python
#### Swift
### Programming tools

#### Git

Git is version control system. It provides distributed, non-linear workflows that are particularly compatible with the agile methodology and collaborative development. The advantage of Git includes the ability to produce consistent change logs (_commits_), compare differences between different commits (_diff_), and branch off of a particular version. “As in any VCS, you can lose or mess up changes you haven’t committed yet; but after you commit a snapshot into Git, it is very difficult to lose, especially if you regularly push your database to another repository.”([source](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics#Git-Generally-Only-Adds-Data)) You can use git on your local machine only, but to harness the power of an asynchronous workflow, it’s a good idea to pair it up with a remote destination (GitHub being one of the most popular of them.)

**Terminologies**: `git init`, local, stage (`git add`), `git commit`, `git branch`, `git merge`

Learn more in basic workflow in [this tutorial](https://try.github.io).

#### Github

GitHub is a web-based Git repository hosting service. It’s utilized Git for source code management, while providing coders and non-coders along an interface to access commit logs. “It also provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.”([source](https://en.wikipedia.org/wiki/GitHub))

GitHub has become the hub of open-source software projects since its birth in 2007, and has evolved into a social platform for contributors. In hiring, a GitHub profile can supplement one’s resume to demonstrate problem-solving process and coding ability. Individuals and teams can set up free public repositories, and pay for private repos (a similar private service is [BitBucket](https://bitbucket.org/).)

More terminologies: `git clone`, `git push`, `git pull`, fork, PR (pull request), issue queue

Register a GitHub account and learn more in [this guide](http://rogerdudler.github.io/git-guide/).

#### IDE
#### Text Editor
#### Unit Tests
### Product management tools
#### Invision
#### OmniGraffle/Basalmiq
#### Sketch
#### Trello
## The methodologies
### Agile

Agile is a management method that aims to deliver products iteratively and efficiently, and works best in a collaborative, open, and non-hierarchy-driven team structure. The management is distributed across the team rather than with a single manager. Started out in the realm of software development, the agile methodology has been adopted by other fields. For example, a digital news product team could include editors, designers, developers, and a product manager. Designers work with editors to think through UX; developers advise designers about UI and data management; the product manager makes sure everyone is contributing constructively, adjust expectations, and sets milestones.

Scrum is a popular technique in agile management: team members conduct very short meetings where they list what they have done, what they are working on, and what is blocking them. Popular tools used by agile teams are Slack, Trello, and GitHub.

### Human-centered design
### Jobs to be done
### Lean
### Test-driven development
## More resources
### Blog posts
- [How to be happy in journalism if you hate being a reporter](https://medium.com/thoughts-on-journalism/how-be-happy-in-journalism-if-you-hate-being-a-reporter-330455b87aec) (Medium, Julia Haslanger)
- [The need for product management in media](https://medium.com/@sundve/the-need-for-product-management-in-media-fe02cddf5ec3) (Medium, Espen Sundve)
- [Editor, product manage thyself](https://medium.com/technology-liberal-arts/editor-product-manage-thyself-b057af9c483e) (Paul Smalera)
