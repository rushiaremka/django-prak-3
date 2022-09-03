# PBP Django Project Template

Platform-Based Programming (CSGE602022) - Organized by the Faculty of Computer Science Universitas Indonesia, Odd Term 2022/2023

*Read this in other languages: [Indonesia](README.md), [English](README.en.md)*
## Preliminary

This repository is a template that is designed to help students who take the Program-based Development/Programming Course (CSGE602022) to know the structure of a Django application project and the files and configurations that are important in running the application. You can freely copy the contents of this repository or utilize this repository as a learning material and also as a starting point to build a Django application project.

## How to Use

If you want to use this repository as a starter repository that you will later modify,

1. Clone this repository to your local.

2. Log into the cloned repository and run the following command to start the virtual environment.

        python -m venv env

3. Power on the environment with the following command.

        Linux/Unix: source env/bin/activate
        Windows: env\bin\activate
4. Install the dependencies needed to run the application with the following command.

        pip install -r requirements.txt

5. Run the Django application with the manage.py runserver command
6. Open http://localhost:8000 in your favorite browser to see if the application is running correctly.

## Deployment Example

In this template, the deployment is completed by utilizing GitHub Actions as a runner and Heroku as an application Hosting platform.

To implement the deployment, you can read the instructions at [Tutorial-0](https://github.com/pbp-fasilkom-ui/ganjil-2023/blob/master/assignments/tutorial/tutorial-0.md).

For the deployed Django application example, you can access it at  [https://django-pbp-template.herokuapp.com/](https://django-pbp-template.herokuapp.com/)

## Credits
This template was based on [PBP Odd 2021](https://gitlab.com/PBP-2021/pbp-lab) written by 2021 Platform Based Programming Teaching Team ([@prakashdivyy](https://gitlab.com/prakashdivyy)) and [django-template-heroku](https://github.com/laymonage/django-template-heroku) written by [@laymonage, et al.](https://github.com/laymonage). This template is designed in such a way so that students can use this template as a starter and reference in doing assignments and their work.