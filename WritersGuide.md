New Writers Guide
===

Timothy Boronczyk

*A writer is a person for whom writing is more difficult than it is for most people.* - Thomas Mann

Writing is a fun way to share your knowledge, experience, and opinions with others, and it can also be very rewarding. Writing about a topic that's new to you may help solidify your own understanding of it (or your friendly editor may point out an easier way of doing something you didn't know before) and make you a better programmer. Or, writing may serve as an avenue for you to become more involved in the community; writing successful articles and blog posts can give you confidence to submit and present a talk at any number of professional conferences held around the world. No one knows exactly what the future brings, but the skills you cultivate and the friendships you form through writing have the potential to open up many opportunities.

But unfortunately, writing can also be intimidating and frustrating for some people. Perhaps you're not sure how to explain a particular concept, or maybe your editor sent back your first draft all marked up with red. When such things happen, it's important you don't grew discouraged. Believe in yourself, accept reasonable criticism, and persist onward.

With all of this in mind, this document was prepared to help minimize the frustration and self-doubt that new writers (and even experienced writers) can experience. It provides practical suggestions and examples for finding inspiration, structuring your content, building a positive working relationship with your managing editor, avoiding plagiarism, and growing your self-confidence. Hopefully it'll help you to write awesome articles, realize the many benefits of writing in your life, and minimize any anxiety or stress you may experience along the way.

Finding Inspiration
---

*You can't wait for inspiration, you have to go after it with a club.* - Jack London

There will be times when you have the urge to write but you're not sure of exactly what to write; indeed, coming up with a good topic can be challenging. Here's a little secret, though... inspiration is everywhere.

Ideas can be found in a variety of places, some of which might seem counter-intuitive at first. You can learn to identify them more easily by always being on the lookout as you go throughout your daily activities. For example, think about the project are you working on at your day job or in your spare time. Is it something others might find interesting? (Of course, if it's proprietary code then make sure whatever you write about is permitted and that you've sanitized any trade secrets.)

