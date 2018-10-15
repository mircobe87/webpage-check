# webpage-check
*A bash script based on SENDGRID (https://sendgrid.com/)
that notifyes you via e-mail when a given web page become reachable*.

This application is based on *SENDGRID*, so you have to provide a valid
*API KEY* to be able to use *SENDGRID*'s REST API. Before calling this script
make sure you have exported the environment variable **SENDGRID_API_KEY**.

To obtain a valid *API KEY* please visit the related documentation on *SENDGRID*
web site at https://sendgrid.com.

## Usage

    webpage-check [OPTIONS]...

### Options

+ __-f, --from-addr__:  Set the e-mail address for the sender. The default value
                        is `webpage-checker@script.bash`.
+ __-F, --from-name__:  Set the name for the sender. The default value is
                        `Webpage Cheker`.
+ __-h, --help__:       Shot this help.
+ __-m, --message__:    Set the e-mail body messate. An empty string is the
                        default value.
+ __-r, --recipients__: A comma separated list of e-mail addresses used as
                        recipients. This value is mandatory.
+ __-s, --subject__:    Set the e-mail subject. If omitted the default value
                        `Webpage is ONLINE` is used.
+ __-u, --url__:        Set the target URL that we want to check. This value
                        is mandatory.
+ __-v, --version__:    Show version info.
+ __-w, --wait__:       Set the time that will pass betweet two consecutive
                        checks in the format **NUMBER[SUFFIX]**. **SUFFIX** may
                        be `s` for seconds (the default), `m` for minutes, `h`
                        for hours or `d` for days.
