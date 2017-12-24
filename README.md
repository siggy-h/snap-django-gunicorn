# Django-Gunicorn, Snapped!

Django-Gunicorn, Snapped! Is an awesome new way to deploy your Django applications.


This snap delivers two processes:
* Gunicorn
* Nginx

Nginx listens on the snap's private /tmp filesystem at `/tmp/django-gunicorn.sock` and is not visible to any other application or filesystem.


# Build
```bash
$ sudo snapcraft
```

# Install
```bash
$ sudo snap install django-gunicorn_0.1_amd64.snap --classic --dangerous
```


### TODO
* Make snap confined
* Snap nginx separate from django-gunicorn snap (this will make builds faster and a bunch of good/cool things possible)
* Possibily template this demo (ex `./create mynewproj` will create the directory layout and files with the correct names)


#### Author
* James Beedy (c) 2017 <jamesbeedy@gmail.com>

### Copyright
* AGPLv3 (see `copyright`)
