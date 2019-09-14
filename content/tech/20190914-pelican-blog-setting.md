Title: python pelican blog config
Date: 2019-09-14 10:20
Modified: 2019-09-14 10:20
Category: Python
Tags: pelican, publishing
Slug: pelican-blog-setting
Authors: yjkim 
Summary: pelican


# install pelican dependency


```sh 
# virtualenv  
$ sudo pip install virtualenv

# pelican plugin 
$ pip install pelican ghp-import Markdown typogrify pelican
```

# activate pelican venv

```sh 
$ mkdir blog && cd blog
$ virtualenv -p python3 venv
$ source venv/bin/activate
$ source venv/bin/activate

```

# start pelican blog with pelican-quick-start 

```sh 
$ pelican-quickstart

 (venv) î‚° yjkim@yjkim-pc î‚° ~/workspaces/blog î‚° pelican-quickstart
Welcome to pelican-quickstart v4.1.1.

This script will help you create a new Pelican-based website.                                                          
                                                                                                                       
Please answer the following questions so this script can generate the files               
needed by Pelican.                                                                                                     
                                                                                                                       
                                                                                                                       
> Where do you want to create your new web site? [.]                                                                   
> What will be the title of this web site? yjkim blog                                                                  
> Who will be the author of this web site? yjkim                                                                       
> What will be the default language of this web site? [ko] ko                             
> Do you want to specify a URL prefix? e.g., https://example.com   (Y/n) n                
> Do you want to enable article pagination? (Y/n) Y                                                                    
> How many articles per page do you want? [10]                                                                         
> What is your time zone? [Europe/Paris] Asia/Seoul                                                                    
> Do you want to generate a tasks.py/Makefile to automate generation and publishing? (Y/n) Y
> Do you want to upload your website using FTP? (y/N) n                                                                
> Do you want to upload your website using SSH? (y/N) n                                                                
> Do you want to upload your website using Dropbox? (y/N) n                                                            
> Do you want to upload your website using S3? (y/N) n                                                                 
> Do you want to upload your website using Rackspace Cloud Files? (y/N) n                                              
> Do you want to upload your website using GitHub Pages? (y/N) Y            
> Is this your personal page (username.github.io)? (y/N) Y                                                             
Done. Your new project is available at /home/yjkim/workspaces/blog    



```


# install pelican themes

* pelican 은 다른 블로그 생성기와 마찬가지로 theme 를 여러 사람들이 제작해놓은 사이트 들이 있기에 참조하여서 만들어 주면 된다. 

```sh
$ git clone --recursive https://github.com/getpelican/pelican-themes

```

# install pelican plugin 

* 요기는 추가로 정리 예정 
* 추천하는 plugin 이 있어보임 
 - https://github.com/getpelican/pelican-plugins
 - https://www.sysadminnotes.ca/worknotes/useful-pelican-plugins.html
