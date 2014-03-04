-flask-bigpipe
==============

python flask bigpipe package

example:

import bigpipe

app = Flask('website')
bigpipe.BigPipe(app)

@app.route('/')
def root():
    bigpipe.scriptstring =  "\
                <script>\
                     alert('my bigpipe')\
                </script>\
                "
    return render_template('home1.html')

app.run()
