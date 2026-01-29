# Spark Neural Network and Artemis1981 Integration Configuration

This directory contains configuration templates for integrating Spark MLlib Neural Networks with the Jury1981/Artemis1981 repository.

## Files

- **neural-network.conf.template**: Spark configuration for neural network settings
- **artemis-integration.properties.template**: Properties for Artemis1981 repository integration

## Usage

1. Copy the configuration files to the `conf/` directory:

```bash
# Copy neural network configuration
cp config/neural-network.conf.template conf/spark-defaults.conf

# Copy Artemis integration properties
cp config/artemis-integration.properties.template conf/artemis-integration.properties
```

2. Edit the files to customize settings for your environment.

3. Start Spark with the configuration:

```bash
./bin/spark-shell
# or
./bin/pyspark
```

## Configuration Options

### Neural Network Settings

- `spark.mllib.neuralnetwork.enabled`: Enable neural network support (default: true)
- `spark.mllib.neuralnetwork.defaultLayers`: Default number of hidden layers (default: 3)
- `spark.mllib.neuralnetwork.learningRate`: Learning rate for training (default: 0.01)
- `spark.mllib.neuralnetwork.maxIterations`: Maximum training iterations (default: 100)

### Mobile Broadband Settings

- `spark.broadband.neuro.enabled`: Enable broadband neuro network (default: true)
- `spark.broadband.neuro.batchSize`: Batch size for training (default: 32)
- `spark.broadband.neuro.optimizer`: Optimizer algorithm (default: adam)

### Artemis1981 Integration

- `spark.artemis.repository`: URL to Artemis1981 repository
- `spark.artemis.integration.enabled`: Enable integration (default: true)
- `artemis.data.sync.enabled`: Enable data synchronization (default: true)
- `artemis.neuralnet.coordination`: Enable neural network coordination (default: enabled)

## See Also

- [Neural Network Integration Guide](../docs/neural-network-artemis-integration.md)
- [Integration Overview](../NEURAL_NETWORK_INTEGRATION.md)
