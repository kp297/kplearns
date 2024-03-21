+++
title = 'Hugo Commands'
date = 2024-03-21T02:51:34-04:00
draft = false
+++

I use Hugo for this website. That doesn't mean I actually know all the commands. These are the basic commands that have been serving me well. 

```shell
hugo version
```

Create new website package/folder
```shell
hugo new site newwebsite 
cd newwebsite 
```

Start server locally
```shell
hugo server 
hugo server -D (for drafts)
```

Add new content
```shell
hugo new content posts/my-first-post.md
```

Publish the site
```shell
hugo
```

After this, the file will be in the public folder

To clean the public folder for new build: Delete the public folder and rebuild it.
