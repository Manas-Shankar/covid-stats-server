# covid-stats-server

A server built using nodeJS and ExpressJS that acts as the backend for the covid-stats-website.
<br>Performs daily inserts (at 4 AM) into the database by retrieving data scraped by [india-covid-scraper](https://github.com/Manas-Shankar/india-covid-scraper) and [world-covid-scraper](https://github.com/Manas-Shankar/world-covid-scraper).<br>
Also retrieves user data (name,phone number and region) submitted via a form on the website and sends a sms message containing daily statistics for their entered region. This is done everyday at 9 AM.<br>
Uses [node-cron](https://www.npmjs.com/package/node-cron) for scheduling tasks and the FAST2SMS service to send messages
