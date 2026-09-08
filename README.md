# Linking Discord and GitHub

GitHub pages is hard to link to Discord, however, this was a reasonably easy way to get a `[username].github.io` domain on your Discord's Domain Connections

## Issues

I tried to make this as idiot proof as possible, if you face issues, please let me know via this repo's `Issues` tab, my Discord or Matrix (links on my main profile) and I'll try to help

## Setup
1) You need to fork this repo, by pressing the button below or pressing "Fork" at the top of this page.

[![Static Badge](https://img.shields.io/badge/fork-me?logo=forgejo&logoColor=white&color=black&size=150)](https://github.com/doughmination/.well-known/fork)

2) Open you Discord Settings, and follow these steps:
    - Open your connections and expand them out (this is at the very bottom of your settings!)
    
      ![](./media/to_connections.png)

    - Press the globe, which represents the domain

      ![](./media/globe.png)

    - Enter your domain as `your-github-username`.github.io (In my case, as my GitHub username is `doughmination`, my domain would be doughmination.github.io)

      ![](./media/enter_domain.png)

    - Change the method from DNS to HTTPS by pressing this button

      ![](./media/move-to-https.png)

    - Copy the "Contents" string

      ![](./media/copy-contents.png)

3) Back on GitHub, open the [discord](./discord) file, and edit it with the text you just copied, and click "Commit Changes"

   ![](./media/commit-works.png)

4) Deploy to GitHub Pages via these steps:
   - Click `Settings` on the very far top right
  
     ![](./media/settings.png)

   - Open up the `Pages` part of the settings

     ![](./media/pages.png)

   - Where it says `Branch`, change this from `None` to `main`

     ![](./media/choose-branch.png)

   - Click Save, and once it's saved, give it between 15-20 minutes, then repeat step 2. This time, it should automatically link, and not ask for any settings
  
     ![](./media/done.png)
