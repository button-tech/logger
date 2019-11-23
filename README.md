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

Log some info:
```
logger.Info("Successfully updated!")
```

Log errors:
```
logger.Error("information", err.Error(), logger.Params{
				"currency": "ETH",
                ...
})
```
Thanks for core of the logger to TRUST team !!!

https://github.com/trustwallet/blockatlas
