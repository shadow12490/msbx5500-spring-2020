# Lab 1

# Learning Objectives

* review how the job market looks
* get feet wet with python jupyter notebooks and the insanity that is the current landscape of the new hotness for the same
* get good at talking about business analytics with people who have no idea, and also with people who have some idea
* practice learning things on your own, together


# Deliverables for this lab

There are check-boxes throughout this document next to "deliverables." In whatever you submit, mark the deliverable as "completed" by putting an `x` between the open
brackets in the raw markdown. Like so: `[x]`.

Subject to change, let's try having you copy the contents of this file into a markdown file in your own repo. Edit your copy.

- [x] Repo copied to desktop.

# Getting un-stuck

If you get stuck with any overwhelming class, use the "think-aloud" protocol (look it up) with yourself. Write out your feelings, write out what you're confused
about, write about your immediate and mid-range project goals. Good grammar is not important here. Just give an outlet to your mind.

Also look into Rubber-Duck Debugging.

You are welcome to ask me to attempt to think-aloud myself.

If you get stuck, open an issue on the class github repo. 

Or, if you'd like me to comment on your work, you could ask me to review a PR that you create on a github repo that you own.



# Tooling


## Github

### Create a github account

Create an account. Old people say "if you want a job, you must make a good LinkedIn profile." I say pfft. Make a good github (or other hosted code repo) 
profile instead and sk8 or die.

* Set a nice profile picture for yourself.
- [x] done
* Set your name and organizational affiliation
- [x] done


### Join the class github stuff

1. From canvas, get a link to the class github "team", and join/request to join it.
1. Once you are a member of the team, you can view the class repo, linked on canvas.
- [x] done 

### Make a personal repo for your work for this class

* add me `deargle` as a collaborator. You can fork the class repo. Or not.
- [x] done, deargle added as collaborator on new fork 1/22


### Create a stupid-easy online web presence.

Jekyll is static-site generator, written in Ruby. GitHub Pages integrates with Jekyll. GitHub Pages will auto-render your repo into html files. You can select a theme, for minimal fuss and muss.

