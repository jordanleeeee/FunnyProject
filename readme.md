# Funny project

This is the starting point to lauch my porject, which is collection of some random funning project illustrating knowledge that I have.

Setup docker in Ubuntu
```
sudo apt-get update
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
rm get-docker.sh 
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

To start the project, run the following command:
```
git clone https://github.com/jordanleeeee/FunnyProject.git
cd FunnyProject

git clone https://github.com/jordanleeeee/ReactQuestionBank.git
git clone https://github.com/jordanleeeee/QuestionBankBackend.git
git clone https://github.com/jordanleeeee/WebImageCrawler.git

sudo docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d --build
```

run these two command for the first time to restore database
```
sudo docker exec -it funnyproject_mongodb_1 bash
mongorestore /home/ -u root
exit
```

hahaha, those are private repo, you cannot access it. However you can have fun in http://www.jordanleeeee.com

<br/>
To terminate the project

```
docker-compose -f docker-compose.yml -f docker-compose.prod.yml down
```

### Language/Framework/technology used:
- Frondend
  - react
    - react router
    - functional component
    - class component
  - i18n
- Backend
  - nodejs
    - express
      - express router
      - express middleware
    - aws-sdk
      - multer-s3
    - winston logging
    - pdfkit
    - jszip
  - python
    - flask
    - beautifulsoup
  - database
    - mongodb
    - redis
- DevOps
  - docker
  - docker compose
  - nginx

### Todo:
  - fix cannot multiple login bug
  - add env config in frontend in an attempt to connecting to differet host in dev and prod environment
  - fix request timeout issue
  - setup regular schedule to clean cache