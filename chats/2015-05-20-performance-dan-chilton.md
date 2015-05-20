# Frontend performance with Vox Media

On Wednesday, May 20th, we had a casual chat about website performance with Dan Chilton ([@bjork24](https://twitter.com/bjork24)), Jason Ormand ([@okor](https://twitter.com/okor)), and Ian Carrico ([@iamcarrico](https://twitter.com/iamcarrico)) of Vox Media.

You can read the [full chat in Slack archives](https://newsnerdery.slack.com/archives/watercooler/p1432144794001061). The following is a summary of what we discussed. If you have a suggestion for a future chat, please drop by `#meta` in Slack.

### Q1: I’m new to frontend performance. What should I look for, and how should I look for it?

* Page load time, specifically to get the page load time as low as possible. Two tools you can use are Chrome's Dev tools network tab and [Web Page Test](http://www.webpagetest.org/). You should also track page weight (e.g. size in MB) and the number of HTTP requests.
* Page load time isn't the time to load everything, though. 
* Q: Thoughts on perceived performance?
* Paul Irish just had a GREAT talk at FluentConf [about thinking about performance as his “RAIL” idea](http://fluentconf.com/javascript-html-2015/public/schedule/detail/40733).
*  Filament Group does a [great job of illustrating it too](http://www.filamentgroup.com/lab/weight-wait.html).
* Q: What are some recent before and after numbers you’ve seen at Vox?
* Vox has just started diving into the meat of our optimizations, so they haven't seen a lot of BIG needle-moving yet... but they're coming.
* Vox is still very much in the `before` of our before and after journey, and they're happy to talk about those in detail.

### Q2: What’s the single most challenging aspect to frontend performance?

* Since Vox has an ad based revenue model ... it's ad performance. Many advertisers and vendor tools have the expectation of being loaded synchronously. We are working to change that (to all async) but it's a very difficult task with many considerations. Ensuring a web asset makes performance sense is relatively straight forward. But ensuring performance goals align with business goals can be very tricky business.
* Also, legacy code. There was a time on the web where Vox wrote JS synchronously. Where they used tables, and didn’t use floats. But much like the change to RWD required a change in thinking about how they write code, a change to a focus on performance will require the same. And just like RWD requires altering how we design, how Vox thinks about projects, how they test our sites: Performance requires changing/challenging current perceptions on the development cycle and how they design/build web experiences.
* A large component of Vox's job is to educate the rest of the team (designers, developers, editorial) about the potential performance implications of their decisions. They believe very strongly that performance should be everyone's concern, not just the purview of our small team.
* Two more cents from Daniel @ Fusion: 1) knowing where to begin with optimizations, and 2) making sure you don’t take one step forward during a performance sprint, and two steps back as a part of your normal product development.
* Fusion had a “performance week” a month and a half ago. They captured lessons learned [on their blog](http://fusion.net/story/121962/performance-is-a-feature-speeding-up-fusion-net/). As a part of the process, they set up [Speedcurve](http://speedcurve.com/) to monitor site performance. However, they haven’t successfully adopted it.
* Vox has an internal tool called Tempo and is also running Speedcurve.

### Q3: What’s one frontend perf trick you wish you had learned at the very beginning?

* The trick is that there are no tricks. It's all about where you get your information. There are a LOT of people out there who are doing great work, writing posts, etc. Finding those people, reading their things, and trying to implement is more useful than anything.
* To get started, you should investigate and measure. Form a hypothesis. Make a change with as limited scope as possible. Measure again. Invalidate/validate hypothesis. If the data checks out, push to production. If not, wash rinse repeat.
* For Dan @ Vox, it was learning to dig deeper into the dev tools. Some recommended videos include https://www.youtube.com/watch?v=S9sktFzL3tQ, https://www.youtube.com/watch?v=gZH1d2Co1X0
* Giving things a pass with [Google Pagespeed](https://developers.google.com/speed/pagespeed/insights/) is "crazy illuminating"
* Q: Regarding LoadCSS and inlining critical CSS, have you found that challenging to work into CMS workflows?
* A little: When Ian was at Four Kitchens, they used it in Drupal, and just did some manual running / testing to ensure the output was right. But they got it to work fairly easily just by commiting our critical CSS to git and having Drupal load it inline. The critical inline CSS was broken apart based on different template files (e.g. home vs. article).
* Web Page Test is an invaluable tool, and Vox is leveraging it internally with their Tempo app.

### Q4: What’s a frontend performance issue you’re currently working on?

* Asynchronous JavaScript code. This isn’t a “quick fix”, nor something they expect to get out the door tomorrow — but certainly something worth focusing on. Vox is working with several team to get a better way of running all of their JavaScript in a unified fashion, and getting legacy code up to speed in the process.
* SPDY/HTTP2.0 are coming to static assets at Vox pretty soon, which is exciting.
* Async ads are also on the roadmap, as is evolving performance tools around metrics tracking and workflow automation.
* Ian @ Vox has been working on loading our fonts with LoadCSS and using Font Face Observer to ensure Vox don’t get any FOIT. So far, we have had GREAT results. Jonathan Suh has a [great post](https://jonsuh.com/blog/font-loading-with-font-events/).
* Q: How does Vox fit refactors into the product backlog?
* It depends on the scope of the refactor. They are constantly pushing and iterating Chorus with small refactors, but large ones (like making The Verge fully responsive) is approached more like a new vertical. In that case, we devote a team to the refactor project and take our time to make it as solid as possible.
* Q: Have you run into any push back over FOUT?
* Not yet! But Ian @ Vox did work heavily with designers to make sure they had some reasonable fallback fonts. The FOUT is not FOUT as much as Flash Of Less Styled Text
* Q: Has anyone found lazyloading images to be a big performance booster on news sites?
* Vox uses JS client side to load images async and hopefully as close to the perfect size as possible in most places. Async image loading is a big WIN. Next up, support for Webp to save bandwidth and async load times.

### Q5: Who are some people to follow on Twitter / RSS for good performance tips?

* In no particular order: @lara_hogan, @paul_irish, @tkadlec, @igrigorik, @addyosmani, @Souders, @ianfeather, @scottjehl, @rdmurphy, @andydavies, @katiekovalcin, @patrickhamann, @jonsuh, @Perf_Rocks, @pathtoperf, @filamentgroup, @SaraSoueidan, @guypod, @tameverts, @jefflembeck
* Lots of +1's for Velocity conference. The NY Perf Meetup Group usually meets the day after Velocity with the same attendees and only costs $15.

### Q6: What tools / processes do you use to make performance a feature of every project?

* Vox has [Justice.js](https://github.com/okor/justice) for everybody on product to view the performance impact of what they building, as they are building it and after it's pushed to production.
* Vox also to wants to have testing on each branch and notify in GitHub PRs, but they haven’t yet gotten to a point that we can achieve that in a productive manner. The repo https://github.com/fourkitchens/frontend-perf shows a really simple example of getting TravisCI performance testing into every PR. Clearly: a very simple one… but something they want to do in a larger fashion.
* Vox is also looking to extend Tempo with Elastic Search + Kibana for getting more comparative metrics and map those back to our commit log.
* Mapping commits to performance changes is of high importance, they are considering automated reports that will go out to devs post commit.
* Q: What else do you use for perf dashboards?
* SpeedCurve and Tempo are two synthic perf tools Vox uses to measure long term perf trends. This is mostly for the for the perf team but all team members can look at their dashboards. They collect a lot of data via Tempo and use Grafana to compile and represent visually. Pretty power interface to perusing data.
* Q: What are your pain points for doing perf testing on Travis?
* Two things: 1) Having an accurate testing environment that mimics production BEFORE code gets to production. 2) Setting up clear budgets on a legacy code base that reflects the end limit of what is allowed.

### Q7: How do you evangelize performance to the rest of your team / company?

* Vox is working on a mixture of things. They are lucky that they have a team that already understands the need for frontend performance, but there are many ways to get a team “on board”. Sharing performance stats, goals, budgets are all great— but generally require an understanding of what things like “Speed Index” actually mean. Something they stole from Etsy / Lara Hogan is to share videos from Web Page Test of our site loading at different speeds and compared to other competitors. Nothing beats having a video that anybody can take a look at to see the exact impact performance can make. They also like to share stats or studies that they find that has the impact of performance included.
* The most excellent Chris Ruppel (@rupl, follow him too!) and Ian @ Vox did a talk on creating a culture of performance, and specific things you can do to everybody in the team (from CXO to developer) to get more buy-in. https://events.drupal.org/losangeles2015/sessions/creating-culture-performance
* Surfacing important performance metrics is one of their most important tasks. They want to make those numbers omni-present and supremely accessible
* Q: Have you built a slack bot for these things yet?
* Good idea for Vax!!! Dan @ Vox would love to see alerts sent out for both big perf gains and losses.

### Open mic

* Q: For your lazyloaded images, what happens when JS on the page breaks? We had lazyload in production for a while, but were running into a variety of implementation issues that caused the general quality/reliability of images on our site to be subpar
* Don't let JS break. But really, there should be some good testing in to make sure broken JS isn’t added, and more importantly error handling.
* Four Kitchens ran into this issue with soem Drupal code, where one small piece would break, and everything else would. We ended up implementing more solids tests to check for that.
* Q: There are more and more tools for measuring page load, what do people use for measuring jank / user experience after the page has load and the scrolling begins?
* Ian @ Vox tests jank purely in Chrome’s dev tools. It may not work to show EVERYBODY’s experience, but the tools are incredibly deep— and can help find a variety of issues
* Justice.js has a streaming FPS meter which was designed to give developers feedback on scroll related issues. If you see peaks and valleys during scroll, you may have an issue. Then open up dev tools and find out why.
* Super critical JS should be inline, but everything else should just be progressive enhancement
