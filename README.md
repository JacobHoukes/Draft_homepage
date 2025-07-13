# Draft Homepage

This is a simple personal homepage project built using HTML and CSS. It serves as a brief introduction and includes a profile image, a job title, a welcome message, and a link to my LinkedIn profile.

## Features

- Displays a profile picture.
- Shows name and title.
- Provides a link to LinkedIn.
- Styled with an external CSS file.

## Project Structure

```
Draft_homepage/
│
├── static/
│   ├── profile_pic.jpeg        # Profile image
│   └── style.css               # Stylesheet
│
├── templates/
│   └── index.html              # HTML file rendered for the homepage
│
├── requirements.txt            # Python package requirements (if expanded)
└── README.md                   # This file
```

## Usage

To run this project using a Python web framework like Flask:

### 1. Install Flask

Make sure Flask is installed:

```bash
pip install flask
```

### 2. Create a Flask App

Create a file named `app.py` and add the following code:

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return render_template('index.html')

if __name__ == '__main__':
    app.run(debug=True)
```

### 3. Run the App

From the root of the project directory, run:

```bash
python app.py
```

Then open your browser and navigate to:

```
http://127.0.0.1:5000/
```

## Author

**Jacob Houkes**  
[My LinkedIn profile](https://www.linkedin.com/in/jhoukes/)
