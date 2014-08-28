aws-cloudwatch
==============

A simple Polymer element to retrieve statistics data from the AWS CloudWatch service.

[Documentation](http://guardian.github.io/element-aws-cloudwatch/)

## Example

``` html
<aws-cloudwatch config="{{awsContent}}"
                namespace="AWS/ELB"
                metricname="Latency"
                starttime="{{timeRangeStart}}"
                endtime="{{timeRangeEnd}}"
                resolution="60"
                statistics="average maximum"
                sink="{{latencyStats}}">
    <aws-dimension name="LoadBalancerName"
                   value="some-aws-ID" />
</aws-cloudwatch>
```
