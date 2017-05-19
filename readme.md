# Running Bookie in Docker

## Initialization

```
git clone https://github.com/ctco-dev/bookie-docker.git
cd bookie-docker
git submodule init && git submodule update
```

## Environment

Create `bookie.env` file with the content like:

```
CALENDAR_HOST=https://mail.company.com/home/${calendarName}/Calendar
ROOMS=[{"name":"Room name","email":"room.name.123@company.com","number":123,"floor":1,"capacity":20}]
MEETING_ORGANIZER=Bookie
MEETING_ORGANIZER_EMAIL=bookie@company.com
MAIL_HOST=mail.company.com
```

## Run it

`docker-compose up`

or

`docker-compose up -d` to run it as deamon

## Open in browser

Just open `http://localhost/` in browser
