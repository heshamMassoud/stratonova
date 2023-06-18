# Stratonova™
Stratonova™ is your running buddy. Stratonova™ is a [Strava](strava.com) add-on application. Stratonova™ summarises your run right after you finish it. No need for input from you. Just finish your run and enjoy a witty storytelling summary automatically posted on your strava activity.

Stratonova™ will also name your run according to the type of run it was from each of the following:
- Interval training 💪🛤️
- Short but Sweet 💁🏽‍♂️
- Long Run ☄️
- Threshold Training 🚀🚀🚀
- Easy Flow 🌊🌊



## Example
https://www.strava.com/activities/9263490351

<img width="893" alt="Screenshot 2023-06-17 at 23 00 50" src="https://github.com/heshamMassoud/stratonova/assets/9512131/3db3eccb-f13f-440f-849d-09aa26d3f03d">


## Current Usage



### `/`
https://stratonova-l5snujqyaq-ew.a.run.app/

Homepage with instructions how to authenticate your strava account. 

### `/exchange_token?code={code}`

https://stratonova-l5snujqyaq-ew.a.run.app/exchange_token?code={code}

Exchanges a code for a short-lived Strava access token that can be used for further requests.

### `/update_workout?workout_id={workout_id}`

https://stratonova-l5snujqyaq-ew.a.run.app/update_workout?workout_id={workout_id}

Updates the Strava workout of the supplied `workout_id` with a new description and name describing how the run went.

## Future Work
In the future, Stratonova™ will do more spicy things like post your run story on socials (e.g. instagram, twitter) automatically. So you don't have to do any manual work after you finished your run.



### Run locally
````bash
go mod tidy
````

````bash
go build -v cmd/main.go
````

````bash
go run cmd/main.go
````

### Debug
````bash
dlv debug --headless --listen=:2345 --api-version=2 --accept-multiclient
````
