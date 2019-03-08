# fluent-plugin-out-stena, a plugin for [Fluentd](http://fluentd.org)

A generic [fluentd][1] output plugin for sending logs to Stena-Agent

## Configuration options

    <match *>
      @type stena
      endpoint_url    http://localhost.local/predict
      rate_limit_msec 100    # default: 0 = no rate limiting
      raise_on_error  false  # default: true
      buffered        true   # default: false. Switch non-buffered/buffered mode
    </match>

## Usage notes

If you'd like to retry failed requests, consider using [fluent-plugin-bufferize][3].

----

  [1]: http://fluentd.org/
  [2]: https://github.com/tagomoris/fluent-plugin-growthforecast
