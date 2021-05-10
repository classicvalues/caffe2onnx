# caffe-onnx
This tool converts Caffe models to ONNX via command line.

## Introduction
**caffe-onnx** is based on previous [work](https://github.com/htshinichi/caffe-onnx) by [htshinichi](https://github.com/htshinichi). 

## Installation
Install from pypi  
`
pip install caffe-onnx
`

Install latest from github  
`
pip install git+https://github.com/asiryan/caffe-onnx
`

Build and install latest from source (for development)  
`
git clone https://github.com/asiryan/caffe-onnx
`

Once dependencies are installed, from the caffe-onnx folder call:  
`
python setup.py install
`  

## Usage
To get started with caffe-onnx, run the caffe2onnx.convert command, providing:
* the path to your caffe prototxt,
* the path to your caffe model,
* the output path of the onnx model,
* the flag (frozen graph or not).

```
usage: convert2onnx.py [-h] [prototxt] [caffemodel] [onnx] [frozen]

positional arguments:
  prototxt          caffe's prototxt file path
  caffemodel        caffe's caffemodel file path
  onnx              onnx model name
  frozen            frozen graph or not
```

Simple example of usage:  
`
python -m caffe2onnx.convert --prototxt googlenet.prototxt
`

## License
BSD-3
