# Field Guide to Media Tech + Product
The world of media tech + product can be confusing at first. As a newly professionalized division within media companies (borne jointly out of startup culture and legacy IT departments), these jobs, tools, and work can be confusing until you've actually worked within a company that has these cultures & observed how they operate.

This field guide is meant to be useful primarily for college students and professors trying to become acquainted with this field, in hopes that we might help address [the pipeline problem](http://davisshaver.com/2015/08/18/weve-got-a-pipeline-problem-in-media-tech-product/) our industry currently faces.

## The roles
### Engineering
#### Analytics/Data Science
Analytics engineers wrangle the sea of data available to the modern media organizations, trying to spot the signal in the noise. Their go-to programming languages are Python and R, and they also use proprietary systems such as Google Analytics, Omniture, Tableau, and many others. 

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
Despite its name, JavaScript has little in common with Java. JavaScript's first life – and still its most prolific use – was as the fundamental "interactive" programming language of the web. Sitting alongside HTML and CSS as one of the big three, JavaScript threads between the two, making the site dynamic. For these uses of JavaScript, many people use [jQuery](https://jquery.com/), "the write less, do more, JavaScript library." Other popular libraries include [MooTools](http://mootools.net/) and [PrototypeJS](http://www.prototypejs.org/).

Previously the domain only of the browser, JavaScript has recently become the foremost "full stack" language. It is one of the most permissive of the languages in this list, being untyped and dynamic. It can be written "raw," or via one of the many preprocessors ([CoffeeScript](http://coffeescript.org/) and [TypeScript](http://www.typescriptlang.org/) being two examples). [Node.js](https://nodejs.org/) allows developers to write JavaScript to handle back end processes; however, while excellent for high-throughput tasks, Node.js performs poorly for computationally intensive tasks. 

#### PHP
Originally little more than a templating language for C, PHP has grown to become one of the most ubiquitous server-side web languages. It has a light learning curve and a wealth of resources available. Most new web projects written in PHP make use of one of its many frameworks; [Laravel](http://laravel.com/) and [Symfony](https://symfony.com/) are the most popular. PHP's greatest weakness is its ambiguity and vaguely schizophrenic organization; its greatest strength is its community and the resources built up for it over the years. [WordPress](http://wordpress.org/) and [Drupal](https://www.drupal.org) are both written in PHP. 

#### Python
Python is a very general-purpose language - you'll find it in Web applications, data analysis, desktop software and scripts for system administrators, among other uses. Among Web developers, it might be best known for its use with the [Django](https://djangoproject.com/) framework, which was first developed at a newspaper, the Lawrence (Kan.) Journal-World. Python source code tends to have a distinctive look, since the indentation of different lines of code is significant to how the code is run.

#### Ruby
Ruby is another general-purpose language and competes with Python in many respects; if one developer uses Python for a task, another almost certainly will do the same in Ruby. It's most popular for its Web framework [Ruby on Rails](http://rubyonrails.org/). Through some quirk of history, editorial-side developers using Ruby seem to tend to work for New York-based organizations.

### Programming tools
#### Git
Git is version control system. It provides distributed, non-linear workflows that are particularly compatible with the agile methodology and collaborative development. The advantage of Git includes the ability to produce consistent change logs (_commits_), compare differences between different commits (_diff_), and branch off a particular version. “As in any VCS, you can lose or mess up changes you haven’t committed yet; but after you commit a snapshot into Git, it is very difficult to lose, especially if you regularly push your database to another repository.”([source](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics#Git-Generally-Only-Adds-Data)) You can use git on your local machine only, but to harness the power of an asynchronous workflow, it’s a good idea to pair it up with a remote destination (GitHub being one of the most popular).

**Terminologies**: `git init`, local, stage (`git add`), `git commit`, `git push`, `git pull`, `git branch`, `git merge`, `git clone`

Learn more in basic workflow in [this tutorial](https://try.github.io).

#### Github
GitHub is a web-based Git repository hosting service. Using Github for your Git-based source code management allows coders and non-coders both to access commit logs using a graphical interface. “It also provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.”([source](https://en.wikipedia.org/wiki/GitHub))

GitHub has become the hub of open-source software projects since its birth in 2007, and has evolved into a social platform for contributors. When hiring or applying for jobs, a GitHub profile can supplement one’s resume to demonstrate problem-solving process and coding ability. Individuals and teams can set up free public repositories, and pay for private repos (a similar private service is [BitBucket](https://bitbucket.org/)).

More terminologies: `fork`, `pull request`

Register a GitHub account and learn more in [this guide](http://rogerdudler.github.io/git-guide/).

#### IDE
Integrated development environments (IDE's) are comprehensive software development tools. Components can include a text editor, build/test automation tools, debugging utilities, and deployment mechanisms. Examples of IDE's include [Visual Studio](https://www.visualstudio.com/en-us/visual-studio-homepage-vs.aspx), [Eclipse](https://eclipse.org/downloads/), and [NetBeans](https://netbeans.org/).

#### Text Editor
A text editor is exactly what it says on the tin – a software programming for editing text files. On *nix, the two bigges are Vim and Emacs, but most developers you encounter are likely to use a Mac and develop in [Sublime](http://www.sublimetext.com/), [Atom](https://atom.io/), or [TextWrangler](http://www.barebones.com/products/textwrangler/). Modern text editors are generally known for their extensibility, allowing engineers to either load or write-from-scratch plugins that do things like syntax detection, linting, or format conversion. Customizing their text editor (and their terminal) is the closest the modern engineer gets to choosing his or her wand at Ollivanders. 
 
#### Unit Tests
A unit test is the core building block of [test-driven development](#test-driven-development). It tests the essence of a function. Unit tests should be written for all functions that take parameters and produce output. They should also be written for the "integration" of the various functions to test the final result. Refer to the TDD section of the field guide for more on this topic.
 
### Product management tools
#### OmniGraffle/Basalmiq
[OmniGraffle](https://www.omnigroup.com/omnigraffle) and [Balsamiq](https://balsamiq.com/) are tools popular for wireframing, the laying out of an interface using crude or "low-fidelity" stand-ins for the actual elements. Wireframes are an important part of the product development process, in which designers and product managers work from the abstract up to the concrete. This concept is well illustrated in Jesse James Garrett's [Elements of User Experience](http://www.jjg.net/elements/):
![uxpin-elements-of-user-experience-by-jesse-james-garrett](https://cloud.githubusercontent.com/assets/1636964/10003956/235673d0-607d-11e5-880c-dfa45d0f4d82.jpg)

#### Sketch
For over a decade, Adobe Photoshop and Illustrator have been unavoidable staples of the web design process, despite the fact that neither was really built with that workflow in mind. Then [Sketch](http://bohemiancoding.com/sketch/) came along. 

A web-first tool for mockups and illustrations, Sketch is the favoured alternative taking over the industry. The program’s features — such as artboards with pre-set mobile dimensions — are built with responsive web in mind. 

Sketch will even attempt to write corresponding CSS, a great first step as you flesh out your webpage. Add in an active community developing plugins for everything from Slack integration to animation and you’ve got a lightweight tool that grows when you need it to. 

Bonus: its clean interface and stripped-down functionality makes it way easier to learn than Illustrator. Even better, it’s only $99.

#### Trello
[Trello](https://trello.com/) is a list-based collaborative project management tool. A user can curate a Trello `board` made up of `lists` that can contain `cards`. Individual cards can have due dates, checklists, associated users, labels, and other metadata. Comments can be left on cards and other users may be mentioned to track the progress of large or multi-stakeholder projects. Like Slack, Trello has begun offering deeper integrations to popular services like Github, DropBox, Google Docs, Evernote, and (naturally) Slack.

## The methodologies
### Agile
Agile is a management method that aims to deliver products iteratively and efficiently, and works best in a collaborative, open, and non-hierarchical team structure. The management is distributed across the team rather than with a single manager. After becoming popular in the software development community, agile methodology has been adopted by other fields. For example, a digital news product team could include editors, designers, developers, and a product manager. Designers work with editors to think through UX; developers advise designers about UI and data management; the product manager makes sure everyone is contributing constructively, adjust expectations, and sets milestones.

Scrum is a popular technique in agile management: team members conduct very short meetings where they list what they have done, what they are working on, and what is blocking them. Popular tools used by agile teams are Slack, Trello, and GitHub.

### Human-centered design
Human-centered design is the process of exploring and understanding needs, wants, and habits of a target audience in order to create products and experiences that fit into their lives, as opposed to products that require a significant change in behavior in order to be used.

HCD is a design process championed by IDEO and its founder, David Kelley. [His TED talk is a great introduction to the discipline.](http://www.ted.com/talks/david_kelley_on_human_centered_design?language=en)

Here is the general arc of an HCD process as illustrated by IDEO in [its toolkit (PDF)](http://www.ideo.com/images/uploads/hcd_toolkit/IDEO_HCD_ToolKit.pdf):
![toolkit_arc](https://cloud.githubusercontent.com/assets/1636964/9603383/6673d20c-507e-11e5-9417-c9ab2293b652.png)

A typical HCD cycle might entail the following:

1. Project overview – what is the problem to be solved? Previously discovered quantitative and qualitative data should be made available at this stage, as well as any examples of how other bodies have attempted to solve the same problem.
2. Interviews – who are the users? who are the stakeholders? How do they talk about the problem? How does it fit into their larger life story? 
3. Persona development– how do the users compare to each other? What attributes or experiences seem common? Can we develop archetypes, or personas, that organize our individuals in a way that allows them to be referenced without mentioning a specific individual? Do we see opportunities that seem to transcend the personas?
4. Brainstorm – how might we target the opportunities identified in the previous stage? [IDEO's ground rules for brainstorming](https://openideo.com/blog/seven-tips-on-better-brainstorming) are immensely helpful here. 
5. Prototyping – how might we turn our brainstorm output into something more concrete? Paper prototypes are valuable in this stage, because they are cheap and quick. For prototypes, it's helpful to begin asking and answering questions about desirability, feasibility, usefulness, usability, and viability.
6. Feedback – Air out the most promising ideas from the prototyping stage. Talk to stakeholders who would be responsible, or involved, in delivering the ultimate product. Try to explore the same aspects mentioned above – desirability, feasibility, usefulness, usability, and viability. 
7. Deliver – At this point, the HCD process becomes more of a traditional agile/lean project. What is the business model? What are the metrics at each point of the delivery pipeline? How can you measure the value-add? What would an incremental delivery of the idea entail? 

HCD is best thought of as a framework to escape your own biases and preconceptions. It focuses, ruthlessly, on delivering value to users in the most effective and efficient way possible. 

<img width="665" alt="screen shot 2015-09-01 at 8 29 43 am" src="https://cloud.githubusercontent.com/assets/1636964/9604171/cf16c6a2-5083-11e5-8a60-fcecdbcb2d57.png">

HCD is a process that can be applied throughout the lifecycle of a product, as the above illustration from IDEO illustrates, and it complements the other methodologies mentioned here.

### Test-driven development
Test-driven development (TDD) lets you [move fast without breaking things](http://fusion.net/story/129411/move-fast-and-dont-break-things/). TDD is a methodology of development that starts with writing a "test" for whatever bug or feature is being added to the application. In true TDD, the developer's first commit will generally be a failing test for the bug or feature. When the commit is pushed to a version control server, a continuous integration (CI) like [Travis](https://travis-ci.org/) or [Jenkins](https://jenkins-ci.org/) will run the tests automatically, providing feedback to the developer about the failure or passage of the test suite.

As noted in the blog post linked above, the TDD loop goes something like this:

1. The developer writes a test and runs it.
1. The test fails and the build goes red.
1. The developer writes code to fix the test and repeats it.
1. The test passes and the build goes green.
1. The developer refactors as needed and runs the test again.

The repeated and systematic use of TDD and CI allows developers to move aggressively on the development of new features while also ensuring that all the features previously developed don't break through the introduction of a "regression", the formal term for when you screw something up. 

Different programming languages have their own unit test frameworks – some examples include [PHPUnit](https://phpunit.de/) for PHP, [RSpec](http://rspec.info/) for Ruby, [Jasmine](http://jasmine.github.io/) for JavaScript, and [pytest](http://pytest.org/) for Python.

## More resources
### Blog posts
- [How to be happy in journalism if you hate being a reporter](https://medium.com/thoughts-on-journalism/how-be-happy-in-journalism-if-you-hate-being-a-reporter-330455b87aec) (Medium, Julia Haslanger)
- [The need for product management in media](https://medium.com/@sundve/the-need-for-product-management-in-media-fe02cddf5ec3) (Medium, Espen Sundve)
- [Editor, product manage thyself](https://medium.com/technology-liberal-arts/editor-product-manage-thyself-b057af9c483e) (Paul Smalera)
