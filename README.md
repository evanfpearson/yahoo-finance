# Yahoo Finance Command Line Tool
Command line tool to download pricing data from yahoo finance with a time period and symbol.

## Usage 
`./yahoo <from_date> <to_date> <symbol>`

## Example
`./yahoo 2020-01-01 2020-06-01 "^DJI"`
This command will download daily data for the Dow Jones Index from Jan 1st 2020 to Jun 1st 2020

## Errors
There are a number of reasons this tool can fail
- `from_date` is after `to_date`
- either `from_date` or `to_date` is after today's date
- the dates are incorrectly formatted: i.e., not `%Y-%m-%d`
- yahoo responded with an error code