Make a [GitHub Pages](https://pages.github.com/) site. You can make either a "personal" page or you can make a "project" page. Make either one. Which one you make depends on what name you give your repository.

If you follow the steps above and make a "project" page, then the instructions will include a way for auto-using a jekyll "theme" -- and it will also generate a default index.md file for you. Try both! Ask questions
on the class repo if your feeble mind can't grasp the schnazzy of this.

Here I am, documenting everything I told you you'd have to figure out for yourself. Go figure out the rest!

- [x] stupid easy web presence is set up 1/22
- [ ] make web presence a little less stupid easy

### Learn Markdown

Markdown is life. You can use markdown on Github, amongst other places. Check out [this github guide](https://guides.github.com/features/mastering-markdown/) to github-flavored markdown.



### Learn Git

Okay, you can just use the [GitHub Desktop](https://desktop.github.com/) client, although warning, I have no idea how it works. But you should eventually learn `git` for terminal if you're l33t.


- [x] *Deliverable:* Show me a GitHub Pages-hosted website -- both the live version, and also the markdown source code. I dunno, have fun.


![](../images/github_pages_ss.png)
* source code/repo: https://github.com/shadow12490/shadow12490.github.io


## Jupyter

Jupyter is everywhere. I want you to try it in several places.


### Jupyter via Anaconda

Anaconda is a python distribution with science-y python libraries pre-compiled and ready-to-go. Very very complicated to compile some of the science-oriented python libraries on Windows otherwise.

Install it!

- [x] Anaconda installed [eventually] (1/22)

Then, using Anaconda Navigator, install/launch ~jupyter~ JupyterLab. JupyterLab looks like Jupyter 2.0. Might as well go with the new hotness.

You are now running jupyter on your laptop. 

- [x] JupyterLab launched from my laptop (1/22)


### Jupyter lots of other places

But there are many other places that will let you run jupyter notebooks on their infrastructure. Let's visit and dabble with each of them so that we can say we did.

* [Amazon SageMaker](https://aws.amazon.com/sagemaker/) 
  ([Do this tutorial](https://aws.amazon.com/getting-started/tutorials/build-train-deploy-machine-learning-model-sagemaker/))
	* **UPDATE:** When you get to **Step 5a** in the tutorial, the AWS given code will throw an error like this: 
		```javascript 
		Using already existing model: xgboost-2020-01-28-06-25-08-731
		ResourceLimitExceeded: An error occurred (ResourceLimitExceeded) when calling the CreateEndpoint operation: The account-level service limit 'ml.m4.xlarge for endpoint usage' is 0 Instances,
		```
		According to [this solution](https://stackoverflow.com/questions/53595157/aws-sagemaker-deploy-fails/), the AWS free tier only runs Machine Learning models on instance type = "ml.t2.medium". The given code on the AWS tutorial uses instance type = 'ml.m4.xlarge" which results in the error posted above. To clarify, use **this** code instead for Step 5a in the tutorial:
		``` javascript
		xgb_predictor = xgb.deploy(initial_instance_count=1,instance_type='ml.t2.medium')
		```
* [Google Colab](https://colab.research.google.com)
* [Microsoft Azure Notebooks](https://notebooks.azure.com/)

- [x] **Deliverable:** Demonstrate somehow that you've used each of these notebook services.
- screenshots below:

![](../images/pt_sagemaker_ss.png)
![](../images/pt_colab_ss.png)
![](../images/pt_azure_ss.png)

Kaggle also has hosted jupyter notebooks. [Kaggle also has good python-for-datascience tutorials](https://www.kaggle.com/learn/). Do the first seven (!) or so -- up to the TensforFlow one. These will take a while, but should be very good get-feet-wet introductions.

- [x] **Deliverable:** Show me somehow that you've gone through all the kaggle tutorials. Get as far as you can. Take notes on what you'd like to talk more about.
- Done, made it through at least all the tutorials, with notes in OneNote

![](../images/kaggle_tutorial_progress.png)


## Job Market

Check Canvas for our collaborative Google doc. Help keep that doc up-to-date with good (1) search query tactics for each site (key terms, filters, etc), as well as (2) good job postings for the greater Denver
area. Also keep notes for yourself, in whatever form you like. Both the shared document and your personal notes should be living documents -- keep them up to date through your job search process.

What job requirements stand out to you in the postings that you see:
* what requirements can you _demonstrate competency in_ already?
* what requirements can you _speak intelligently_ about?
* which requirements do you think you already have within-reach?

* what tentative goals do you want to set for yourself for this semester for how to become a stronger job candidate?

Which jobs are the most interesting to you? Why?

- [x] **Deliverable:** Show me what method you are using to manage your job search process.

* I use an excel sheet that tracks applications, job titles, and dates, but I don't have that set up for my full time search just yet. (1/22)

# Gain Knowledge and Become Conversant in...
It is Very Important to not sound and look like an idiot when talking about business analytics in e.g. interview or networking settings.

After this lab, you should be _conversant_ in the following areas. Deliverable: write up little elevator-pitch-length responses to questions such as the following.


* [x] read the chapters from the Business Analytics book that will help you answer questions such as the following:
	* [x] what is business analytics?
		* Business analytics is the umbrella term covering a field focused on understanding past business data to gain insight. The process of collating, sorting, processing, and studying business data to transform it to "business insights" [Source](https://www.microstrategy.com/us/resources/introductory-guides/business-analytics-everything-you-need-to-know)
	* [x] why learn about business analytics if the job role won't be an analyst -- what job roles involve analytics?
		* It's important to have an understanding of what would be going on in your business analytics world, especially if you were required to communicate with an analytics team. Mostly so you don't sound like an idiot when they use "technical" terms, but also because everyone dabbles in "analytics" in some way shape or form.
	* [x] what is predictive analytics? what is supervised analytics, and what is unsupervised analytics?
		* **Predictive analytics** - the practice of extracting information from existing data sets in order to dtermine patterns and predict future outcomes and trends.
		* **Supervised vs unsupervised analytics** - supervised refers learning techniques to find the relationship between independent variables and dependent output variables. Unsupervised refers to learning techniques that group instances without a specified target attribute. Source: book
	* [x] what is a target? what are features? What are dependent variables, and independent variables?
		* **target** - also: dependent variable - the variable your model is trying to predict
		* **features** - also: attribute - quanitity describing an instance. Has domain defined by the attribute type. Common types:
			* categorical - finite number of discrete variables
			* continuous
		* **independent var** - also: features - input variable
		* **dependent var** - output variable, result
	* [x] what is a model?
		* **model** - structure and corresponding interpretation that summarizes (or partially summarizes) a set of data for description or prediction. Examples: classifiers, regressors, inputs, etc.
* [x] what is jupyter, how does it relate to python, where can one find a jupyter, contrast with anaconda and local notebooks
	* Jupyter Notebook - an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text
		* It relates to python because notebooks can be written in the python language. 
	* Anaconda - platform/toolset with tools for data scientists. 

* [x] what is AWS, what is sagemaker, how does it compare with google Colab
	* AWS - Amazon Web Services
		* Sagemaker - a fully managed service that provides every developer and data scientist with the ability to build, train, and deploy machine learning (ML) models quickly
		* Colab - Google's free online Jupyter notebook environment
