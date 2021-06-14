# Funny project

This is the starting point to lauch my porject, which is collection of some random funning porject illustrating knowledge that I have.

To start the project, run the following command:
```
git clone https://github.com/jordanleeeee/FunnyProject.git
cd FunnyProject

git clone https://github.com/jordanleeeee/ReactQuestionBank.git
git clone https://github.com/jordanleeeee/QuestionBankBackend.git
git clone https://github.com/jordanleeeee/WebImageCrawler.git

docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d --build
```
then you can have fun in http://www.jordanleeeee.com

<br/>
To terminate the project

```
docker-compose -f docker-compose.yml -f docker-compose.prod.yml down
```

Language/Framework/technology used:
- frondend
  - react
    - react router
    - ...
- backend
  - nodejs
    - express
  - python
    - flask
  - ...
- devOps
  - docker
  - docker compose
  - ...