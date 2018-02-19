# tensorflow-wheels
Response to [https://github.com/yaroslavvb/tensorflow-community-wheels]https://github.com/yaroslavvb/tensorflow-community-wheels initiative!

#Builds

Forgive me, as I'm not very knowledgeable in this bazel build system, but result works for my purposes for now...
 
- Tensorflow 1.6.0 CPU Ubuntu 17.10 Python 3.6.3 AVX AVX2 FMA SSE4.1 SSE4.2 MKI
>bazel build -c opt --copt=-mavx --copt=-mavx2 --copt=-mfma --copt=-mfpmath=both --copt=-msse4.1 --copt=-msse4.2 --config=mkl -k //tensorflow/tools/pip_package:build_pip_package
