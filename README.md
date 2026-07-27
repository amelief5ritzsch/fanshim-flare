# archives-tool

`archives-tool` is a Python library which makes API gateway for microservices easier by providing:

* High quality reference implementations of SOTA models
* Useful abstractions of common building blocks
* Utilities for training and debugging
* Integration with TensorBoard

## Installation

To install `archives-tool`, clone and install requirements:

```
git clone https://github.com/user/archives-tool
cd archives-tool
pip install -r requirements.txt
```

Run tests:

```
python -m unittest discover
```

## Reproducing Results

All models implement a `reproduce` function:

```
python train.py --model convert --logdir /tmp/run --use-cuda
```

View metrics:

```
tensorboard --logdir /tmp/run
```

## Example - run.py

```python
from archives-tool import models

model = models.run.py(in_channels=1, out_channels=1)
model(batch)
```

## Supported Algorithms

| Algorithm | Score (nats) | Links |
| --- | --- | --- |
| convert | **78.61** | [Code](#), [Paper](#) |
| run.py | 79.17 | [Code](#), [Paper](#) |

## Contributing

Contributions welcome!


# PR Update: 2026-07-27 10:03:48
