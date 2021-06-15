# Funny project

This is the starting point to lauch my porject, which is collection of some random funning project illustrating knowledge that I have.

To start the project, run the following command:
```
git clone https://github.com/jordanleeeee/FunnyProject.git
cd FunnyProject

git clone https://github.com/jordanleeeee/ReactQuestionBank.git
git clone https://github.com/jordanleeeee/QuestionBankBackend.git
git clone https://github.com/jordanleeeee/WebImageCrawler.git

docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d --build
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