<b> <center>Full Stack Web DEvelopment Using Python HTML<sub>5</sub>,CSS<sub>3</sub> and JavaScript.</center> </b>

<p style="text-align:justify;"> I will be creating an full function web app using python Microframework called FLASK, the final product will be an authetication page where a user can Register and create account, the they can log in and end up to a landing page  where they cancomment and share a post. </p> 

<p style="text-align:justify;">
 Flask is a web framework. This means flask provides you with tools, libraries and technologies that allow you to build a web application. This web application can be some web pages, a blog, a wiki or go as big as a web-based calendar application or a commercial website.
</p>

<p style="text-align:justify;"> 
Flask is part of the categories of the micro-framework. Micro-framework are normally framework with little to no dependencies to external libraries. This has pros and cons. Pros would be that the framework is light, there are little dependency to update and watch for security bugs, cons is that some time you will have to do more work by yourself or increase yourself the list of dependencies by adding plugins. In the case of Flask, its dependencies are:
  </p>
  <ul>
  <li>Werkzeug a WSGI utility library </li>
  <li>jinja2 which is its template engine</li>
  </ul>
  <p style="text-align:justify;">
  Where WSGI is basically a protocol defined so that Python application can communicate with a web-server and thus be used as web-application outside of CGI  while Jinja2 is a template engine for Python.  You can use it when rendering data to web pages.  For every link you visit, you want to show the data with the formatting. By using a template engine we can seperate display logic (html, css) from the actual Python code. </p>


<b><center> A simple python Hello world code from tempalates. </center> </b>
<p style="text-align:justify;">
Preriquisetes for ubuntu users:
 <ol>
  <li> sudo apt install python3-venv- to install virtual environment </li>
  <li> python3 -m venv <env name>  creating virtual environment for development. </li>
  <li> source <env name>/bin/activate - activating environment</li>
  <li> pip install flask -To use python package manager to install flask. </li>
 </ol>
  <p style="text-align:justify;">
 <b> Note:</b> Flask looks for templates index files in a folder called <b>tempalates</b>, statics files images, JavaScripts and Cascading Style Sheet in a <b> static</b> folder.
 <b>1). app.py </b>
 <pre>
from flask import Flask
# Create the application.
app = Flask(__name__)

@APP.route('/')
def index():
    """ Displays the index page accessible at '/'
    """
    return flask.render_template('index.html')

if __name__ == '__main__':
    app.debug=True
    app.run()
 </pre>
 </p>
 
 
 
 
 
  <p style="text-align:justify;">
 
 <b> templates/index.html </b>
 <pre>
 <!DOCTYPE html>
<html lang='en'>
<head>
  <meta charset="utf-8" />
  <title>Hello world!</title>
  <link type="text/css" rel="stylesheet"href="{{ url_for('static', filename='hello.css')}}" />
</head>
<body>

This is a flask page 

</body>
</html>
 
 </pre>
 
 <p>
