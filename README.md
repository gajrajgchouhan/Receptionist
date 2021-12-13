# Receptionist

This website will notify you when your turn arrives for your interview.

## Description

Presently, we face issues when scheduling and managing queues for applications like virtual Interviews. There may be many interviewees in the queue and one person making it late or taking too much time messes up the schedule of others.

This website will show a pop-up message and send you a mail when the interviewer invites you to join the meeting. You will also be able to check your position in the queue so that you can plan your schedule to attend the interview.

## Usage

You just need to log in to the website with your email id with which you're registered for your interview. Then just wait for your turn.

Meanwhile, you can also complete your assignments or may even finish up your last slice of pizza :P without worrying about missing your turn.

Enjoy

## Tech Stack

-   Frontend: HTML, CSS, Javascript
-   Backend: Flask, Socket.IO, MongoDB, Redis

## Database

-   There are three MongoDB collections.

![Screenshot from 2021-07-28 17-17-19](https://user-images.githubusercontent.com/54475046/127317371-449393b2-28df-4a33-b7f8-c28347d6e3e2.png)

## How To Run

1. Install redis from redis.io
2. **Start Redis**.
3. Make your `constants.py`.

```python
ATLAS_ADMIN_PWD = ""
GOOGLE_CLIENT_ID = "xxx.apps.googleusercontent.com"
GOOGLE_SECRET = "-v5Y"
GOOGLE_DISCOVERY_URL = "https://accounts.google.com/.well-known/openid-configuration"
MJ_API_KEY = 'xxx'
MJ_API_SECRET = 'xxx'
EMAIL_ID = 'xxx@gmail.com'
EMAIL_PASSWORD = 'xxx'
```

5. Use the google cloud console to generate the appropriate ID/Secret. (Follow ![this](https://medium.com/@thomashellstrom/use-google-as-login-in-your-web-app-with-oauth2-352f6c7f10e6)) <!-- Can be improved -->
6. Make a MongoDB Atlas Document.
7. Install `requirements.txt`.
8. Run `run.sh`.

## BUGS

Only works on localhost currently ! SocketIO doesn't work on deployement 🚨

## License

[MIT](https://choosealicense.com/licenses/mit/)
