# yonamine.github.io

# Table of Contents
1. [How to run locally](#how-to-run-locally)





## How to run locally
1. You can use the `Jekyll` command

```shell
$ jekyll serve
```

In the current version, there's no live update. If you add, delete or change any file, you should kill the jekyll process (pressing `ctrl + c`) and run the above comand again.

2. Or you can run the Python3 WebServer

Run the following command:
```shell
$ jekyll build --watch
```
It will re-build the whole Jekyll project, every time you add, delete or change any file from your project. The Jekyll process will be running until you kill it ((pressing `ctrl + c`)).

And then, run the next command:
```shell
$ python3 -m http.server --directory _site/ 4000
```
In Python3, there's a simple HTTP server. In our case, it's enough to run our web site. I am passing the port **4000** and the directory served is "**_site**", like `jekyll serve`.

3. Or even NodeJS

I'll skip it but it's very easy to create a simple web server.

4. Open any browser

Then, open any web browser and go to [http://127.0.0.1:4000/](http://127.0.0.1:4000/).
Note that if you change the port value, you have to change in the URL as well.


* * *
[◀ BACK](#table-of-contents)
<br/><br/><br/>


