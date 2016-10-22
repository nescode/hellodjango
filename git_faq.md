### Git FAQ
While development you will come across several issue and questions with Git and GitHub. This page will give you a fair knowledge of how to address those common issues and questions.

### How to remove git cache and update `.gitignore`
Several times, we missed to update `.gitignore` and upload files which we should not. Follow this process to update and remove your `.gitignore` cache and update repositories.
```
$ git rm -r --cached .
$ git add .
$ git commit -m "Your message"
