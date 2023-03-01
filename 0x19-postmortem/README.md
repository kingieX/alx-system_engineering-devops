# 0x19-postmortem

## Cause and resolution
while trying to ascertain the cause of the error, we had to trace it back to the root by running them on a test server which shows the same errors. so this means the error might be coming from somewhere else. after scanning through the files we discovered that the error was as a result of a typo in thr file extension >
> .phpp was used instead of 

> .php

To resolve that, we searched through the directory and fixing the typo error.

AFter that is done, the changes is committed and pushed. Then the server is restarted.


## prevention

This type of error is not from the server but from the application so to prevent this from happening again, we do the following

* Throughly test the application before deployment. This will help to point out such errors and prevented.

* Add status moitoring software which may enable uptime-monitoring services.
