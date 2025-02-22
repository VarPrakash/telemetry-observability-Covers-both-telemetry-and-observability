# OpenTelemetry Example

This repository contains an OpenTelemetry example project that demonstrates how to set up observability using OpenTelemetry.

## Prerequisites

Ensure you have the following installed on your system before proceeding:

- [OpenTelemetry Collector](https://opentelemetry.io/docs/collector/)
- [Jaeger](https://www.jaegertracing.io/) (for tracing visualization)
- [Prometheus](https://prometheus.io/) (for metrics monitoring)
- [Grafana](https://grafana.com/) (for dashboard visualization)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/VarPrakash/opentelemetry-example.git
   cd opentelemetry-example
   ```

2. Start OpenTelemetry Collector:
   ```sh
   docker-compose up -d
   ```

3. Verify that the services are running:
   ```sh
   docker ps
   ```

## Usage

1. Run the application with OpenTelemetry enabled.
   ```sh
   go run main.go
   ```

2. View traces in Jaeger:
   - Open [http://localhost:16686](http://localhost:16686) in your browser.

3. Monitor metrics in Prometheus:
   - Open [http://localhost:9090](http://localhost:9090) in your browser.

4. Visualize data in Grafana:
   - Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```
opentelemetry-example/
├── main.go        # Application code
├── docker-compose.yml # OpenTelemetry and monitoring setup
├── config.yaml    # OpenTelemetry Collector configuration
├── README.md      # Project documentation
```

## Additional Resources

For more files and examples, you can clone the official OpenTelemetry demo repository:
[OpenTelemetry Demo](https://github.com/open-telemetry/opentelemetry-demo.git)

## License

This project is licensed under the MIT License.

## Author

[VarPrakash](https://github.com/VarPrakash)
