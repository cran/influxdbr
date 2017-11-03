# influxdbr 0.13.0.9000

## Breaking changes

* `influx_write` function argument `xts` changes to `x` (method is now generic)

## New features

* `influx_write` now accepts data.frames to upload mulitple tags and fields per timestamp (#20).

## Bug fixes

* correct parsing of json structure without `statement_id` (#32).

* special characters in `xts` attributes are now supported (#30).

* Fix special character representation in `show_series`.

* Using double quotes in string arguments of `influx_query` wrappers (e.g. `influx_select`, `show_tag_values`) (#22).

* IQL wrapper functions with no expected return value now use `influx_post` instead of `influx_query`.  

# influxdbr 0.13.0

* Fix coercion error in `influx_write()` in case of sub-second accuracy (#25).

* `influx_select()` correctly parses integer arguments (#27).

* Significantly improved performance of `influx_query()` (#28).

# influxdbr 0.12.0

* First CRAN release