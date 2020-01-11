[![HitCount](http://hits.dwyl.io/ro6ley/django_ec2.svg)](http://hits.dwyl.io/ro6ley/django_ec2)

# Django_Redis

This repository contains the code for this [blogpost](https://stackabuse.com/deploying-django-applications-to-aws-ec2-with-docker/).

## Getting Started

### Prerequisites

Kindly ensure you have the following installed on your machine:

- [ ] [Python 3](https://realpython.com/installing-python/)
- [ ] [Pipenv](https://pipenv.readthedocs.io/en/latest/#install-pipenv-today)
- [ ] [Docker](https://www.docker.com/products/docker-desktop)
- [ ] [Git]()
- [ ] An IDE or Editor of your choice

### Running the Application

1. Clone the repository
```
$ git clone https://github.com/ro6ley/django_ec2.git
```

2. Check into the cloned repository
```
$ cd django_ec2
```

3. If you are using Pipenv, setup the virtual environment and start it as follows:
```
$ pipenv install && pipenv shell
```

4. Install the requirements
```
$ pip install -r requirements.txt
```

5. Start the Django API
```
$ python manage.py runserver
```

6. Navigate to `http://localhost:8000`

7. Build the Docker image:
```
$ docker build . -t django_ec2
```

8. Publish the Docker image to Dockerhub:
```
$ docker tag django_ec2 <DOCKERHUB_USERNAME>/django_ec2
$ docker push <DOCKERHUB_USERNAME>/django_ec2
```

9. Deploy on AWS EC2 as outlined in this [article](https://stackabuse.com/deploying-django-applications-to-aws-ec2-with-docker/)

## Contribution

Please feel free to raise issues using this [template](./.github/ISSUE_TEMPLATE.md) and I'll get back to you.

You can also fork the repository, make changes and submit a Pull Request using this [template](./.github/PULL_REQUEST_TEMPLATE.md).
