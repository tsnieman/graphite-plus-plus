# graphite-plus-plus
Graphite.dev is a phenomenal dev tool that brings branch stacking to the masses (and so much more... they're eating Github's lunch, in my opinion).

This is a repo of links and tools that makes Graphite even more awesome. Feel free to contribute!

## Improving Github Access

### Bookmarklet

<img width="328" alt="image" src="https://user-images.githubusercontent.com/573204/229561599-3fa10597-0d40-4f21-a1c7-83054f3606c0.png">

You can add a bookmarklet to easily open Github from any Graphite page. Right-click in the bookmarks bar and click "Add Page". Title can be "Open in GH" or whatever you want, and URL is the following:

```
javascript:(function()%7B(()%3D>%7Bif (window.location.hostname %3D%3D%3D 'app.graphite.dev' %26%26 window.location.pathname.includes('%2Fgithub%2Fpr%2F')) %7Bconst pathname %3D window.location.pathname%3Bconst pieces %3D pathname.replace('%2Fgithub%2Fpr%2F'%2C '').split('%2F')%3Bconst githubUrl %3D %60https%3A%2F%2Fgithub.com%2F%24%7Bpieces%5B0%5D%7D%2F%24%7Bpieces%5B1%5D%7D%2Fpull%2F%24%7Bpieces%5B2%5D.split('%2F')%5B0%5D%7D%2F%60%3Bwindow.open(githubUrl)%3B%7D%7D)()%7D)()
```
![image](https://user-images.githubusercontent.com/573204/229560063-4b55ab38-bb92-40b4-b73b-7ee38c849b46.png)
