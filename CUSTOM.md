# hugo-vaf: An Adventure with Hugo for the "Visualizing Abolition & Freedom" Project

## First Install

```
cd ~/Projects/Docksal
fin project create
```

```
ma8660:Docksal markmcfate$ fin project create
1. Name your project (lowercase alphanumeric, underscore, and hyphen): **hugo-vaf**

2. What would you like to install?
  PHP based
    1.  Drupal 8
    2.  Drupal 8 (Composer Version)
    3.  Drupal 7
    4.  Wordpress
    5.  Magento
    6.  Laravel
    7.  Symfony Skeleton
    8.  Symfony WebApp
    9.  Grav CMS
    10. Backdrop CMS

  Go based
    11. Hugo

  JS based
    12. Gatsby JS

  HTML
    13. Static HTML site

Enter your choice (1-13): **11**

Project folder:   /Users/markmcfate/Projects/Docksal/hugo-vaf
Project software: Hugo
Project URL:      http://hugo-vaf.docksal

Do you wish to proceed? [y/n]: y
Cloning repository...
Cloning into 'hugo-vaf'...
remote: Enumerating objects: 42, done.
remote: Total 42 (delta 0), reused 0 (delta 0), pack-reused 42
Unpacking objects: 100% (42/42), done.
3. Installing site
 ALERT:  Some Docksal services were not running
         Restarting Docksal system services...
Configuring network settings...
Password:
Resetting Docksal services...
 ➔ proxy
 ➔ dns
   upstream 132.161.151.100
Enabling automatic *.docksal DNS resolver...
Clearing DNS cache...
 ➔ ssh-agent
Identity added: id_rsa (id_rsa)
Removing containers...
Removing network hugo-vaf_default
WARNING: Network hugo-vaf_default not found.
Removing volume hugo-vaf_cli_home
WARNING: Volume hugo-vaf_cli_home not found.
Removing volume hugo-vaf_project_root
WARNING: Volume hugo-vaf_project_root not found.
Removing volume hugo-vaf_db_data
WARNING: Volume hugo-vaf_db_data not found.
Volume docksal_ssh_agent is external, skipping
Identity added: id_rsa (id_rsa)
Starting services...
Creating network "hugo-vaf_default" with the default driver
Creating volume "hugo-vaf_cli_home" with default driver
Creating volume "hugo-vaf_project_root" with local driver
Creating volume "hugo-vaf_db_data" with default driver
Building cli
Step 1/2 : FROM docksal/cli:2.1-php7.1
2.1-php7.1: Pulling from docksal/cli
f2b6b4884fc8: Pulling fs layer
8db887c45800: Pulling fs layer
6e0e41c52c70: Pull complete
...
Digest: sha256:162f762eedd6ab9535e2d3d38c642d9de0ee5577cb459c0f40df40c42bab2f15
Status: Downloaded newer image for docksal/cli:2.1-php7.1
 ---> 4c7331d4cf77
Step 2/2 : RUN wget -q https://github.com/gohugoio/hugo/releases/download/v0.34/hugo_0.34_Linux-64bit.deb -O /tmp/hugo.deb     && dpkg -i /tmp/hugo.deb
 ---> Running in 143d21af3f03
Selecting previously unselected package hugo.
(Reading database ... 38368 files and directories currently installed.)
Preparing to unpack /tmp/hugo.deb ...
Unpacking hugo (0.34) ...
Setting up hugo (0.34) ...
Removing intermediate container 143d21af3f03
 ---> 9873d48c0b05
Successfully built 9873d48c0b05
Successfully tagged docksal/cli:hugo-0.34
Creating hugo-vaf_web_1 ... done
Creating hugo-vaf_cli_1 ... done
Waiting for hugo-vaf_cli_1 to become ready...
Connected vhost-proxy to "hugo-vaf_default" network.
WARNING: Removing ALL changes to current project in 5 seconds. Press Ctrl-C to cancel...
Initializing new hugo site...
Congratulations! Your new Hugo site is created in /var/www.

Just a few more steps and you're ready to go:

1. Download a theme into the same-named folder.
   Choose a theme from https://themes.gohugo.io/, or
   create your own with the "hugo new theme <THEMENAME>" command.
2. Perhaps you want to add some content. You can add single files
   with "hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>".
3. Start the built-in live server via "hugo server".

Visit https://gohugo.io/ for quickstart guide and full documentation.
/var/www/content/posts/my-first-post.md created
Downloading a theme...
Initialized empty Git repository in /var/www/.git/
Cloning into '/var/www/themes/ananke'...
remote: Enumerating objects: 23, done.
remote: Counting objects: 100% (23/23), done.
remote: Compressing objects: 100% (21/21), done.
remote: Total 1138 (delta 2), reused 11 (delta 1), pack-reused 1115
Receiving objects: 100% (1138/1138), 2.53 MiB | 3.05 MiB/s, done.
Resolving deltas: 100% (600/600), done.
Compiling a static site...

                   | EN  
+------------------+----+
  Pages            | 10  
  Paginator pages  |  0  
  Non-page files   |  0  
  Static files     |  3  
  Processed images |  0  
  Aliases          |  1  
  Sitemaps         |  1  
  Cleaned          |  0  

Total in 165 ms

Done!
  Open http://static.hugo-vaf.docksal
  To develop a Hugo site with real-time updates use fin develop (see README.md for details)

  Read more about Hugo on https://gohugo.io/getting-started/quick-start/
ma8660:Docksal markmcfate$
```
