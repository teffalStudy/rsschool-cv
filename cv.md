# Resume

## First Name

Konstantin

## Last Name

Ryzhankov

## Contact Info

* **e-mail:** teffal@mail.ru
* **skype:** rka3011
* **phone:** +7 (911) 347-49-47

## Summary

I want to become a professional backend developer. I am interested in developing front-end using vuejs.

It is very interesting to implement a Python backend with a web interface on vuejs.

I would like to apply the accumulated experience in teaching programming for beginners, in particular the creation of interactive training programs.

## Skills

* python 3
* vuejs
* html

## Code examples

```py
class GenDoc:
    def __init__(self, contents):
        self.contents = contents
        self.text = ''
        for line in contents:
            self.add_title(line['title'])
            self.get_text(line['path'])

    def add_title(self, title):
        if title:
            self.text += f'\n# {title}\n'

    def add_text(self, text_file, path_img):
        next_string = text_file.readline()
        while next_string:
            if next_string.strip()[:2] == '![':
                next_string = f"![]{next_string.replace('./img', f'{path_img}/img').split(']')[1]}"
            self.text += next_string
            next_string = text_file.readline()

    def create_doc(self, name):
        pypandoc.convert_text(self.text, format='md', to='docx', outputfile=f"{name}.docx")

    def get_text(self, pathes):
        for path in pathes:
            with open(f"{path}README.md", encoding='utf8') as f:
                self.add_text(f, path)
```

## Experience

For the last two years I have been a teacher and course developer: Python, VUE, and Robotics.

My sites:

* python tutorial: [https://learn4kid-python.firebaseapp.com/](https://learn4kid-python.firebaseapp.com/)
* tutorial vuepress: [https://learn4kid-vuepress.firebaseapp.com/](https://learn4kid-vuepress.firebaseapp.com/)
* textbook for reading English with voice synthesis: [https://teffal.github.io/](https://teffal.github.io/)

## Education (including courses, seminars, lectures, online learning)

Professional education:

* electrician technician (2000-2003)
* civil engineer (2004-2008)
* industrial climber (2012)

Professional retraining courses:

* programming python (2016)
* programming js (2016)

# English

* B1 intermadiate
