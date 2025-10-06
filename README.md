# Tensorflow-2.19.0-no-avx
Tensorflow 2.19.0 wheel for old CPUs without AVX.
Linux x86-x64
Built with Python 3.12

`bazel build //tensorflow/tools/pip_package:wheel --repo_env=USE_PYWRAP_RULES=1 --repo_env=WHEEL_NAME=tensorflow --config=cuda --config=cuda_wheel --copt="-mno-avx" --copt=-mno-avx2 --copt=-mno-fma`

Enjoy!
