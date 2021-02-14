# dockerangular

Config for dockerizing your Angular projects in Docker!

### Instalation:

* Put files in your project directory.
* Copy contents of docker-compose.yml.dist to docker-compose.yml

<code>
	cp docker-compose.yml.dist docker-compose.yml
</code>

>You can remove .dist file now.

* Finish your docker-compose config - change host to that of your application
* Change start script in package.json file to:

<code>
	"start": "ng serve --host 0.0.0.0 --disableHostCheck",
</code>	

### Running app:

* Build your application container with:
<code>
  docker-compose build
</code>

> You need to rebuild your container after you installed new dependencies!

* Run your application:
<code>
  docker-compose up
</code>

>Thats it! Go to http://your-host/ and enjoy!
