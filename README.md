# buildkite_parallel

This tool will break apart tests to run in parallel on buildkite

## usage
`parallel_buildkite <runner> <test> [<test> ...]`

## examples
`parallel_buildkite make test1 test2`

## Optional ENV vars

### BUILDKITE_PARALLEL_JOB
job number must be less then BUILDKITE_PARALLEL_JOB_COUNT

### BUILDKITE_PARALLEL_JOB_COUNT
the number of total jobs

### DEBUG
set to "true" for all logs to be printed

### KEEP_LOGS
set to "true" if you want to keep logs on disk

### LOG_DIR
the directory the logs are stored in
(defaults to a directory created by mktemp -d)
