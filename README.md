# BUTTON LOGGER

Usage:

env DSN - sentry token

```
func init() {
	if err := logger.InitLogger(os.Getenv("DSN")); err != nil {
	       log.Fatal(err)
	}
}
```

Log some info(not error) to sentry:
```
logger.SendMessage("Successfully updated!")
```

Log some info to stdout:
```
logger.Info("Successfully updated!")
```

Log errors:
```
logger.Error("GetBalance", err.Error(), logger.Params{
	       "currency": "ETH",
                ...
})
```
Thanks for the core of the logger to the TRUST WALLET team !!!

https://github.com/trustwallet/blockatlas
