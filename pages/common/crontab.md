# crontab

> Schedule cron jobs to run on a time interval for the current user.
>
> Job definition format: "(min) (hour) (day_of_month) (month) (day_of_week) command_to_execute" - month maybe numeric 1-12 or JAN-DEC; day_of_week maybe numeric 0-6 or SUN-SAT

- Edit the crontab file for the current user:

`crontab -e`

- View a list of existing cron jobs for current user:

`crontab -l`

- Remove all cron jobs for the current user:

`crontab -r`

- Sample job which runs at 10:00 every day. * means any value:

`0 10 * * * {{path/to/script.sh}}`

- Sample job which runs every minute on the 3rd of April:

`* * 3 Apr * {{path/to/script.sh}}`

- Sample job which runs at 02:30 every Friday:

`30 2 * * Fri {{path/to/script.sh}}`
