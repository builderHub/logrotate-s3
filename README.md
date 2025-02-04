# logrotate-s3
The utility scans a directory for '.log' files, zips and uploads them to s3 bucket, and removes the local copy.

### Usage
#### 1
./log_rotate.sh

Directory to scan: /var/logs

S3 bucket URL: s3://my-bucket/logs/

Choose mode: manual


#### 2
./log_rotate.sh

Directory to scan: /var/logs

S3 bucket URL: s3://my-bucket/logs/

Choose mode: schedule

Enter cron schedule: 0 2 * * *  (Runs daily at 2 AM)

→ Adds a cron job to perform log rotation daily at 2 AM.
