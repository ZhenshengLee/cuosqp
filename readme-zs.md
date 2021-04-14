# cuosqp

## install cuosqp

修改`include/CMakeLists.txt`

```
# 添加下一行
"${CMAKE_CURRENT_SOURCE_DIR}/osqp_api_utils.h"
```

```sh
cmake .. -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/opt/osqp/cuosqp -DCUDA_SUPPORT=ON -DDFLOAT=ON -DDLONG=OFF -DUNITTESTS=ON
```

## install osqp-eigen

```sh
export osqp_DIR=/opt/osqp/cuosqp
cmake .. -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/opt/osqp-eigen/osqp-eigen
```

## todo:

[ ] change osqp target name to cuosqp
[ ] unittests all passed
