
### uWSGI
---
.py
https://uwsgi-docs.readthedocs.io/en/latest/

```py
def application(env, start_response):
  start_response('200 OK', [('Content-Type', 'text/html')])
  return [b"Hello World"]

from flask import Flask
app = Flask(__name__)
@app.route('/')
def index():
  return "<span style='color:red'>I am app 1</span>"

my $app = sub {
  my $env = shift;
  return [
    '200',
    [ 'Content-Type' => 'text/html' ],
    [ "<h1>Hello World</h1>" ],
  ];
};

my $uwsgi_opt = uwsgi::opt;
print $uwsgi_opt->{'http'};

class App
  def call(environ)
    [200, {'Content-Type' => 'text/html'}, ['Hello']]
  end
end
run App.new

from flask import Flask
app = Flask(__name__)
@app.route("/")
def hello():
  return "Hello World! i am app1"
  
from flask import Flask
app = Flask(__name__)
@app.route("/")
def hello():
  return "Hello World! i am app3"

from pprint import pprint
def application(environ, start_response):
  start_response('200 OK', [('Content-Type', 'text/plain')])
  return ['It Works!']
def auth_kafka(request_uri, http_cookie, http_authorization):
  pprint(locals())
  return 'true'
import uwsgi
uwsgi.register_rpc('auth_kafka', auth_kafka)

ws = new WebSocket('ws://127.0.02:8000/?subscribe=true')
```

```rb
require 'sinatra'
get '/hi' do
  "Hello World"
end
run Sinatra::Application
```


```
```



