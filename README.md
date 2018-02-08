## Building a Real-Time Object Recognition App with Tensorflow and OpenCV

## Requirements

* some [pre-trained models](https://github.com/tensorflow/models/blob/477ed41e7e4e8a8443bc633846eb01e2182dc68a/object_detection/g3doc/detection_model_zoo.md) (especially with a focus on light-weight models, so that they can run on mobile devices)

* a [Jupyter notebook](https://github.com/tensorflow/models/blob/master/research/object_detection/object_detection_tutorial.ipynb) example with one of the released models

* Download the frozen model [(.pb — protobuf)](https://developers.google.com/protocol-buffers/) and load it into memory
    ```angular2html
    # From tensorflow/models/research/
    protoc object_detection/protos/*.proto --python_out=.
    ```