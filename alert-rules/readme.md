# Alert rules
This folder contains alert rules for different applications.

The alert rules must be passed to the approriate application.

## Rules

### Prometheus

- [low_memory.rules](./prometheus/low_memory.rules) -- This rules file contains two
rules. One for low memory alert specific to robot-2 and a generic rule for low memory for all the devices.
- [ros2_battery](./prometheus/ros2_battery.rules) -- This rule triggers when the ROS 2 topic `/battery_level` from a robot is below 10%. This is meant to work with the [ros2-grafana-agent](https://github.com/canonical/ros2-grafana-agent-example) example.

You can find more about Prometheus alert rules in the [official documentation](https://prometheus.io/docs/prometheus/latest/configuration/alerting_rules/).

### Loki

- [high_log_rate.rules](./loki/high_log_rate.rules) -- This rule triggers when the log
rate for an instance has exceeded 100 logs per second for the last 5 minutes.

You can find more about Loki alert rules in the [official documentation](https://grafana.com/docs/loki/latest/alert/).
