 I'm Building a GitHub for Writers (madebyloren.com)
311 points by guynamedloren 2 years ago | 146 comments
[http://madebyloren.com/github-for-writers]


Comment by crazygringo 2 years ago: [6296836]
A lot of programmers already find it awfully hard to wrap their heads around how
git works. I can only imagine how hard it will be for non-programmers to (it
doesn't suprise me that the successful example used is written by
_mathematicians_).

HOWEVER, that doesn't mean it can't be done. In fact, if there are ways to
visually simplify git and make it more intuitive for non-programmers, those
techniques could wind up making git even better for programmers too.

I could also imagine a convergence of the git model and the wiki model someday
-- where anyone can edit (like Wiki), but where there are branches, merging,
etc. Obviously, a lot of internal wiki's don't need such complicated version
control, but for things like Wikipedia, it could be amazing.

I think there are a _lot_ of areas for working on writing collaboration -- group
projects in school, business proposals, technical manuals, all sorts of things.

And the main attraction for users over, say, Google Docs, is that _your changes
don't overwrite others'_. The fact that your edits create a "branch", that then
others can accept/reject/modify/merge, is a vast improvement in creative
collaboration.


    Comment by malandrew 2 years ago: [6297277]
    Learn Git Branching did a really good job of making git easier to
    understand:

    [http://pcottle.github.io/learnGitBranching/]

    If you take that approach and update with precise but plain english
    vernacular (redundant?) and domain specific examples, then you are halfway
    there to making it understandable by regular people.

    The most important thing to help people really get it is to promote small
    commits to their work. The real value of git only makes sense when you start
    making small commits. Having worked as an editor in a past life, having
    something like cherry-pick and interactive rebase would have been most dope.
    In a way, maybe editors are the best audience for driving adoptions among
    writers in general. For professional editors, version control is a
    painkiller. For writers, it is a painkiller if the writer is an obsessive
    editor. For those who write and commit once, but don't go back and review
    commits and refactor, it doesn't provide much value.

    Think about how Apple Time Machine made a stab at operating system backups
    and snapshotting. Was it perfect? No. But it was a step in the right
    direction.

    Loren and others may not solve all the problems right out the gate, but they
    will lay the groundwork for new approaches to teaching version control to
    writers and other audiences.


        Comment by Walkman 2 years ago: [6298386]
        Learn Git Branching is best learning tool I ever tried! With this tool
        and a little practice on the side I was able to learn the basics of git
        within a couple of hours so that I can confidently branch, merge, push,
        pull and rebase and I know what I'm doing! Programmers should invert
        more learning tool like this!


        Comment by AlexSolution 2 years ago: [6298163]
        Love this site. Hoping people contribute a few more lessons to it in the
        near future.


            Comment by xxbondsxx 2 years ago: [6299868]
            Thanks Alex! I'm working on some lessons around push / pull / rebase
            right now that I think will be super helpful for learning the next
            steps.

            Progress has slowed a bit since work has ramped up, but now that
            intern season is over I'm expecting to make some progress


        Comment by edraferi 2 years ago: [6297596]
        learnGitBranching is a fantastic resource that I didn't know about.
        Thanks!


        Comment by dalek_cannes 2 years ago: [6300274]
        Whoa! Now _that's_ how you teach anything command-line to non-
        programmers. Someone should do something like this for unix commands and
        the like.


    Comment by guynamedloren 2 years ago: [6296942]
    > _In fact, if there are ways to visually simplify git and make it more
    intuitive for non-programmers, those techniques could wind up making git
    even better for programmers too._

    That's the goal.  I want git to handle everything behind the scenes, and
    everything that the user touches just 'makes sense' - ie its not all that
    different from what they're already doing.  A 'save' button makes a git
    commit, editing somebody else's content automatically creates a new branch,
    'submitting' that content on the new branch creates a pull request .. etc.


        Comment by terrycb 2 years ago: [6300433]
        This is a really fantastic idea. I can also imagine writers will get a
        great deal of use out of git cherry pick.


        Comment by dylangs1030 2 years ago: [6300211]
        You could combine the advantages of git versioning with wiki style
        collaboration and make a git-wiki like the parent said, but for writers.

        Wikipedia is largely prose, but of a nonfiction variety. This would be a
        good intersection for git, which was born out of code.

        You could call it..."geeky"...too bad it wouldn't be for geeks.


    Comment by nwhitehead 2 years ago: [6297206]
    The intersection of git and wikis is interesting, it's one of those things
    that sounds compelling but then the details usually end up making it hugely
    complicated. Worth thinking about.

    For general writing collaboration I would seriously consider not allowing
    arbitrary branches. Most people just get confused managing multiple
    independent outstanding branches that potentially branched from different
    points in the history.

    One restriction could be that each user gets a single branch (their
    suggested change). As changes get merged into HEAD each user's branch must
    be rebased (with a click) before they can add more changes to it. From a
    programming point of view this is restrictive; why can't I suggest two
    independent features? But keeping track of dependencies is precisely what's
    hard for people.


        Comment by guynamedloren 2 years ago: [6297325]
        > _For general writing collaboration I would seriously consider not
        allowing arbitrary branches. Most people just get confused managing
        multiple independent outstanding branches that potentially branched from
        different points in the history._

        Yep, absolutely true.

        > _One restriction could be that each user gets a single branch (their
        suggested change). As changes get merged into HEAD each user's branch
        must be rebased (with a click) before they can add more changes to it._

        Heavily considering this approach.


    Comment by gcr 2 years ago: [6299208]
    Honestly, I think writers could benefit more from the collaborative editing
    model than the git branching model.

    When do writers need to branch their stories/articles into two forks? If
    they do that, why not just copy the document and work on it there? The large
    bodies of text don't have the filesystem dependence that programs do; it
    doesn't matter what the manuscript is called if nothing #include s it or
    require()s it.

    Instead, it can be quite valuable to have a collaborative text editor: your
    colleagues' changes are shown in real time as they make them. If you go on a
    plane ride, they're synced when you get more internet access, with conflicts
    clearly shown and deliminated so you can resolve them simply.


        Comment by jtheory 2 years ago: [6300297]
        My wife is a novelist.

        The collaborative editing would be useful in the later phases of a book
        -- i.e., working with an editor and copyeditor, it's be great to have a
        really efficient way to review changes made to the actual text (instead
        of reviewing a hard-copy with hand-written corrections, and then hoping
        those corrections are accurately hand-merged into the text...).

        But for most of the life of a manuscript, it's just the author working
        completely solo (from what I've seen).  In the standard flow, there's no
        editor until the book (in a fairly complete and polished draft) is sold
        to a publisher.  A literary agent may read drafts along the way, but
        normally wouldn't touch the text, just write up higher-level feedback.

        On the other hand, the task of designing a narrative that flows well at
        the scope of a novel is really hard, and can take a lot of large-scale
        trial and error to improve.  She usually _does_ have several "branches"
        of her current project, as well as large chunks that she has cut from
        the current draft but doesn't discard (and sometimes may be re-added).

        Her first published novel shed more than 300 pages that were never re-
        added on its way to the final version... it's hard to keep track of all
        that.  It wasn't like "drop this chapter", generally, more like "remove
        this subplot from the hundred or so places it shows up".

        I'm not sure how well the git model would address the problems -- the
        big problem is scale, and visualizing large structures made up of lots
        and lots of tiny little words.  They are plenty of pain points worth
        attacking, though, except that most writers don't have much cash to
        spend on tools.


            Comment by sdoering 2 years ago: [6300515]
            For something like that you would need a way to mark parts of text,
            that deal with certain subplots/plots. Like different colors for
            different plots, but what happens, when they intersect? Or you could
            use flags, or something like that.

            An easy way to trace a plot throughout the novel. Interestingly, a
            tool, that enables this could even be used by literature students,
            when analyzing texts for an interpretation (been there, studied
            that). The only problem with this is copyright and the inability to
            get your hands on a digital os-/reader-independent format, to work
            with in the first place.

            I worked mostly with texts from medieval times and it was a pain to
            get hold of (good) digital versions. May be, that this is because
            language processing approaches are not that widely used in my former
            field of study.

            So to wrap it up - a great tool, enabling authors with this could
            enable also a better understanding of novels for literature students
            alike.


    Comment by jonnathanson 2 years ago: [6297829]
    _"And the main attraction for users over, say, Google Docs, is that your
    changes don't overwrite others'. The fact that your edits create a "branch",
    that then others can accept/reject/modify/merge, is a vast improvement in
    creative collaboration."_

    This.

    Version control is a capital-P Pain In The Ass for group writing projects.
    Anything that improves the version control problem in collaborative writing
    solves a very real need. Perhaps not a huge TAM at first glance, but a real
    need nonetheless.


    Comment by alightergreen 2 years ago: [6300132]
    Haha! Agreed, but like lots of software things--I think that's mostly
    because the instructions are written by the programmers. I'm management at
    my company (don't code), but have never had trouble grasping the conceptual
    issues and intricacies of code, and that makes me really good at teaching
    it. You just have to contextualize it properly for their perspective.
    Writers, or anyone that's not a programmer, doesn't care what a git is or
    how it work technically. They want to know how it will fulfill their
    wants/needs, and they want big buttons labeled with those solutions. I could
    teach my grandma to use to the github client if there was a shortcut to it
    on her desktop.


    Comment by etler 2 years ago: [6298170]
    I love git, but some of the metaphors and inconsistencies it makes are
    definitely not good and make it much harder to pick up than it should be. I
    think with the right set of metaphors and ui it can work.


Comment by babuskov 2 years ago: [6296783]
I was looking for something like this. I'm planning to write an epic sci-fi
novel and make it available under some open license (Creative Commons BY-SA
probably). Since I'm not a native English speaker, I'm hoping those who are
would jump in and help me perfect the text.

My final hope is to see a Hollywood movie made out of it one day, because many
recent SF movies lack good story.

My other idea is to make the story branch into different directions. I would
write the main storyline, but another writer could come and fork it at some
point. The reader would be left with a choice at some point: would you like this
character to take that decision or the other - and after choosing, the reader
could read the forked variant.

This is the first time I'm publicly writing about this idea. I'm still undecided
what technology to use to create it.


    Comment by thirdtruck 2 years ago: [6297988]
    I'm cheering you on, babuskov!

    I've used git with my sci-fi novel, Planet Oz, since I first drafted it back
    in 2008. Quite glad I did since it makes the editing process much easier to
    track.

    Can't wait to begin the Kickstarter in October.


    Comment by kybernetikos 2 years ago: [6300761]
    > I'm still undecided what technology to use to create it.

    I've got friends working on projects a bit like this.  Markdown served from
    github pages is nice, as you edit and compare diffs in markdown, but you can
    get it automatically rendered into a nice readable form too.

    My own view though is that the most likely way to fail is to  lose
    motivation, and having interminable discussions over minutia early on while
    writing is likely to suck away your energy.  I'd probably get at least the
    skeleton of the whole story into your repos before encouraging others to
    contribute.


        Comment by babuskov 2 years ago: [6301001]
        Yep, the skeleton for the whole story is ready. I have been pondering
        about all those main story parts in the past 2-3 years. My next step
        would be breaking each chapter into smaller parts, without writing down
        any specific sentence. The last part of the process would be actually
        writing it.


    Comment by maxerickson 2 years ago: [6297188]
    Have you looked at Z-code? There's lots of reasonably modern interpreters
    for it and there seems to be a fairly active community.


        Comment by babuskov 2 years ago: [6297516]
        No. I just googled now, but there seems to be a lot of stuff named
        Z-code and I'm not sure what exacly am I looking for.

        Can you give me some URL?


            Comment by VikingCoder 2 years ago: [6297712]
            I think Max is talking about the Z-Machine interpreter that Infocom
            created to make games like Zork and Hitchhiker's Guide to the
            Galaxy.  There are many of modern ways to use it, like Inform (I
            recommend Inform 6 over 7), and even a web interpreter, Parchment.

            That's if you want someone to PLAY the choice in the story.  Which
            is slightly different from what you're talking about.


                Comment by maxerickson 2 years ago: [6299532]
                Yeah, the Z-Machine interpreter. But I think it is reasonable to
                look at choose your own adventure as a fairly straightforward
                game, so Z-code presumably provides the necessary features for
                it.


    Comment by Blahah 2 years ago: [6297417]
    Git branching a storyline is an awesome idea.

    I'd love to know when this book gets off the ground - I enjoy both sci-fi
    and correcting other people's English.


        Comment by babuskov 2 years ago: [6297500]
        Thanks, I'll take you up on that. I assume that the e-mail in you HN
        profile is valid?


            Comment by Blahah 2 years ago: [6301326]
            Yup - look forward to your email.


        Comment by atmosx 2 years ago: [6298427]
        Cool, I know whom to call for reviews :D


Comment by tptacek 2 years ago: [6296900]
This is sort of what Nate Kontny is doing with Draft, which I like kind of a
lot, much more than I expected to.


    Comment by spartango 2 years ago: [6297859]
    Draft's editing/version control is rather awesome and easy to use. It would
    be neat if Loren and Nate could work together to get some of the github-like
    "social" features into Draft--following updates and broadcasting progress.

    My feeling would be that having one platform with both features would be
    better than having two very similar things here.


    Comment by emhart 2 years ago: [6297179]
    I've been loving draft to the point that I haven't really engaged with any
    of the other new platforms out there, like editorially. I sign up to beta
    just about any of them that come along, but Draft just feels like home
    already. That said, I can't imagine I wouldn't at least play around on the
    platform the author describes.


    Comment by Shank 2 years ago: [6297617]
    My biggest issue with Draft is consistency in behavior. Personal anecdotes
    are frowned upon here, but for most of last week the ability to export files
    wasn't working at all for me. When I'm dealing with Markdown, this is the
    last thing I want to happen.

    I much prefer a system that's geared to projects and not specific types of
    document too. For example, if this supported housing a collection of
    documents and an image or two - with changes able to be made on each file,
    it would be amazing. Google Docs I edit with others quickly tends to devolve
    into three different types of sharing/permissions issues, and I'm left
    frustrated or wondering why some people can access one thing or another.

    There's definitely room to innovate here.


        Comment by guynamedloren 2 years ago: [6297644]
        > _I much prefer a system that's geared to projects and not specific
        types of document too. For example, if this supported housing a
        collection of documents and an image or two - with changes able to be
        made on each file, it would be amazing._

        Nailed it.  That's what I'm building :)


    Comment by artgon 2 years ago: [6297606]
    Agreed. Draft tackles versioning and editing in markdown very well. The
    incremental save feature makes all of this transparent to the writer.


Comment by dylandrop 2 years ago: [6298372]
This is interesting, but I think it kind of fails to take its audience into
consideration.

1) It assumes writers write like programmers code. This isn't true. At least
with scripts, what typically happens is the writer will write an entire script,
send it to their boss for revisions, and then rewrite it. They would consider it
a pain in the ass if they had to make "commits" for every page they wanted to
add, and especially if their bosses had to review each change (mostly because
bosses are executives who just want to leave their mark by making unnecessary
changes on things).

2) In either book or script writing (or whatever) small grammatical changes are
unimportant, and there will be way more of these than we would care to look at.
Who cares about reverting a change of "its" to "it's"?

I see this kind of thing as being useful for writing an informal, informational
book in the form of an extended blog post (see
[http://gettingreal.37signals.com/]) but otherwise, I can't really see it being
that useful for professional writers.

Also, something that I think would be REALLY useful (that I'm honestly surprised
I haven't seen is a Final Draft - meets - Google Docs (screenplays editable by
multiple people via online, all stored online). Dunno if anyone's seen anything
like this.

Sources: My dad is a TV writer.


    Comment by cauthonLuck 2 years ago: [6300296]
    Scientific writers do write like programmers code. There are as many as ~15
    authors on a paper. The scientific paper has intensive markup, often in
    Latex. And collaborative writing like GoogleDocs doesn't work b/c 3
    different authors will make changes to the same sentence and you need to be
    able to see all three changes next to each other. Not to mention figures,
    equations, etc...

    MS Word and Libre office aren't powerful enough for scientific writing and
    aren't universally embraced or consistent across operating systems.

    Github for writers is desperately needed. Draft doesn't do nearly enough

    Source: physical science graduate student


        Comment by natejenkins 2 years ago: [6300423]
        Hey, I'm working on a similar project for scientific writing.  You can
        find the link in my profile along with my email.

        We have had success with large collaborations working on it, 15 authors
        should not be a problem.

        Check it out and feel free to contact me.


    Comment by baby 2 years ago: [6299838]
    Exactly. I don't care about the document progression or the changes of
    words. I just want "versions" and "notes". I actually did a writing
    application for myself only and I had two windows, one on the left with the
    actual text, one on the right with the notes, also a sidebar with the
    chapters and progression of the book.


    Comment by gcb0 2 years ago: [6298907]
    i try to get my SO to write academic essays in applications that have
    history or diff viewing... but never had any success. but that only means
    the current offerings are bad. even for programmers.

    regarding your points, when i set up `meld` to show the text she sent vs
    what her professor or coleague sent back, she is amazed. So there is
    usefulness.

    Second, have you ever used Kwrite in KDE? you don't have to commit or
    anything. just type. and it shows the diffs marks on the left. pretty hand.
    and avoid commits and all.

    about point #2, just make branches and tags more practical. Also, try to
    merge back those 'word fixes' in other branches ' heads. would be awesome
    even for programmers.

    source: optimist :)


Comment by jedc 2 years ago: [6298135]
Is it just me, or are there a number of fairly high-profile writing tools that
have launched recently?  The ones I'm thinking about:
 
  * Draft http://draftin.com
  * Editorially http://editorially.com
  * Quip http://quip.com
  * Loren's Penflip http://www.penflip.com
  * Google Docs (obviously not new)
 
A lot of thoughts running through my head, including that finally
products are being built from the ground up both for collaboration and for
mobile/tablets.  (And that this appears to be an early sign of the end of
Microsoft's dominance in the office productivity software world.)


    Comment by guynamedloren 2 years ago: [6298148]
    I'm on your 'high-profile' list!

    Made my day, thank you.


    Comment by Myrmornis 2 years ago: [6299403]
    Are any of these projects aiming to interface well with MS Word or
    OpenOffice?


        Comment by sdoering 2 years ago: [6300562]
        Well you could use pandoc [1] for creating MS Word or other file-
        formats. As far as I know MS Word is still the choice to use for
        novelists, when it comes to giving test to editors and a like.

        So pandoc could be used for transforming a text into many different
        formats (even ebook formats).

        Might be an interessting thing to look at for the creator of "git for
        writers" ;-)

        [1]: [http://johnmacfarlane.net/pandoc/]


Comment by scottfr 2 years ago: [6296861]
I'm currently using GitHub to collaborate on writing a book with a non-technical
coauthor. Generally it works great, but there are two key issues:

* Changes are tracked by line which is equivalent to a paragraph in a book. If I
go in and add a comma to a paragraph and my coauthor simultaneously changes a
word in that paragraph that can create issues.

* Errors are very difficult to solve for my coauthor. When Github Window's app
encounters an error, it basically says "Just open up the command line and you
should be able to figure out how to solve this". Of course this isn't feasible
for a non-technical audience.

If your product can fix these two issues (which it looks like it is trying to)
it could be very valuable.


    Comment by sdesol 2 years ago: [6298350]
    Disclaimer.  I'm the creator of GitSense which is working on building
    advanced power tools for Git and GitHub.

    The diffing problem is solved quite easily with the Google Diff, Match,
    Patch algorithm and our Smart View technology.  When GitSense was created,
    it was obvious that we all work differently and we all have different needs
    which was why we made it insanely customizable. If you are not familiar with
    the Google Diff, Match, Patch algorithm, you can learn more about it here:

    [https://code.google.com/p/google-diff-match-patch/]

    I've also put some screen shots of what the diff results for two markdown
    files would look like at:

    [http://screenshots.gitsense.com/google-diff-patch-match.html]

    The context aware source code that is used in GitSense to display the diff
    can be found here:

    [http://screenshots.gitsense.com/google-diff-match-patch-integration.js]


    Comment by nadaviv 2 years ago: [6296938]
    > Changes are tracked by line which is equivalent to a paragraph in a book.

    When using Markdown, I usually split paragraphs over multiple lines (usually
    between sentences) which makes diffs much easier to read, while still
    rendering as a single paragraph.


        Comment by jamie_ca 2 years ago: [6298082]
        I know people who break lines per phrase/clause, rather than per
        sentence. You wind up with lots of very short lines, but that doesn't
        matter after Markdown is done processing. The benefit is some _very_
        granular diffs that are easy to read, as you work out rewording things
        in the editing process.


        Comment by vidarh 2 years ago: [6297021]
        Same here. "Single line paragraphs" are a pet hate of mine - they have
        no place in plain text files even if those files are intended to be
        post-processed.


            Comment by breadbox 2 years ago: [6297203]
            Absolutely, but you still have the issue that a minor wording change
            can cause an entire paragraph to be marked as changed if your editor
            re-wraps the paragraph. Or, if the editor doesn't rewrap the
            paragraph, then they slowly get more and more ragged over time,
            making it annoying to read through.

            A diff tool that understands paragraphs is an essential tool for
            this project.


            Comment by gabemart 2 years ago: [6297643]
            I disagree with this. In a plain text file that consists of prose,
            line breaks are presentation, not content. Hardcoding them into the
            file doesn't appeal to me. It makes editing a pain in the neck. It
            also means the line breaks have to be removed again if you want to
            move between formats.


                Comment by gknoy 2 years ago: [6297883]
                That sounds like an editor issue, though. You should be able to
                reflow a paragraph, indent it or whatever it as you like.

                A compromise might be to break lines on sentence boundaries:
                edits are often constrained within sentence or paragraph
                boundaries, and then diff would give more meaningful output for
                most sentences.

                ^-- This one sentence is two lines long, though, so perhaps my
                idea is not that good. Diffs would still be easier to read than
                if each paragraph were one line.


            Comment by tasuki 2 years ago: [6297176]
            I'm still undecided on this. Say you have a long paragraph and have
            to add one word at the beginning. You have two options - either
            rewrap and introduce a silly diff, or don't rewrap and exceed your
            chosen text width.

            Single line paragraphs don't put such a difficult choice in front of
            you. If your diff software is any useful, it'll highlight your
            change within the line.


                Comment by gknoy 2 years ago: [6297900]
                Perhaps you could have a special kind of commit, a "text-rewrap"
                commit (similar to merge commits), which might let your diff
                presentation tool alternate between diffing lines, pararaphs, or
                the like.  I agree, the presentation layer really needs to be as
                granular as your editing team needs to be.  I __really__ like
                how Github shows the differences within a line that is
                different.


                Comment by nadaviv 2 years ago: [6299421]
                That's why I don't use fixed-width. I break lines up logically,
                usually at the end of a phrase/sentence, regardless of their
                length.


    Comment by cinger 2 years ago: [6298201]
    i write quite a bit with git, and recently brought an old collab project
    with a friend onto it.

    i do all of the git work, and i just have my friend add my edits to his
    document, then he sends it back and i diff the two for potential errors...
    he requested it be this way because he is stuck in his ways, but we've
    agreed to go full git on book two in the series...

    that said, when i first started sending him diff files we both saw this as a
    problem... my solution? i just wrote a script that i run on the diff to just
    highlight the changes made, then send him the new edited diff.
 
        -PARAGRAPH
        +PARAGRAPH
 
    becomes :
 
        -SENTENCE
          -word...word
          +word...word
        +SENTENCE
 
    ... i place git's diff at the bottom of the file in case he wants to
    look that over as well, but this cleans up the edits real nice


Comment by AndrewDucker 2 years ago: [6297186]
What I mostly want, when writing collaborative documents, isn't a git equivalent
- it's a code-review equivalent.

I want to leave comments on individual words, sentences, paragraphs, etc., with
suggestions for changes.  And that's something that git doesn't allow, because
the smallest change you can comment on is a file, with no ability to comment on
specific parts of it.


    Comment by guynamedloren 2 years ago: [6297279]
    Git doesn't support it, but GitHub does.  You can comment on individual
    lines via GitHub.  I'm going to do something similar - maybe on a more
    granular level (words/sentences).


    Comment by gamblor956 2 years ago: [6297833]
    It sounds like you're looking for Microsoft Word, which has offered this
    feature for more than a decade (albeit though not online until this past
    year).


    Comment by cauthonLuck 2 years ago: [6300329]
    Latex has line comments and since it is compiled into a document you can
    place line breaks anywhere. It does break the flow of the sentence though.

    I've used Latex+vim+git to write scientific papers recently. It is
    unfortunately much too complicated for my colleagues to adopt. They're
    holding onto MS Word which is far inferior in terms of markup, citing, and
    VCS.

    I've been converting my Latex documents to ugly word documents for
    collaborating and editing. The MS Word editing isn't great either. The
    strikethrough method breaks up flow. I've also had problems deleting side
    comments in Libre office. And the MS Word experience isn't always the same
    on Macs.


    Comment by manish_gill 2 years ago: [6297267]
    You can usually do it with shared Google docs. I know a few writers who
    share their content with a few trusted betas. It provides the necessary
    features, I think. Highlights, commenting etc.

    I think there is also a "real-time" feature that it provides (not sure about
    that), so there is usually more than one eye on the doc as the chapter is
    being typed.


    Comment by pbowyer 2 years ago: [6300485]
    I asked how this could be implemented online 2 days ago:
    [https://news.ycombinator.com/item?id=6284610]

    I believe Operational Transforms are the way to go, but I have no basis for
    that.


    Comment by JeffJenkins 2 years ago: [6297274]
    If you're using google docs for your collaboration this sort of commenting
    is built in. It's a great feature.  Almost better than collaborative editing


Comment by begriffs 2 years ago: [6297215]
I think the guys at Github do want to help non-technical people learn to
collaborate with git in areas like education, government, and literature.

Check out this interview where one of the Github trainers, Brent Beer, talks
about these ideas. You might want to get in contact with him.

[http://blog.begriffs.com/2013/08/an-interview-with-brent-beer.html]


    Comment by guynamedloren 2 years ago: [6297250]
    > _I think the guys at Github do want to help non-technical people learn to
    collaborate with git in areas like education, government, and literature_

    Yep, they're doing it, just not quickly enough :)

    Neat, I'll check out the interview.  Thanks!


Comment by stared 2 years ago: [6297839]
Take a look at "Why use version control systems for writing a paper"
([http://academia.stackexchange.com/questions/5277/]).

When it comes to diffs for text, just add "--color-words":

git diff HEAD~1 --color-words my_file.md

But I agree with other stuff, that for non-techies Git + GitHub may be to hard
to start.


Comment by joshdotsmith 2 years ago: [6296812]
I know that Michael Hartl of RailsTutorial is working on something very much
like this, but will be a full end-to-end product including things like sales.

I can't wait to see what he comes up with.


Comment by bliker 2 years ago: [6296818]
How are you solving the diff problem? Word based diffs tend to be jumpy and hard
to follow. On the other hand line based diffs do not work well for text (prose).


    Comment by guynamedloren 2 years ago: [6296854]
    Yeah, prose.io uses word diffs and it's definitely hard to follow.

    I'm doing 'fragment diffs' (doesn't really have a name) - but basically, all
    the text is displayed as you would read it (sentences and paragraphs), with
    diffs displayed inline and colored.  Added content in green, removed content
    in red - doesn't matter if it's characters/words/sentences/paragraphs - it
    all works.

    Screenshot is not the best, but something like this:

    [http://www.flickr.com/photos/madebyloren/9620674181/]


        Comment by philsnow 2 years ago: [6299168]
        Don't know if you've already thought of / planned this, but please
        please implement a side-by-side diff view.

        Code is easy enough to read in a unified diff because lines are usually
        short (unless java). Prose flows a lot more fluidly, and there is no
        formal grammar for human language. I have had the displeasure of having
        to read "redlines" (prose with inline diffs marked in red strikeout) and
        I find them completely impenetrable.


        Comment by cauthonLuck 2 years ago: [6300350]
        I'm using latex+vim+git for this purpose currently. I put two spaces
        after a period to signal the end of a sentence in Latex. Which helps me
        break the document up by sentences with vim.

        If you're using markup then encouraging the period-double-space could be
        a harmless way of easily breaking the document up by sentences


    Comment by dragonwriter 2 years ago: [6296932]
    "Sentence-based" diffs would work well for prose, but the problem is
    recognizing sentences, given the other uses for full stops. If you use hard
    line breaks at, and only at, sentence ends, you could use line-based diffs
    to do this (but this may run into editing convenience issues.)


    Comment by ??? 2 years ago: [6298992]
    [deleted]


    Comment by 2mur 2 years ago: [6296862]
    We've been working on a similar problem. Writing in markdown, pre-processing
    the saved markdown to truncate to 80 column (best fit) paragraphs and then
    diffing on the markdown.


    Comment by rzimmerman 2 years ago: [6296856]
    I think for writing, sentence-based diffs would be the most useful.


Comment by mallyvai 2 years ago: [6297786]
From @kmatzen's comments on Authorea.com: " What do you get when you combine
authors with gonorrhea? Authorea!

I like it! There are two things I would still like though. One would be page
rendering in the browser. We often have to iterate several times on a paper
adjusting figures, text, padding, etc. to get everything to fit within the page
limit. I could write the paper in this and then export it to tex, but that
defeats the purpose. The second thing is support of popular LaTeX packages. It
looks like I can upload arbitrary tex documents, but that's going to get messy
if I have to upload the same packages for every paper I'm writing.

We use github for our papers right now. Less than ideal. "


    Comment by natejenkins 2 years ago: [6301904]
    What can I say?  Naming is hard.  We initially thought to ourselves,
    "Spreading science should be fun and intuitive, like an STD. And it should
    be hard to get rid of."  Thus Authorea was born.

    Have you tried our pdf exporter to check page length?  We are trying to
    build it out to where you, as a user, don't have to worry about packages.
    If there is a journal you would like to submit to and we don't currently
    have the journal setup as an export template, please contact us and we will
    be happy to add it.

    It's funny how authors worry so much about page length and figure placement,
    and then the first thing a journal does is remove all of the formatting the
    author has put in place.


    Comment by apepe 2 years ago: [6301966]
    hi @kmatzen/@mallyvai! Adding briefly to Nate's comment (my co-founder at
    Authorea), I would like to point out that we do support many popular LaTeX
    packages. One big reason why we do not support custom LaTeX packages is that
    some of them are really intended for the printed page and cannot be easily
    ported to the web- and the point of Authorea is to create web-native
    documents, which render in the browser, first, and can then be ported to
    print formats. In other words, we support a safe subset of LaTeX which we
    can easily convert back and forth into other web formats (such as Markdown).
    Do let us know if you have a LaTeX package in mind and we will see if we can
    add it for you.


Comment by mehulkar 2 years ago: [6296714]
What about draftin.com? I use that already and I like it a lot.


    Comment by guynamedloren 2 years ago: [6296749]
    Big fan of Draft (and Nate).  It's got the version control part down, and I
    think it works well for gathering feedback on blog posts and other short
    form content, but it isn't designed for longer form content as far as I can
    tell.  It's also missing the community aspect that GitHub has, which is
    huge, as well as features that would make writing an ebook or textbook
    feasible.  Definitely a great tool though.


        Comment by spartango 2 years ago: [6297872]
        Any reasons not to work with Nate? It seems like the social stuff could
        be built in tandem with his strong editor.


    Comment by wkdav 2 years ago: [6296990]
    [https://draftin.com/] - Agreed, great.

    [http://www.roughdraft.io/] - Also, I like it.

    I don't think it's a bad idea to proceed with it, I would just find a way to
    differentiate it from what's out there.


    Comment by jms703 2 years ago: [6296885]
    ditto. simple and easy to use.


Comment by guard-of-terra 2 years ago: [6299242]
The idea is terrific but focus is all wrong. Writers don't need branches. They
don't code features in. Hell, most developers don't do stupid updates-on-branch-
then-merge-merge-suffer-merge-curse-merge commit accounting.

Writers usually write alone, what they need is: A (desktop) tool with basic
WYSIWYG markup (paragraphs, bold/italic, that sort of thing) with version
control, visual diffs, export into common formats. Maybe a pull request or two.


    Comment by cauthonLuck 2 years ago: [6300363]
    Scientific writers do need branches. When there are 10 authors on one paper
    all suggesting different paragraphs/figures/equations at different times.


Comment by chalst 2 years ago: [6297575]
I'm familiar with similar workflows.  Last week, I edited via a (private) Github
repo with a scientist client who use Emacs/ org-mode/ ediff, authoring  .org
files, editing using Git staging to create change sets and inline \NB[]{}
commands to annotate changes, and ediff/git-merge to step through and resolve
changes.

Some observations:

1.Ediff is a nice tool to use for resolving Git conflicts;

2. Org mode works very well with this workflow, provided you use one paragraph
per Unix line;

3. Latex generation can be very nice from org-mode sources, and the org-mode ->
Latex exporter allows a nicer separation of content from presentation than you
get with vanilla Latex.

I'd love to hear of anyone who has success with a similar, but vi-based
workflow.


    Comment by cauthonLuck 2 years ago: [6300378]
    I use a similar setup with vim+latex+git for chemistry articles. It works
    amazing for me. I feel like it is the most powerful presentation setup and
    most efficient editing setup currently available.

    I break sentences by ending with two spaces. (this doesn't matter since
    Latex is markup) The only issue arises when ideas span across multiple
    sentences, but I believe there is a flag for controlling the number of lines
    around a diff. (sorry, I'm new to git) But this sort of proves the point
    that an easy wrapper for git should be created for scientific writing.

    The two main problems I have are: 1. adoption by collaborators (they can't
    surmount the learning curve) 2. diffing sentences is very different from
    lines of code


        Comment by chalst 2 years ago: [6302942]
        Typical Org-mode code diffs better than typical Latex code.  This is a
        serious argument in favour of authoring in Org-mode and using its Latex
        export facility.


Comment by ozh 2 years ago: [6300751]
I'm a little late in the party but I wanted to express my feelings anyway. I
wrote a book with 2 other authors 2 years ago, and would have LOVED a tool like
this. Going over Word documents in revision mode was a colorful nightmare. In
general, having to work with Word was not the ideal stuff anyway.

To my point: to be totally useful along the whole typical writing process with
traditional publishers (authors -> technical review  -> authors -> editor review
-> authors -> punctuation/misc review -> authors -> editor) you'll need at some
point to export as Word documents. Ideally, collaborate in Git like environment,
export as Word, receive a new Word with all those colored revision and import
into Git like stuff.


Comment by jawerty 2 years ago: [6296919]
I think this is a really interesting idea; however, I don't think it's a very
good method to build it as 'Github for Writers' since coding and writing are two
very different processes. For instance, writers often create their work on their
own instead of with multiple contributions. Contributors is more of a code
project attribute, for anyone who knows how to program well can add/modify code
while not anyone who knows write well can add/modify to a story.

It is true that writers need editors but editors are certainly not writers. If
there was a system where all of the contributors acted more like 'editors'
rather than writers than I personally think it would be an awesome version
control program.


    Comment by RougeFemme 2 years ago: [6296993]
    I think this may be true for fiction (. . .writen often create their work on
    their own. . .not anyone. . .can add/modify a story), but I think it's a
    great idea for non-fiction, such as the textbook and research paper examples
    that the OP cited. Other examples include user or technical manuals,
    requirements documentation. . .The team members are often more akin to
    contributors (code or otherwise) than to editors. Individual but interlinked
    units have to come together to form a whole.


        Comment by gknoy 2 years ago: [6297926]
        Absolutely. My wife's job as a professional editor involved editing
        hundred-page documents, often with more than one author. A tool which
        made version control simple, yet writing easy, would be a godsend.

        The down side is, many such organizations (e.g., military) have
        standardized on Word, which is terrible for collaborative review,
        editing, and version control of long documents. (Of any documents?) She
        would have been extremely happy had her employer allowed them to use
        LaTeX or similar.


            Comment by guynamedloren 2 years ago: [6306326]
            > _Absolutely. My wife's job as a professional editor involved
            editing hundred-page documents, often with more than one author. A
            tool which made version control simple, yet writing easy, would be a
            godsend._

            I hope you signed up - I want to that editing process easier!


                Comment by lutusp 2 years ago: [6306330]
                > I want to that editing process easier!

                I believe that sentence no verb.


                    Comment by guynamedloren 2 years ago: [6308576]
                    Ha, woops.


    Comment by gizmo686 2 years ago: [6296979]
    One question is, do writers create their own work because of the nature of
    writing, or because they lacked the tools for collaboration. I have seen
    several examples of collaborative writing.  The first example that comes to
    my mind is the SCP Foundation [1].

    [1] [http://www.scp-wiki.net/]

    EDIT: Actually posting the link might help. (Although redacting it has a
    nice sense of irony too).


    Comment by thirdtruck 2 years ago: [6298064]
    As someone who writes software and fiction (heck, even software-fiction in
    the form of visual novels), I actually keep finding more and more parallels
    between the craft.

    I like to explain the fiction creation process as "writing code that targets
    the Human BIOS."


Comment by Doctor_Fegg 2 years ago: [6297062]
Great idea. Yes please!

But Markdown as UI... is less than ideal. It's great for hackers, but there's
already a GitHub for hackers, and it's called GitHub. No matter how much
prose.io prettifies it, you still get those damn asterisks all over the place.

Personally, I write in TextEdit, Helvetica 12pt. That's not a universal answer,
but it works for me. (Previously I used MacWrite Pro, ClarisWorks and Word 5.1
at different times, but the basic appearance was the same.) Anything that makes
a bold word look like "* * this * *" breaks 20 years of habit, and I won't do
it.

Markdown as backend storage, fine. But not as the primary editing interface.


    Comment by fian 2 years ago: [6299972]
    At work we are trialling Lyx + Subversion for collaborative creation of
    developer documentation.  The stored data is in a text + markup format which
    allows for easy diffing.  Lyx being a layer over Latex means we can easily
    transform into a wide variety of formats, but mostly we output to PDF and
    HTML.  Subversion was chosen as we already had a server available and there
    isn't really the same need to branch/merge documents compared to code.
    Writing in Lyx took a little time to get used but I definitely feel more in
    control that when trying to wrangle complex docs in Word.


        Comment by kraymer 2 years ago: [6300375]
        I used to write my documents in Lyx too but spreading the tool amongst
        my colleagues involved a lot of evangelism.  Markdown is a backend
        storage easier to adopt as developers are used to it (stackoverflow,
        github) but it produces output for the web : no pagination,
        header/footer, etc. Throw pandoc+tex template into the mix, and it
        starts to get really interesting : a quickly hacked markdown file
        transforms into nice pdf will all needed attributes. But why stop there?
        Now that you have a build process, move it to a server and add some
        hooks to injects traceability infos (author, last edit date, commit
        hash...) into the generated document, etc...

        I went down this road, and it works surprisingly well. If you're
        trialling different solution for writing technical developer
        documentation, see a more precise description of the workflow that I
        pushed on my blog yesterday: [http://kray.me/pro/doclegit-git-
        documentation-server/] (sorry for the copy quality, english not my first
        langage, corrections by mail are welcomed)


            Comment by fian 2 years ago: [6300442]
            Interesting.  When we set this up we looked at maybe adding an
            automated build (transform) step on commit via our CI (Jenkins)
            server.

            While the software developers are comfortable learning and using
            Markdown or other markup syntaxes, I eventually would like to spread
            this approach to other technical people in the company. In previous
            attempts at teaching basic scripting (Awk, Ruby, Python) to
            engineers who are comfortable writing complex logic operations in
            Excel and who can dabble in VBA - I found a lot of resistance to the
            idea of learning a new syntax.  So I expect the evangelism required
            to get these colleagues to write in Markdown will be greater than
            showing them Lyx, which at least looks like one of the editing modes
            in Word.


                Comment by kraymer 2 years ago: [6300469]
                I thought the main technical hurdle (for not dev crowd) in my
                current workflow was git as there exist a lot of good Markdown
                editors on all platforms ;)


    Comment by guynamedloren 2 years ago: [6297298]
    > Markdown as backend storage, fine. But not as the primary editing
    interface.

    That's interesting - hadn't thought about storing in markdown and just
    displaying as html.  Hmmm.


Comment by uams 2 years ago: [6296701]
The key to this one will be figuring out what features of git (and in particular
github) will make it successful in other verticals.

I wonder if some key CS concepts are so fundamentally ingrained, but that
writers think about their work flow differently.


Comment by GrinningFool 2 years ago: [6297470]
Is this going to be focused on those who use latex and markdown, or the the
broader audience of 'people who write'?

If the latter, you run into a problem pretty quickly - MS Word.  It's still one
of the most popular document editing tools out there.  More recent versions do
store content in zipped XML, but are you willing to put the work into parsing
that content at a level sufficient to let it integrate into the kind of flow you
discuss?

(EDIT: That said: if your target is those creating text-based documents, then I
think this is an excellent idea. )


Comment by cauthonLuck 2 years ago: [6300358]
How many of these options penflip, draft, etc are actually open source?

I'm looking for very specific features on the level of Latex libraries that
would never make it into a for profit application.


Comment by ??? 2 years ago: [6299110]
[deleted]


Comment by bambax 2 years ago: [6298171]
This is a fantastic idea, beautiful and beautifully simple. Of course, one can
think of a million objections to its success, but I really really hope it
succeeds!


Comment by FiddlerClamp 2 years ago: [6297564]
Have you asked a representative sample of writers whether they write this way,
and would like to use your site to write this way? Outside of business,
collaborative writing seems to be pretty minimal (I say this as a novelist)...

Also, if there could be some cross-compatibility with MS Word's Track Changes (I
know, I can dream...) that would be great.


Comment by nwhitehead 2 years ago: [6297266]
An idea is to think about rendering/typesetting as a feature. For many, getting
an environment set up to turn the project files into final files of whatever
form is a huge barrier. It would be great to have a bunch of back-end rendering
be just a click: Markdown->HTML, Markdown->PDF, Markdown->epub, Latex->PDF,
Latex->HTML.


    Comment by cauthonLuck 2 years ago: [6300385]
    especially when you throw in citations for scientific articles. Which often
    require compilation of the citation database, citation order, and citation
    insertion. Adding 3 more steps to the process.

    I've recently switched to papers to help with this. It seems to have a
    strong community and supports both MS word, libre office, and vim. Jury's
    still out though.

    [http://www.papersapp.com/papers/]


    Comment by guynamedloren 2 years ago: [6297406]
    Already done


Comment by rrhoover 2 years ago: [6298250]
Ironically, I posted a call to action to build a community for writing together.
Very curious to see how Loren's project does and how it compares to Draft and
others.

[https://medium.com/writers-on-writing/920214571e3d]


Comment by lizelfman 2 years ago: [6297605]
As a writer I'd be glad to use something like this.  I'm working on a book with
the founder of a non-profit in DC, and it involves a lot of sharing articles,
trading thoughts, and sending documents. We've been using Honey.is which is nice
for small businesses but just not as collaborative as we need it to be.


Comment by decadentcactus 2 years ago: [6299423]
This might be useful for contracts, as well. Editing points and having history,
being able to comment on specific parts etc.

Not 100% sure on how to solve the "legally binding" part if the other party
declines digital signatures, but it'd be a good way to get the contract written
and agreed on.


Comment by gt5050 2 years ago: [6296892]
This sounds great.

I am also working on something similar called Papyrus. It lets authors create
and edit ebooks simultaneously.

[http://papyruseditor.com/en/home/collaborate/new]


Comment by felipebueno 2 years ago: [6297059]
It's sad for me to see what you are doing because I had the same idea like 5
months ago. But I'm not that good on putting ideas into actions so it didn't go
that far. :(

That'd be an awesome tool for witers, bloggers, editors, etc.

Keep up the good work! =)


Comment by hyperpape 2 years ago: [6299964]
I wonder if you might prefer something like Darcs to Git. I've heard a lot of
amnbivalence about Darcs as a practical software project (just seems to be
losing momentum, and it has never matched Git for speed), but I wonder if the
model is more apt for writing than Git.


Comment by pavanred 2 years ago: [6296955]
This might be naive, but don't authors use Latex to write? So, in a sense why
can't they use github as it is to collaborate on writing?

(I guess it goes without saying, I do not have any experience or knowledge about
the writing process authors follow)


Comment by dbspin 2 years ago: [6301017]
Can't emphasise enough how important offline editing would be for something like
this. As a professional writer (whose co-written a book), you can't rely on
always having internet; but you always need to be able to work on your current
project.


Comment by zfrenchee 2 years ago: [6297161]
I wonder if Github is working on something like this.

I'm sure they're familiar with the idea and they seem like the best team to
bring it online. They're still a startup looking for growth opportunities: this
one seems obvious.


Comment by SunboX 2 years ago: [6300790]
> What's so awesome about GitHub?

It isn't all reasons mentioned in this article ... the most awesome about github
are the developers. This is the biggest reasons why a "github for writers" could
fail


Comment by based2 2 years ago: [6298733]
Wooki* is a smart tool to write documents. It let you publish them and get
reviews

[https://github.com/spreadthesource/wooki]


Comment by diziet 2 years ago: [6298079]
Do authors really collaborate as much as developers do? Wikipedia is an example
of people collaborating on writing something, but the subject matter is quite
different from the kinds of writing that gets done.


Comment by srameshc 2 years ago: [6296777]
I am trying to do the same. I never even thought about sharing this concept till
I could launch. I know for sure this a great area to work on and it will make a
huge impact for collaborative story telling.


Comment by theorique 2 years ago: [6301496]
Github works on source code, which is text files.

Writers work on English text (or other languages) which is text files.

What does this do that Github itself (or equivalent - bitbucket, etc) does not?


Comment by albertoperdomo 2 years ago: [6302082]
Just a heads up: I just tried to signup for the newsletter and got a nasty Rails
error page (500). It turns out Iwas browsing with JS turned off (using
NoScript). It worked fine after activating JS.


Comment by victormier 2 years ago: [6300953]
As I was reading all these words about project collaboration I started getting
more and more excited about the thought of myself collaborating in your project.
Until I saw it was not open sourced...


Comment by gprasanth 2 years ago: [6296887]
Just today, I was checking out the JS API wrappers for Github API v3 and I found
Github.js. There, I discovered this site called prose.io

Check it out! It's awesome!


Comment by agentultra 2 years ago: [6298383]
Github for lawyers, laws, court records, etc. I wonder how the lobbying industry
would change if there were highly-public records of everyone's additions to a
bill.


Comment by hrjet 2 years ago: [6297063]
Could this be used for other text-based documents?

I am thinking of accounting systems such as ledger-cli which let you keep your
accounts in plain text files.


Comment by rrrene 2 years ago: [6298119]
So I get the vibe that this will never be open sourced but is a side-project of
yours that (should it come to fruition) will be run as for-profit.

Am I right?


Comment by RazerM 2 years ago: [6297112]
This site doesn't work very well on mobile [http://imgur.com/opmjUGn]


    Comment by guynamedloren 2 years ago: [6297125]
    Ah I know.. I've been meaning to fix that.


    Comment by guynamedloren 2 years ago: [6306335]
    Fixed now btw.


Comment by user1241320 2 years ago: [6301402]
I thought [https://poetica.com/] was doing just this


Comment by malcolmmcc 2 years ago: [6298979]
See also [https://www.scigit.com/]


    Comment by michaelbuddy 2 years ago: [6309289]
    link fails. no https on that site.


        Comment by malcolmmcc 2 years ago: [6325219]
        huh, both work for me.


Comment by frozenport 2 years ago: [6297574]
We edit research quality publications on Bitbucket. So Git already works for
writers.


Comment by bayesianhorse 2 years ago: [6297016]
I always thought "forking" in writers is sort of frowned upon...


    Comment by guynamedloren 2 years ago: [6297058]
    Just like 'forking' code was frowned about before open source software came
    about ;)


        Comment by Thrymr 2 years ago: [6297262]
        > Just like 'forking' code was frowned about before open source software
        came about ;)

        Long after that, in fact. Forking an open source project was a desperate
        measure to free it from unresponsive/difficult/differently opinioned
        maintainers, that could leave a rift in the community for years (see
        Lucid/XEmacs). GitHub made forking something that was normal, common and
        expected.


Comment by ??? 2 years ago: [6297767]
[deleted]


Comment by thenerdfiles 2 years ago: [6298504]
Just re-purpose git-flow with a "writing/publishing" namespace:
[https://github.com/nerdfiles/Concept-of-Flat-Design#adaptation-of-git-flow]
 
    master   <->  publication
    develop  <->  draft
    feature  <->  chapter
    release  <->  edition
    hotfix   <->  redact
    support  <->  copyright
 

