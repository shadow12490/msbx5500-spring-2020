# 1/13/2020

Dave soliloquied about think-aloud protocol and rubber duck programming for
working through tough problems and writing and debugging code.

We attempted a collaborative job search but got depressed, jaded, and overly
cynical after reading the first promoted posting on linkedin under "data scientist."
Filtering the listings by experience level was somewhat helpful. Collected various
technologies that we may add to our portfolios in order to signal intelligence and
with-it-ism.

We played a bit with github, and had the students join the class "repo." Github Teams is
better than a shared private repo, because collaborators on private repos by default
all have push access to the repo, and I do not trust my students to not unintentionally
or otherwise wreck the class repo. Github Teams allows more granular access permissions.

Will meet again this week to discuss invidiual goals and progress with and for job applications,
and also to discuss potential side projects.

Triscuits were popular but seriously who eats barbeque chips at 9am. Next
time will be triscuits, apples, and cheese sticks.

# 1/15/2020

Interviews with each student during office hours. Goal was to check in with each student
about their job-search status, desires, etc. Students exhorted to have at least three-ish
actual job postings in mind, and to build out portfolio for those jobs. Dave attempted
to light a fire under proverbial students to get them to start applying _now_.


# 1/27/2020

Spent first part of class comparing notes and strategizing about job applications. Business
value / costs of false positives versus false negatives were pondered, including resumes and early rounds 
of interviews as "signaling" events. 

Second half was dedicated to sundry questions about using git and setting up a personal website using github pages,
jekyll, etc. A few questions related to the Kaggle machine learning questions were addressed.

Business analytics class midterms were posted, and students were assigned to take both. Open-notes, open feedback.
I told the students that I had them take the midterms the exams as a way to help them know some of the things
that I think a b-school data analyst graduate should know.

We talked through a Hunter Douglas case project that the students have in one of their other classes. Used it as
an example of CRISP-DM -- articulating the business question, understanding the data, understanding what modeling
can do (make predictions on what?). Discussion had good participation.

Stomach illness went around this week, beginning with Saturday previous. My individually-wrapped cheese sticks 
were wrongly accused.

# 2/3/2020

Between class sessions, one student practiced submitting pull requests to the class repo to fix lab documentation. Will
formally build pull requests into the class requirements in the future. It's important github practice.

Quick job update. Several career fairs this week, and campus visits from recruiters. Answered a few jekyll github pages
questions related to using my theme which I broke off from my site. 

Began interactive-lecture-ing at students about the all-encompassing review of all things Business Analytics. 
Notes [here](/business-analytics-crash-course-2-3-2020.md).

During office hours, began to talk about confusion matrices, ROC curves with their p-coin baselines, TPR vs FPR vs PPV,
and how those relate to AUC. Class priors, class imbalances and strategies for handling the same. Need to cover this again
next Monday.

Had intended to start with the kaggle credit card fraud dataset, but did not get to it. Want to start by next class. Also
want to give them quick ways to put up markdown versions of their R or python analyses / write-ups. Gists, .md, the like.

# 2/17/2020

*   jekyll website help.
    -   we learned that many garbage jekyll themes exist on the internet. One student paid for one, and it's pretty good. 
        Another moved to minimalmistakes, open-source and extremely configurable, and it's pretty good. 
        Before, two students were themes that were essentially broken -- usually the url insertion was wrong, missing a / in some places etc. 
        Incompatible with GithubPage. 
    -   Two students wrestled for a bit (hours) during office hours with getting Ruby installed on their machine so that they could serve 
        their sites locally. Iteration was much faster once they had that set up. Ruby version is important. WSL on windows with ubuntu makes ruby pretty easy, but
        is not strictly necessary.
    -   Another student was having troubles with his website looking weird on github but rendering normally locally. The issue was that he was not using 
        github_pages gem locally, and was using a different markdown processor, so things were not looking the same locally as on github. 
        Lesson learned was to emphasize the use of github pages gem locally
    -   A student had a similar problem where his theme was using jekyll-paginator-v2, which is not githubpages-compatible. Lesson learned was to find themes which are github-pages compatible.
    -   Takeaway is that this "easy" assignment is not easy. Flesh out a guardrails assignment that points students towards either paid themes or something vetted like minimalmistakes which are
        supported and github-pages-compatible.
*   A student asked a question about a k-nearest-neighbors R assignment from their Advanced Analytics class. Their class example had used `knnreg`, which is for regression, 
    while their homework assignment was with classification. The example code included printing the "mean" of the knnreg predictions, which threw an error for the 
    homework quiz problem because means can't be taken on binomial factors. We explored the functions' online documentation, and learned that R has (at least) 
    two libraries which provide knn -- `class` and `caret`. The function signatures are completely different. And the `class` variant can provide classification-based knn. 
    We also tried to get probability predictions from `class:knn` but after some confusion and delay we realized that the probability-estimates that it reports are relative 
    to the class that it reports as "winning" the prediction -- unlike `sklearn` where one probability-estimate is provided for each class separately. 
    Therefore we could not easily apply our own cutoff threshold. We despaired at the non-standard APIs for machine learning in R.
    -   Relatedly, I despaired that students are not reading my class-related blog posts. 
        I have decided to fail all students unless they read my blog. My class-related blog posts are a sort of textbook for the class.
*   We reviewed my analytics-class slide decks on choosing a good `k` for `k`-nearest-neighbors. This led to a discussion on overfitting, underfitting, cross-validation, etc. 
    Impromptu used slide decks from my ugrad analytics class to lecture-discuss on material. Also discussed regularization for regression -- lasso and ridge.
    -   We also briefly alluded to k-means-clustering. Many students still are fuzzy on what exactly is unsupervised machine learning.