Reading the work of others can also be a source of inspiration. Many of us frequent sites like [reddit](http://www.reddit.com), [DZone](http://www.dzone.com), and [StackOverflow](http://stackoverflow.com) on a daily basis but don't realize the glimpse into the programming zeitgeist they provide. Don't limit yourself to just sites that pertain to your favorite technology, either. If you're a PHP developer, by all means check out the blogs on [PHPDeveloper.org](http://www.phpdeveloper.org), but then check out [Planet Smalltalk](http://planet.smalltalk.org) as well. People are doing exciting things in other languages and you might find inspiration from their work too.

If you find yourself in a real bind, there's always the option of asking others for suggestions. When I was the managing editor for PHPMaster.com, I set up a mailing list for regular authors to discuss topics and I keep a short list of additional topics on hand just in case I was asked. Some of the topics were for articles I wanted to see on the site but didn't had the time to write myself, and others were suggestions from programmers who would like to read them but didn't have the background themselves to write them.

Before You Begin...
---

*By failing to prepare, you are preparing to fail.* - Benjamin Franklin

Some authors prepare an outline to organize their thoughts before writing, and others write from the pen with only a vague idea beforehand of what they want to discuss and in what order its elements will be presented. You don't necessarily need a formal outline enumerating each talking point, but you should have some plan of attack before you start writing. Writing blindly is never a good idea.

### Who Is your Target Audience?

First identifying the nature and expectations of your target audience goes a long way in turning your inspiration idea into a successful article.

If you're writing about recursion, ask yourself whether you are targeting beginners or established programmers; the focus would be different for each group. Beginners need a clear, unambiguous definition of recursion almost immediately, and probably won't need to know about head/tail calls. Experienced programmers will know what recursion is already but might be looking for more substantial content related to language internals (call stack, head/tail behavior, etc).

### What ONE Thing Will your Article Accomplish?

An article should have one solid goal. Once you identify what your main point will be, all content in the article should be leading towards that.

Staying with the topic of recursion, would the article encourage users to use recursion? Is the purpose to teach them the basics of recursion? Would it warn them of the dangers of recursion? What about identifying when recursion is useful? Each of these could be a strong article, but together they would overwhelm the reader with too much information and possibly not enough explanation.

### What is a Good Logical Flow?

With your article goal in mind, ask yourself where does the discussion start and where does it end, and on that path what points are worth stopping at to take a closer look. Does point A lead to B, which then leads to point C, and then ultimately to point D? Don't jump around from point A to C to D to B! Each idea should build upon the preceding point.

I wrote [Working with Slim Middleware](http://www.sitepoint.com/working-with-slim-middleware) to show readers how to implement custom middleware components for the Slim framework. The article is too long to reproduce here but I invite you to read through it and take note of its logical progression.

 1. Understanding Middleware
 2. Implementing Middleware
 3. Registering and Configuring Middleware

It's important to first have an understanding of the architecture related to middleware to properly implement a middleware component (point 1). After conveying that information, I moved on to show how one writes a custom component (point 2). Once the reader had a custom component, I offered guidance on deploying and using it (point 3). Each point naturally leads to the next, and each point depends on the previous.

The Essay Structure
---

*The skill of writing is to create a context in which other people can think.* - Edwin Schlossberg

The standard essay-structure is often a good device to employ when you first start writing articles since it's especially well suited to tutorials and how-to articles. The essay contains an introduction, a detailed body, and a summary or conclusion. You can experiment structuring your articles in different ways as you grow and gain confidence in your abilities as a writer, but the essay-structure is tried and true.

### The Introduction

The introduction is the first part of your article. As such, it's important to make a good first impression with the reader. The introduction should:

 1. Entice the reader and pull him into your article because he wants to read more,
 2. Introduce the main concept your article,
 3. State the goal/purpose of the article, and
 4. If the article is part of a series, identify how many parts are in the series and what installment this article is.

Enticing the reader sometimes requires a little bit of creativity. For example, it's hard to get someone excited over the Scatter-Gather integration pattern. You could use a personal anecdote to catch the reader's attention and relate a particular problem you faced which was solved by using the pattern.

The main concept of the article should be defined in the introduction as well. Continuing the example, you could explain that Scatter-Gather is a pattern applicable to integrating enterprise systems. It routes a request to a number of recipients and then collects and distills the responses into a single response.

And finally, the purpose of the article should be clearly stated. This is your promise to the reader. Usually (but not always) it looks like "In this article you will learn how to..." or "I will show you how you can..." Stating the purpose of the article is important because it helps the reader clearly and unambiguously identify what the article is about and whether it's something he's willing to devote his time to read.

Here's an example of an introduction:

    Comparison shopping is nothing new but has become infinitely easier since the advent of the Internet. Major sites like Nextag and shopzilla let consumers find the best price on any number of products with just a few mouse clicks. Recently, I was tasked with implementing a similar concept as part of a client's web application; it needed to connect to several different APIs to obtain price lists and the best price would be cached in a database. It was then when I learned about Scatter-Gather, an enterprise integration pattern which routes a request to a number of recipients and then collects and distills the responses into a single response. The client system would initiate requests to various vendors and the responses would be funneled to a collector process to determine the lowest price.
    While understanding the pattern was easy for me, I encountered a few unexpected issues while implementing it. In this two-part series I'll share with you what I've learned so that, hopefully, you can avoid the same mistakes I made. In this part you'll learn how to identify when the Scatter-Gather pattern is appropriate and when it's not, and how you can implement it with a minimal amount of fuss with Apache Camel. In Part 2 I'll teach you the key things you'll need to know to scale your solution successfully.

Try to identify each of the key ingredients in the example introduction. How does the author try to draw the reader into the article? What is the main concept? Is it clear what the purpose of the article is?

### The Body

The body of the article expounds on the ideas first given in the introduction and fulfills the commitment made by the author to the reader. Generally it's encouraged to divide the body of lengthier articles into sections which serves three purposes:

 1. Foreshadow what steps the readers will go through as they learn about the topic
 2. Allow readers to easily find an important section they may want to read again later, and
 3. Break the body up so the article doesn't look like a giant wall of text when it's published.

Each section should be given a header so the reader can easily see the shape of the article. For example, the article [Watermarking Images with Imagick](http://www.sitepoint.com/watermarking-images) I wrote teaches people how to programatically add a watermark to an image using PHP and the ImageMagick extension. It contains body sections on what makes a good watermark, applying the watermark, and scaling the watermark when the target image is smaller than the mark. Together the section headers create a road map which helps the reader gain a broad-level understanding and get their bearings simply by skimming through the article.

When providing code examples in your article, it's also preferable that you first discuss what functionality is needed, then present the code, and then discuss the code itself. This pattern of requirement-code-discussion mimics discovery-based learning by subtly encouraging readers to think about a problem, providing the solution, and then reinforcing the solution through explanation.

Here's an excerpt from the article to illustrate this:

    SCALING THE WATERMARK
    [...] While this approach is fine if you know the size of the original images beforehand since you can create the watermark with the appropriate dimensions, you might want a more robust approach in case the sizes of the original images vary. Such an approach might be to place the watermark in the center of the image and scaling the watermark beforehand if it is larger than the original image.

    <?php
    // how big are the images?
    $iWidth = $image->getImageWidth();
    $iHeight = $image->getImageHeight();
    $wWidth = $watermark->getImageWidth();
    $wHeight = $watermark->getImageHeight();
    if ($iHeight < $wHeight || $iWidth < $wWidth) {
        // resize the watermark
        $watermark->scaleImage($iWidth, $iHeight);
        // get new size
        $wWidth = $watermark->getImageWidth();
        $wHeight = $watermark->getImageHeight();
    }
    // calculate the position
    $x = ($iWidth - $wWidth) / 2;
    $y = ($iHeight - $wHeight) / 2;
    $image->compositeImage($watermark, imagick::COMPOSITE_OVER, $x, $y);

    The getImageWidth() and getImageHeight() methods return the width and height of an image respectively, measured in pixels. By comparing the width and height of the watermark image to those of the original image, you can determine whether or not it is necessary to resize the watermark so it will fit on smaller images.

    Resizing the watermark is accomplished by calling the scaleImage() method which takes an allowed width and height. The method will scale the image down so that the maximum width is no larger than the allowed width, and the maximum height is no larger than the allowed height, while maintaining the image's aspect ratio.

This example is a section with the header "Scaling the Watermark." The paragraph prior to the code sample explains what functionality is needed – the code should be able to watermark images that are not of a predetermined size. The code is then presented which demonstrates how to scale the watermark based on the size of a target image and positions the watermark in its center. The two paragraphs that follow then explain the salient parts of the code.

Besides giving less-experienced readers reinforcement opportunities by presenting your code first followed by its explanation, another benefit is that it allows experienced readers to save time by skipping over the text if they understand the code. This is more difficult if the code is presented only a few statements at a time and the explanation is interspersed, or if the explanation of the code is contained entirely within code comments.

### The Conclusion

Just as a good host invites his guests in at his door and then later sends them off home with a smile, a good article greets readers with the introduction and waves goodbye with the summary. Your article should conclude with a final summary or conclusion section, the purpose of which is to avoid a sudden and jarring ending. It offers you a final chance to reinforce the key points of your article, tie up any loose ends that may be left, and perhaps identify where the reader can go to find more information if he's interested.

My article [Migrate from the MySQL Extension to PDO](http://www.sitepoint.com/migrate-from-the-mysql-extension-to-pdo) teaches the basics of updating PHP code which uses the older mysql extension with PDO instead. Here's its conclusion:

    Now you have the basic knowledge necessary to start migrating from the older MySQL extension to the newer PDO extension. You've seen that while most of the time PDO is already available, it's easy to set up if for some reason it isn't. You've also seen how easy it is to connect to a MySQL database server, issue queries, and receive the results. Of course this was just a practical overview; to learn more about what PDO has to offer and how you can take advantage of it, I encourage you to read the available documentation at php.net.

The example confirms the promise I made in the introduction (to impart the knowledge necessary to start using PDO) was satisfied in the article's body. It then reiterates the concepts that were discussed and offers the official documentation as a source of additional information for those who want to learn more.

Developing Your Writing Style
---

*Borrowed thoughts, like borrowed money, only show the poverty of the borrower.* - Lady Marguerite Blessington

All authors come to develop a style, a "voice", that is distinctly their own. As you develop yours, keep in mind that understanding technical concepts can be hard enough as it is so it's best to use simple language; it's easier to read and understand than flourishy prose. 

### Use Simple, Informal Language

Understanding technical concepts can be hard enough as it is, so it's best to use simple language when writing because it's easier to read and understand than flourishy prose. 
Here's an example that's overly prosaic, adapted from [Flexible View Manipulation, Part 2 – Using Decorators](http://www.sitepoint.com/flexible-view-manipulation-2) by Alejandro Gervasio:

    For years we've been so busy parroting here and there about the heaps of virtues and drawbacks exposed by the model/controller tandem that this never-ending verbiage of nerdy gossip made us unintentionally bastardize the role of views, downgrading it to the level of just a clunky HTML template.

The above can be rewritten with most of the exaggerated verbiage removed. The phrase "parroting here and there" can be replaced with "discussing", the descriptive "heaps" is unnecessary, etc.

    For years we've been so busy discussing the virtues and drawbacks of the model/controller tandem that we've overlooked the role of views, denigrating them to the level of clunky HTML templates.

The revision is clearly more readable and still retains the essence the author intended.

### Don't Duplicate the Documentation

When writing an article discussing a particular library or API, It's easy to write something that in the end resembles documentation. Method X does action ABC, method Y does DEF; we all know documentation isn't interesting to read!

Consider structuring such articles around something fun you've done with the library or API instead. The documentation already explains how individual methods work, so if you instead show how the methods work together to accomplish a specific task you'll have written a more interesting article.

### Plagiarism

Plagiarism is including the work of others in yours and passing it off as your own, either intentionally or unintentionally. Plagiarism has been viewed differently throughout history but the modern view perceives plagiarism as dishonest.

Here's an example I've constructed using an excerpt from Callum Hopkins' article, [Why You Should Use Bcrypt to Hash Stored Passwords](http://www.sitepoint.com/why-you-should-use-bcrypt-to-hash-stored-passwords): 

    Bcrypt is incredibly slow to hash input compared to other functions. How much slower is Bcrypt than, say, MD5? Using a work factor of 12, Bcrypt hashes the password "yaaa" in about 0.3 seconds on my laptop. MD5 on the other hand takes less than a microsecond. Don't think Bcrypt sounds like it would be too slow to use, though. You can set how large you want the cost of your hashing to be. This means you can sacrifice time and go for all-out-security by using a huge Key Factor, or you can use a minimum Key Factor and reduce the time it takes to hash the input value.

And here's the real excerpt showing proper attribution:

    Bcrypt is incredibly slow to hash input compared to other functions.  Consider this quote from Coda Hale's article How to Safely Store a Password (bit.ly/dlRWpc):

    > How much slower is Bcrypt than, say, MD5? Using a work factor of 12, Bcrypt hashes the password "yaaa" in about 0.3 seconds on my laptop. MD5 on the other hand takes less than a microsecond.

    Don't think Bcrypt sounds like it would be too slow to use, though. You can set how large you want the cost of your hashing to be. This means you can sacrifice time and go for all-out-security by using a huge Key Factor, or you can use a minimum Key Factor and reduce the time it takes to hash the input value.

Proper citation lets readers know what are your words and what are the words of another. Giving credit where credit is due is not only fair, but it also makes sure that your unique voice is heard and not the voice of another.

For more information on plagiarism, visit [plagiarism.org/plag_article_plagiarism_ faq.html](http://plagiarism.org/plag_article_plagiarism_ faq.html).

Working with your Editor
---

*To write well, express yourself like the common people but think like a wise man.* - Aristotle

Your editor is your primary contact and advocate so never be afraid to ask him questions if you don't understand something. He is responsible for managing authors and ensuring published articles are clear, correct, concise, complete, and consistent. It's the editor's job to ensure all submissions meet a level of quality before publication. If your article doesn't meet your editor's expectations then he'll send it back to you with changes and constructive feedback to help you improve it.

Whenever two or more people work together though there is the potential for friction, so here are some tips to avoid common misunderstandings and help foster a positive working relationship with your editor.

### Tips for Working with your Editor

 * Keep in mind there is one editor to many authors. Your editor will try his best to help you grow as an author but may not always be available for hand-holding. Always submit the best possible draft you can.
 * Be sure to meet your deadlines. Sometimes things happen in your life that will require your attention and will cause you to miss a deadline. Your editor will be understanding, but be sure to email him and let him know so he can make other arrangements if necessary.
 * You can expect your editor to respond in a timely manner to your emails. 
Remember to return the courtesy.
 * Always remember that criticism is not a personal attack. The editor is only trying to help you produce the best article possible. If you have a disagreement with your editor over a particular example or explanation, ask him for clarification and try to understand his point of view.
 * Read through your article before submitting it to make sure it has an introduction that clearly identifies the purpose of the article and a summary/conclusion that reinforces the key points that were discussed.
 * Editors are people too! Feel free to friend your editor on Facebook or follow him on Twitter, start an email conversation, say hello to him at a convention, etc. (But no creepy stalking!)

Additional Advice
---

*We are all apprentices in a craft where no one ever becomes a master.* - Ernest Hemingway

Following a tried and true writing structure and corresponding with your editor can sometimes be the easiest of part writing; the biggest challenge for an author can be to overcome self-doubt. Have you ever said to yourself any of the following?

 * I can't write that much.
 * I can't explain concepts so others can easily understand them.
 * People aren't interested in what I have to say.

Yes? Stop it! You're only setting up obstacles for yourself on your path to success and self-made obstacles are the hardest of all to overcome.

### Article Length

It's true articles are expected to be a certain length, but they're not novels. An online article should be between 500-1,500 words. Typically, 500-600 words is sufficient when writing an editorial/opinion piece, and 1,000-1,500 words is good for technical/how-to articles. 

Anything beyond 1,500 words should be broken up into a series of articles because it becomes too much to digest in one sitting, but always ask your editor first before submitting a series to make sure there is enough room in the publication schedule for it. And if you're having trouble reaching your word count goal, don't hesitate to ask your editor for suggestions on what you can add.

### Yes, You CAN Write

If you're worried you can't write, it may help to think about how much writing you already do on a daily basis – writing emails, chatting over instant messenger services, documenting APIs, even updating Twitter and Facebook statuses. You've already proven you are capable of communicating effectively with others through writing without even realizing it!

If you're writing in a language other than your native language, you may want to try writing in your native language first and then translate the article into the target language afterward. Writing in a language you're comfortable with can help alleviate some of the stress and fear about making grammar mistakes and frees you up to focus on writing good content and clear explanations. It's easier for your editor to correct grammar and phrasing than poor content.

### Understand your Audience

Above all, always keep your audience in mind. They're programmers, just like you, looking for ways to solve everyday problems and grow in their craft. Share your experiences with them as only you can; they want to hear what you have to say!

If you have an idea for an article that you would like to read but you genuinely don't have the skill level needed to write about it, suggest the topic to your editor. He might maintain a small wish list of topics just for this reason and might be able to find another author who has the skill set and is willing to write. Perhaps later, when you've gained experience yourself with the topic, you can write a follow-up article to share with others your own pitfalls while learning.

In Closing
---

*Put it before them briefly so they will read it, clearly so they will appreciate it, picturesquely so they will remember it, and, above all, accurately so they will be guided by its light.* - Joseph Pulitzer

Writing is supposed to be fun and rewarding. These guidelines offer you a way to minimize some of the frustration that authors often experience when writing. You've learned about the essay-structure and how it offers you a framework in which to organize your content in an accessible manner, how to foster and maintain a positive working relationship with your editor, and a handful of ways to encourage yourself when filled with self-doubt.

The Internet of course is filled with resources to help new writers which you may want to look at as well. Here are a few to get you started:

 * [5 Ways to Overcome Self-Doubt while Writing](http://www.bradsreader.com/2008/11/5-ways-to-overcome-self-doubt-while-writing)
 * [Advice to Writers](http://www.advicetowriters.com)
 * [Applying Writing Guidelines to Web Pages](http://www.useit.com/papers/webwriting/rewriting.html)
 * [Better Beginnings: How to Start a Presentation, Book, Article, ...](http://headrush.typepad.com/creating_passionate_users/2006/10/better_beginnin.html)
 * [Guide to Writing a Basic Essay](http://lklivingston.tripod.com/essay)
 * [General Writing Resources (Perdue Online Writing Lab)](http://owl.english.purdue.edu/owl/section/1)
 * [How to Write an Outline](http://www.writeexpress.com/writing-outline.html)
 * [How to Write for the Web](http://www.ojr.org/ojr/wiki/writing)
 * [Missing Manual Author Guidelines = Top Rate Advice](http://davidbarneswork.posterous.com/the-missing-manual-author-guidelines-top-rate)
 * [Plagiarism - Explained by Common Craft](http://www.commoncraft.com/video/plagiarism)
 * [Plagiarisma.net – Free online plagiarism detection software](http://plagiarisma.net)
 * [Tips for Dealing with Your Editor](http://freelancewrite.about.com/od/editorsandagents/qt/editortips.htm)
 * [Tips on Working with Your Editor](http://www.stinalindenblatt.com/2011/07/guest-post-tips-on-working-with-your.html)
 * [What Does a Managing Editor Do?](http://www.wisegeek.com/what-does-a-managing-editor-do.htm)

