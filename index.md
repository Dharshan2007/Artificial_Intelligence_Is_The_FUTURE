---
layout: page
title: Home
---
>"Predicting the future isn't magic, it's artificial intelligence" -Dave Waters

>"Artificial intelligence is a tool, not a threat" -Rodney Brooks

>"AI is the science of making machines do things that would require intelligence if done by men" -Marvin Minsky

---

## **The aim of this website**

This is a place where i post my journey through AI and the things I have learnt till now along with the resources I use to guide me through this spectacular journey. The projects I do will also be posted here. FOLLOW FOR MORE!

---
## **Reasons to have a website**

Before diving into the topic, lets discuss on why you should have a website of your own, regardless if you're a students like me or an entrepreneur who wants to make a name for themselves. FIrstly, your websites are a portfolio for you which displays your past achievements and it also expresses your unique talents and skills. Secondly, a website acts like a digital business card for a company: people can reference it again and again for things like contact information, names of employees, services offered and more. Last but not the least, your own websites can help you build credibility; having a professionally designed, thorough and easy-to-use website can help you to more easily convey to potential customers that you are a reputable organization, one they want to do business with.

---
## **The plethora of PROVIDERS**

There are a plethora of services (providers) that may assist you in creating your blog, but as a novice developer, I would recommend Github Pages. A professional tool that allows you to expand at your own pace while maintaining control over your postings.

---
## **How to host a website on github?**

STEP 1: Open [github.com](https://github.com/) and sign in or sign up with valid credentials. You'll most often see this landing page as shown in the image below. Your options to sign in or sign up will be available on the top right if your screen.

---
![](2021-12-27-12-15-57.png)

![](2021-12-27-12-28-30.png)

---
STEP 2: Download either [GitHub for Mac](https://desktop.github.com/) or [GitHub for Windows](https://desktop.github.com/), depending on your operating system. Open the app and log in using the account you just created.

---
![](2021-12-27-13-47-27.png)

---
STEP 3: (On Mac) - After you login, click advanced and make sure that your name and email are correct. Then, click "Install Command Line Tools", just in case you want to start using the command line later in life. Git is actually a command line tool, but GitHub's applications take its functionality and present it in an attractive interface.

---
![](![](tempsnip.png).png)

---
STEP 4: Create a new repository in your GitHub application. Name it your-username.github.io. The name is very important. Note the folder that GitHub is saving the repository to. Make sure the "Push to GitHub?" box is checked.

STEP 5: Move your website's files into the folder that GitHub just created when you made the repository. IMPORTANT: Your homepage HTML file must be called "index.html", and it must exist in the top-level directory.

STEP 6: Back in the GitHub application, you should see your files in the left column. Make sure they are all checked. If so, enter a message in the text box called "commit summary", something like "initial commit." Then, click the commit button.

STEP 7: Click the "Publish repo" button in the top right corner.

STEP 8: Give it about 10 minutes, then check your-username.github.io. Your website should be there!

---
## **Using custom domain names**

You can just leave your website at that address (it'll give you some serious street cred in the developer world), but if you have a custom domain you would like to use, it is very simple to make GitHub redirect your page.

1. Log in to your domain registrar and find where to change your host records. If you don't know, you can usually Google "(domain registrar) change host records", and your registrar will have an explainer telling you how to do it.
2. Change your domain's A Record to 204.232.175.78. This is GitHub's IP address, which allows GitHub to resolve your URL and serve the correct files.
3. In your website's directory folder on your computer, create a file called "CNAME". On the first line, type your domain name. Save the file.
4. In your GitHub application, you should see the file in the left column. Make sure it is checked and enter your commit message. Have it say something like "Adding CNAME file."
5. Click "Sync branches."

It can take as long as 48 hours for your domain to resolve to your GitHub page. However, it is usually pretty quick, so check back in an hour or so.

---
## **Push existing local repository to remote**

But what if you already have a local repository? How do you get that into GitHub?

If some of your projects already have local repositories setup on your developer machine, then you will need to add the [new GitHub repositories as remotes](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories). Just like when cloning a new repository, look for the remote URL in the upper right of your repository’s file viewer.

![](2021-12-27-14-10-02.png)

Now add the remote repository and name it “origin”. It doesn’t have to be named that, but it’s standard and matches what you would get if you used the git clone approach.

```bash
$ git remote add origin <URL to GitHub repo>
```

Confirm the remote was added properly

```bash
$ git remote -v
> origin <URL to GitHub repo> (fetch)
> origin <URL to GitHub repo> (push)
```

To push any commits that you have locally, use the following commands making note of the name of the remote repository to push against and the branch in which you want your changes included. If asked for credentials, you’ll need to use your GitHub username / email and password.

```bash
$ git push [remote] [branch]

# Example pushing the master branch to the origin remote
$ git push origin master
```

---
## **User Site vs Project Site**

Everyone gets a single user GitHub Page which is published from a repository that is dedicated to that page. This page is typically used to showcase you, your abilities, and a collection of your projects. Treat this like a landing page dedicated to you. You can brag about yourself and your credentials or just make a good-looking listing of all your repositories and their GitHub Page.

Project sites are infinite and only limited by the number of repositories attached to your GitHub account. Use these to spruce up the public persona of your project to attract even more attention. Sure, a README file is good, but it’s usually just text. With a GitHub Page, you can build a full-blown web-based experience to show off your project and its use cases.

To build your user site, you’ll need to create a repository named `<username>.github.io` so that GitHub knows this repository exists only to be published for your user GitHub Page. You would then access this page at `https://<username>.github.io` unless you’re using a custom domain.

---




